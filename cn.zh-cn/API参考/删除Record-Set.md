# 删除Record Set<a name="dns_api_64005"></a>

## 功能介绍<a name="section49332166"></a>

删除单个Record Set。

## URI<a name="section41336317"></a>

DELETE /v2/zones/\{zone\_id\}/recordsets/\{recordset\_id\}

参数说明请参见[表1](#table52104579)。

**表 1**  URI格式的参数说明

<a name="table52104579"></a>
<table><thead align="left"><tr id="row50570707"><th class="cellrowborder" valign="top" width="19.878012198780123%" id="mcps1.2.5.1.1"><p id="p2586631"><a name="p2586631"></a><a name="p2586631"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.748725127487251%" id="mcps1.2.5.1.2"><p id="p8190559"><a name="p8190559"></a><a name="p8190559"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.80871912808719%" id="mcps1.2.5.1.3"><p id="p540664720479"><a name="p540664720479"></a><a name="p540664720479"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.56454354564543%" id="mcps1.2.5.1.4"><p id="p59455556"><a name="p59455556"></a><a name="p59455556"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row51170717"><td class="cellrowborder" valign="top" width="19.878012198780123%" headers="mcps1.2.5.1.1 "><p id="p51187411"><a name="p51187411"></a><a name="p51187411"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.748725127487251%" headers="mcps1.2.5.1.2 "><p id="p52539597"><a name="p52539597"></a><a name="p52539597"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.80871912808719%" headers="mcps1.2.5.1.3 "><p id="p18406147194716"><a name="p18406147194716"></a><a name="p18406147194716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.56454354564543%" headers="mcps1.2.5.1.4 "><p id="p27848947"><a name="p27848947"></a><a name="p27848947"></a>所属zone的ID。</p>
<p id="p1528562011414"><a name="p1528562011414"></a><a name="p1528562011414"></a>公网Zone ID可以通过<a href="查询公网Zone列表.md">查询公网Zone列表</a>获取。</p>
<p id="p22777371252"><a name="p22777371252"></a><a name="p22777371252"></a>内网Zone ID可以通过<a href="查询内网Zone列表.md">查询内网Zone列表</a>获取。</p>
</td>
</tr>
<tr id="row49313939"><td class="cellrowborder" valign="top" width="19.878012198780123%" headers="mcps1.2.5.1.1 "><p id="p35006119"><a name="p35006119"></a><a name="p35006119"></a>recordset_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.748725127487251%" headers="mcps1.2.5.1.2 "><p id="p16923420"><a name="p16923420"></a><a name="p16923420"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.80871912808719%" headers="mcps1.2.5.1.3 "><p id="p3406204715472"><a name="p3406204715472"></a><a name="p3406204715472"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.56454354564543%" headers="mcps1.2.5.1.4 "><p id="p28619802"><a name="p28619802"></a><a name="p28619802"></a>待删除recordset的ID。</p>
<p id="p12406443193011"><a name="p12406443193011"></a><a name="p12406443193011"></a>可以通过<a href="查询单个Zone下Record-Set列表.md">查询单个Zone下Record Set列表</a>获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section36482533"></a>

-   请求参数

    无

-   请求样例

    删除域名的记录集，域名的Zone ID为“2c9eb155587194ec01587224c9f90149”，Recordset ID为“2c9eb155587228570158722b6ac30007”。

    ```
    DELETE https://{DNS_Endpoint}/v2/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587228570158722b6ac30007
    ```


## 响应<a name="section59907344"></a>

-   参数说明

    **表 2**  响应样例的参数说明

    <a name="table2027435217127"></a>
    <table><thead align="left"><tr id="rf63e3f73474e4c278a069c18f2cbda2e"><th class="cellrowborder" valign="top" width="18.33%" id="mcps1.2.4.1.1"><p id="a6ef51227cb264b32bebfc986d3e637d9"><a name="a6ef51227cb264b32bebfc986d3e637d9"></a><a name="a6ef51227cb264b32bebfc986d3e637d9"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.259999999999998%" id="mcps1.2.4.1.2"><p id="ae4f0a65aa76a4fb1957074bb69d5dbdd"><a name="ae4f0a65aa76a4fb1957074bb69d5dbdd"></a><a name="ae4f0a65aa76a4fb1957074bb69d5dbdd"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.41%" id="mcps1.2.4.1.3"><p id="a47bf2f8c9f504cc9bee2e5ec1257eb3f"><a name="a47bf2f8c9f504cc9bee2e5ec1257eb3f"></a><a name="a47bf2f8c9f504cc9bee2e5ec1257eb3f"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="rc4ac2a5267624f239ad9b1cd01768435"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="aed4e16cb934a49af80a35a677f91d92e"><a name="aed4e16cb934a49af80a35a677f91d92e"></a><a name="aed4e16cb934a49af80a35a677f91d92e"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="a5fe96ba32d0f47149f32f3ea7d4f05e6"><a name="a5fe96ba32d0f47149f32f3ea7d4f05e6"></a><a name="a5fe96ba32d0f47149f32f3ea7d4f05e6"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.41%" headers="mcps1.2.4.1.3 "><p id="a0b0a5c0cd1f24b55a29ecdb6066b3705"><a name="a0b0a5c0cd1f24b55a29ecdb6066b3705"></a><a name="a0b0a5c0cd1f24b55a29ecdb6066b3705"></a>Record Set的ID。</p>
    </td>
    </tr>
    <tr id="ra9e885d12b4d43428831752336a0d4c0"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a32fb714b039b4a978222179f61a0f076"><a name="a32fb714b039b4a978222179f61a0f076"></a><a name="a32fb714b039b4a978222179f61a0f076"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="a83b8bc6a22eb48f087f3b842f1a177be"><a name="a83b8bc6a22eb48f087f3b842f1a177be"></a><a name="a83b8bc6a22eb48f087f3b842f1a177be"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.41%" headers="mcps1.2.4.1.3 "><p id="a3a0582b25e7f4c9c9028a0a082553e63"><a name="a3a0582b25e7f4c9c9028a0a082553e63"></a><a name="a3a0582b25e7f4c9c9028a0a082553e63"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="r8a5cb7251c6e4ad2aac8e92c1fc1c825"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a2ba0b3a7490e4f8c9f2d001abc31b5fc"><a name="a2ba0b3a7490e4f8c9f2d001abc31b5fc"></a><a name="a2ba0b3a7490e4f8c9f2d001abc31b5fc"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="a590b27e6f7304033beb416c2615febf4"><a name="a590b27e6f7304033beb416c2615febf4"></a><a name="a590b27e6f7304033beb416c2615febf4"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.41%" headers="mcps1.2.4.1.3 "><p id="a6566187b31744bdfbfd273d05ada45cc"><a name="a6566187b31744bdfbfd273d05ada45cc"></a><a name="a6566187b31744bdfbfd273d05ada45cc"></a>Record Set的描述信息。</p>
    </td>
    </tr>
    <tr id="r6ff9dc233cc64b6eb856a2f2d4ecdfea"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="adb2e4a3dc5264bd194c9fdbb52d738f0"><a name="adb2e4a3dc5264bd194c9fdbb52d738f0"></a><a name="adb2e4a3dc5264bd194c9fdbb52d738f0"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="a9a32df9951ea4e63a36979ffe7839125"><a name="a9a32df9951ea4e63a36979ffe7839125"></a><a name="a9a32df9951ea4e63a36979ffe7839125"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.41%" headers="mcps1.2.4.1.3 "><p id="a69a040838e314d9992462ec5cb23db6f"><a name="a69a040838e314d9992462ec5cb23db6f"></a><a name="a69a040838e314d9992462ec5cb23db6f"></a>托管该记录的zone_id。</p>
    </td>
    </tr>
    <tr id="r82492d1a4b134373ba3e3fb657f19346"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="ade468dd7e4d24dc2bc83795202c2e618"><a name="ade468dd7e4d24dc2bc83795202c2e618"></a><a name="ade468dd7e4d24dc2bc83795202c2e618"></a>zone_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="ae9bad680780945638499d66748a089ee"><a name="ae9bad680780945638499d66748a089ee"></a><a name="ae9bad680780945638499d66748a089ee"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.41%" headers="mcps1.2.4.1.3 "><p id="af6bb9568887946fd83f837a9f67c9d35"><a name="af6bb9568887946fd83f837a9f67c9d35"></a><a name="af6bb9568887946fd83f837a9f67c9d35"></a>托管该记录的zone_name。</p>
    </td>
    </tr>
    <tr id="r58a2d0249a9d46608dceb58752487962"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a6812a6c96d0b4f08ad96cd4aa92c29ef"><a name="a6812a6c96d0b4f08ad96cd4aa92c29ef"></a><a name="a6812a6c96d0b4f08ad96cd4aa92c29ef"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="a0cacd81f8e7247ed9b3e4b4a0d5a1c1a"><a name="a0cacd81f8e7247ed9b3e4b4a0d5a1c1a"></a><a name="a0cacd81f8e7247ed9b3e4b4a0d5a1c1a"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.41%" headers="mcps1.2.4.1.3 "><p id="a3db4aa6f5f604faeb111cc5b98a05bf9"><a name="a3db4aa6f5f604faeb111cc5b98a05bf9"></a><a name="a3db4aa6f5f604faeb111cc5b98a05bf9"></a>记录类型。</p>
    <p id="p20817123416132"><a name="p20817123416132"></a><a name="p20817123416132"></a>取值范围：A、AAAA、MX、CNAME、TXT、NS（仅限公网Zone）、SRV、PTR（仅限内网Zone）、CAA（仅限公网Zone）。</p>
    <p id="zh-cn_topic_0037134404_p15442435577"><a name="zh-cn_topic_0037134404_p15442435577"></a><a name="zh-cn_topic_0037134404_p15442435577"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a>。</p>
    </td>
    </tr>
    <tr id="r06be1132e6b544eaac47c6b6cae4af1d"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="abe5c52a6e2154f6391976aa80857198f"><a name="abe5c52a6e2154f6391976aa80857198f"></a><a name="abe5c52a6e2154f6391976aa80857198f"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="a57fe1965995b4f99a67c1c84d927f3b6"><a name="a57fe1965995b4f99a67c1c84d927f3b6"></a><a name="a57fe1965995b4f99a67c1c84d927f3b6"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.41%" headers="mcps1.2.4.1.3 "><p id="p123031523174010"><a name="p123031523174010"></a><a name="p123031523174010"></a>解析记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="p1030317233408"><a name="p1030317233408"></a><a name="p1030317233408"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    </td>
    </tr>
    <tr id="r8cb1518cb4b84bf0b8115a7f4a8835c4"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="ae57bbd14742845c2aced32f030bc6a80"><a name="ae57bbd14742845c2aced32f030bc6a80"></a><a name="ae57bbd14742845c2aced32f030bc6a80"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="a5a480487a4fc42fa987d5ba2c6d920b9"><a name="a5a480487a4fc42fa987d5ba2c6d920b9"></a><a name="a5a480487a4fc42fa987d5ba2c6d920b9"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.41%" headers="mcps1.2.4.1.3 "><p id="a7ff6973b19f84ee5aa83b0967e0c2434"><a name="a7ff6973b19f84ee5aa83b0967e0c2434"></a><a name="a7ff6973b19f84ee5aa83b0967e0c2434"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="r93b32291d1e64da39452a8997fcda248"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a9bc903f33fd54c9aa3b1f9d07ed6a31a"><a name="a9bc903f33fd54c9aa3b1f9d07ed6a31a"></a><a name="a9bc903f33fd54c9aa3b1f9d07ed6a31a"></a>create_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="a55f1491f864c456eae0b254526eaf1f8"><a name="a55f1491f864c456eae0b254526eaf1f8"></a><a name="a55f1491f864c456eae0b254526eaf1f8"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.41%" headers="mcps1.2.4.1.3 "><p id="ab802d00a14d74a5abe323755a0c1a9c3"><a name="ab802d00a14d74a5abe323755a0c1a9c3"></a><a name="ab802d00a14d74a5abe323755a0c1a9c3"></a>创建时间。</p>
    <p id="zh-cn_topic_0037134404_p91253279589"><a name="zh-cn_topic_0037134404_p91253279589"></a><a name="zh-cn_topic_0037134404_p91253279589"></a>格式：yyyy-MM-dd'T'HH:mm:ss.SSS</p>
    </td>
    </tr>
    <tr id="rececad4599034fec9010552d92c3b3d1"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="ae3d53158cf0e4b0c81f9aeafbbf377a2"><a name="ae3d53158cf0e4b0c81f9aeafbbf377a2"></a><a name="ae3d53158cf0e4b0c81f9aeafbbf377a2"></a>update_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="a1b01ca3627dc49c986c67d231de5c85f"><a name="a1b01ca3627dc49c986c67d231de5c85f"></a><a name="a1b01ca3627dc49c986c67d231de5c85f"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.41%" headers="mcps1.2.4.1.3 "><p id="acbcc47bca305436b8fb99d10b0de8765"><a name="acbcc47bca305436b8fb99d10b0de8765"></a><a name="acbcc47bca305436b8fb99d10b0de8765"></a>更新时间。</p>
    <p id="ab3462c7056cd417e81ff267a3ea46443"><a name="ab3462c7056cd417e81ff267a3ea46443"></a><a name="ab3462c7056cd417e81ff267a3ea46443"></a>格式：yyyy-MM-dd'T'HH:mm:ss.SSS</p>
    </td>
    </tr>
    <tr id="r18fd03e795cb427a953b0efb798cdc64"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="afe9aea31aae443be91d0a1ea8db8806d"><a name="afe9aea31aae443be91d0a1ea8db8806d"></a><a name="afe9aea31aae443be91d0a1ea8db8806d"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="a7f0d877c3b134d3bbaaa813571ef16fb"><a name="a7f0d877c3b134d3bbaaa813571ef16fb"></a><a name="a7f0d877c3b134d3bbaaa813571ef16fb"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.41%" headers="mcps1.2.4.1.3 "><p id="a9a68c20d53b843ed98875ccfce9781f4"><a name="a9a68c20d53b843ed98875ccfce9781f4"></a><a name="a9a68c20d53b843ed98875ccfce9781f4"></a>资源状态。</p>
    <p id="a6083e4f4301a476da8c39b9587e46bb9"><a name="a6083e4f4301a476da8c39b9587e46bb9"></a><a name="a6083e4f4301a476da8c39b9587e46bb9"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="rf566452075b04b41ac618d76387832ab"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="aad28018162974cd3ab00f6e7b50a0d40"><a name="aad28018162974cd3ab00f6e7b50a0d40"></a><a name="aad28018162974cd3ab00f6e7b50a0d40"></a>default</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="a4d66625c999244ffa5a6dcfa967cc6d2"><a name="a4d66625c999244ffa5a6dcfa967cc6d2"></a><a name="a4d66625c999244ffa5a6dcfa967cc6d2"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.41%" headers="mcps1.2.4.1.3 "><p id="aa87419f5ec904492968127f0424e88dd"><a name="aa87419f5ec904492968127f0424e88dd"></a><a name="aa87419f5ec904492968127f0424e88dd"></a>标识是否由系统默认生成，系统默认生成的Record Set不能删除。</p>
    </td>
    </tr>
    <tr id="r327b7fd09445440cb72ab3cd7fd54f76"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a4b770fd18dd948aea76499724a625eca"><a name="a4b770fd18dd948aea76499724a625eca"></a><a name="a4b770fd18dd948aea76499724a625eca"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="a319fefa4c28b48ee9c5918b78a8746d8"><a name="a319fefa4c28b48ee9c5918b78a8746d8"></a><a name="a319fefa4c28b48ee9c5918b78a8746d8"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.41%" headers="mcps1.2.4.1.3 "><p id="p4619625201026"><a name="p4619625201026"></a><a name="p4619625201026"></a>该Record Set所属的项目ID。</p>
    </td>
    </tr>
    <tr id="r63b97c55056a4b32a3895d2af40c74a0"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a94878242f50449aaae37b65105b3d867"><a name="a94878242f50449aaae37b65105b3d867"></a><a name="a94878242f50449aaae37b65105b3d867"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="af62c9f365b1f4d9b8743da27e6085818"><a name="af62c9f365b1f4d9b8743da27e6085818"></a><a name="af62c9f365b1f4d9b8743da27e6085818"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.41%" headers="mcps1.2.4.1.3 "><p id="ad757db1edea54d3cacac51db1def8abf"><a name="ad757db1edea54d3cacac51db1def8abf"></a><a name="ad757db1edea54d3cacac51db1def8abf"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p4390201110479"><a name="p4390201110479"></a><a name="p4390201110479"></a>详细信息请参见<a href="#table354521744216">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  links参数说明

    <a name="table354521744216"></a>
    <table><thead align="left"><tr id="row954518179427"><th class="cellrowborder" valign="top" width="18.3018301830183%" id="mcps1.2.4.1.1"><p id="p654513173424"><a name="p654513173424"></a><a name="p654513173424"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.591959195919593%" id="mcps1.2.4.1.2"><p id="p654551714212"><a name="p654551714212"></a><a name="p654551714212"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.10621062106211%" id="mcps1.2.4.1.3"><p id="p1545141717427"><a name="p1545141717427"></a><a name="p1545141717427"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3545101710429"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p115467171428"><a name="p115467171428"></a><a name="p115467171428"></a>self</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.591959195919593%" headers="mcps1.2.4.1.2 "><p id="p254611713427"><a name="p254611713427"></a><a name="p254611713427"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.10621062106211%" headers="mcps1.2.4.1.3 "><p id="p5546171744214"><a name="p5546171744214"></a><a name="p5546171744214"></a>当前资源的链接。</p>
    </td>
    </tr>
    <tr id="row1118615044919"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.591959195919593%" headers="mcps1.2.4.1.2 "><p id="p19656144517367"><a name="p19656144517367"></a><a name="p19656144517367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.10621062106211%" headers="mcps1.2.4.1.3 "><p id="p76567451365"><a name="p76567451365"></a><a name="p76567451365"></a>下一页资源的链接。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "id": "2c9eb155587228570158722b6ac30007",
        "name": "www.example.com.",
        "description": "This is an example record set.",
        "type": "A",
        "ttl": 300,
        "status": "PENDING_DELETE",
        "links": {
            "self": "https://Endpoint/v2/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587228570158722b6ac30007"
        },
        "zone_id": "2c9eb155587194ec01587224c9f90149",
        "zone_name": "example.com.",
        "create_at": "2016-11-17T12:03:17.827",
        "update_at": "2016-11-17T12:56:03.827",
        "default": false,
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c"
    }
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

