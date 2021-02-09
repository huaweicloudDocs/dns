# 删除Record Set<a name="dns_api_65005"></a>

## 功能介绍<a name="section49332166"></a>

删除单个Record Set。

## URI<a name="section41336317"></a>

DELETE /v2.1/zones/\{zone\_id\}/recordsets/\{[recordset\_id](查询单个Zone下Record-Set列表-多线路.md)\}

参数说明请参见[表1](#table52104579)。

**表 1**  URI格式的参数说明

<a name="table52104579"></a>
<table><thead align="left"><tr id="row50570707"><th class="cellrowborder" valign="top" width="21.08%" id="mcps1.2.5.1.1"><p id="p2586631"><a name="p2586631"></a><a name="p2586631"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.9%" id="mcps1.2.5.1.2"><p id="p8190559"><a name="p8190559"></a><a name="p8190559"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.99%" id="mcps1.2.5.1.3"><p id="p8722175318367"><a name="p8722175318367"></a><a name="p8722175318367"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="43.03%" id="mcps1.2.5.1.4"><p id="p59455556"><a name="p59455556"></a><a name="p59455556"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row51170717"><td class="cellrowborder" valign="top" width="21.08%" headers="mcps1.2.5.1.1 "><p id="p51187411"><a name="p51187411"></a><a name="p51187411"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.9%" headers="mcps1.2.5.1.2 "><p id="p52539597"><a name="p52539597"></a><a name="p52539597"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.99%" headers="mcps1.2.5.1.3 "><p id="p6722853133612"><a name="p6722853133612"></a><a name="p6722853133612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.03%" headers="mcps1.2.5.1.4 "><p id="p27848947"><a name="p27848947"></a><a name="p27848947"></a>所属zone的ID。仅支持公网zone。</p>
<p id="p22777371252"><a name="p22777371252"></a><a name="p22777371252"></a>可以通过<a href="查询公网Zone列表.md">查询公网Zone列表</a>获取。</p>
</td>
</tr>
<tr id="row49313939"><td class="cellrowborder" valign="top" width="21.08%" headers="mcps1.2.5.1.1 "><p id="p35006119"><a name="p35006119"></a><a name="p35006119"></a>recordset_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.9%" headers="mcps1.2.5.1.2 "><p id="p16923420"><a name="p16923420"></a><a name="p16923420"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.99%" headers="mcps1.2.5.1.3 "><p id="p1722953103615"><a name="p1722953103615"></a><a name="p1722953103615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.03%" headers="mcps1.2.5.1.4 "><p id="p28619802"><a name="p28619802"></a><a name="p28619802"></a>待删除recordset的ID。</p>
<p id="p12406443193011"><a name="p12406443193011"></a><a name="p12406443193011"></a>可以通过<a href="查询单个Zone下Record-Set列表-多线路.md">查询单个Zone下Record Set列表</a>获取。</p>
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
    DELETE https://{DNS_Endpoint}/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587228570158722b6ac30007
    ```


## 响应<a name="section59907344"></a>

-   参数说明

    **表 2**  响应样例的参数说明

    <a name="table2027435217127"></a>
    <table><thead align="left"><tr id="re9569d6bd3c94391ae8636078bb03d72"><th class="cellrowborder" valign="top" width="18.33%" id="mcps1.2.4.1.1"><p id="abdca8cb5f51e4c76af147dd1dd053757"><a name="abdca8cb5f51e4c76af147dd1dd053757"></a><a name="abdca8cb5f51e4c76af147dd1dd053757"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.37%" id="mcps1.2.4.1.2"><p id="a39d155916b5a45b28f5ec9ed241685d4"><a name="a39d155916b5a45b28f5ec9ed241685d4"></a><a name="a39d155916b5a45b28f5ec9ed241685d4"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.3%" id="mcps1.2.4.1.3"><p id="ae80695cc1dc24a79a05b8fe31d1f0174"><a name="ae80695cc1dc24a79a05b8fe31d1f0174"></a><a name="ae80695cc1dc24a79a05b8fe31d1f0174"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r52c11fefcc8b418f8b2401a5be373f47"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="aefb75f3287d14ed9816398e0c20c01d0"><a name="aefb75f3287d14ed9816398e0c20c01d0"></a><a name="aefb75f3287d14ed9816398e0c20c01d0"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="ab1b0000b053a47a7a7b688f252128dc7"><a name="ab1b0000b053a47a7a7b688f252128dc7"></a><a name="ab1b0000b053a47a7a7b688f252128dc7"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="adff6526e6958471c8de31afb69d94398"><a name="adff6526e6958471c8de31afb69d94398"></a><a name="adff6526e6958471c8de31afb69d94398"></a>Record Set的ID。</p>
    </td>
    </tr>
    <tr id="rfee7fb943e7e4109a67c6ee970603414"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a0acf617e67ec4b3fa51536e2cab144e4"><a name="a0acf617e67ec4b3fa51536e2cab144e4"></a><a name="a0acf617e67ec4b3fa51536e2cab144e4"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="a092529af9b0b48bbb6ea7197333b26f0"><a name="a092529af9b0b48bbb6ea7197333b26f0"></a><a name="a092529af9b0b48bbb6ea7197333b26f0"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="a9d7f89294ce648ba9d4a0a32b197db47"><a name="a9d7f89294ce648ba9d4a0a32b197db47"></a><a name="a9d7f89294ce648ba9d4a0a32b197db47"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="r730f7b102d57470e980aa85bdad88cd6"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="aac2dce43d5004d3187a8095bd1a6fa47"><a name="aac2dce43d5004d3187a8095bd1a6fa47"></a><a name="aac2dce43d5004d3187a8095bd1a6fa47"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="a043dfd5056e143c7a7871520a8698bf3"><a name="a043dfd5056e143c7a7871520a8698bf3"></a><a name="a043dfd5056e143c7a7871520a8698bf3"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="a0e240743eb3f4e56ac4bd78d04af1b9c"><a name="a0e240743eb3f4e56ac4bd78d04af1b9c"></a><a name="a0e240743eb3f4e56ac4bd78d04af1b9c"></a>Record Set的描述信息。</p>
    </td>
    </tr>
    <tr id="r2b7289ca61764982b20006247e9aeca1"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="aca2c7ed052c24b87a36c938e54f01926"><a name="aca2c7ed052c24b87a36c938e54f01926"></a><a name="aca2c7ed052c24b87a36c938e54f01926"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="a75ed3102fab64b2285b6693d491bdf9b"><a name="a75ed3102fab64b2285b6693d491bdf9b"></a><a name="a75ed3102fab64b2285b6693d491bdf9b"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="a8e14c2a97f214f1cbc53f78c62618c6e"><a name="a8e14c2a97f214f1cbc53f78c62618c6e"></a><a name="a8e14c2a97f214f1cbc53f78c62618c6e"></a>托管该记录的zone_id。</p>
    </td>
    </tr>
    <tr id="r0a009e6721794701a3e523d287e9dd68"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="aa6f0328240684adeae2f4cd66424e552"><a name="aa6f0328240684adeae2f4cd66424e552"></a><a name="aa6f0328240684adeae2f4cd66424e552"></a>zone_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="ac5f694c92bde4749b8d02639479df1a7"><a name="ac5f694c92bde4749b8d02639479df1a7"></a><a name="ac5f694c92bde4749b8d02639479df1a7"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="af1716885723746bcab351c966872cdfd"><a name="af1716885723746bcab351c966872cdfd"></a><a name="af1716885723746bcab351c966872cdfd"></a>托管该记录的zone_name。</p>
    </td>
    </tr>
    <tr id="r148eb821bc8d4dc18a1f830cff6b81a5"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a8b7d7e6e3c754cafa0620ee0418e07bd"><a name="a8b7d7e6e3c754cafa0620ee0418e07bd"></a><a name="a8b7d7e6e3c754cafa0620ee0418e07bd"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="a198878893476468d88aa399ef4524f20"><a name="a198878893476468d88aa399ef4524f20"></a><a name="a198878893476468d88aa399ef4524f20"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="a40f7e2d49d9b43d1b3f1b28979f68a37"><a name="a40f7e2d49d9b43d1b3f1b28979f68a37"></a><a name="a40f7e2d49d9b43d1b3f1b28979f68a37"></a>记录类型。</p>
    <p id="a0f6083cba776472db7d497b91d7815d9"><a name="a0f6083cba776472db7d497b91d7815d9"></a><a name="a0f6083cba776472db7d497b91d7815d9"></a>取值范围：A、AAAA、MX、CNAME、TXT、NS、SRV、CAA。</p>
    <p id="zh-cn_topic_0082840627_p104661629809"><a name="zh-cn_topic_0082840627_p104661629809"></a><a name="zh-cn_topic_0082840627_p104661629809"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a>。</p>
    </td>
    </tr>
    <tr id="rd44126ec17414d15905fd59ab185b903"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a40575ddb25dd4c90a26cea4dcb2886a4"><a name="a40575ddb25dd4c90a26cea4dcb2886a4"></a><a name="a40575ddb25dd4c90a26cea4dcb2886a4"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="aea9d2e55fa674d35b1a2e957ab2a85d0"><a name="aea9d2e55fa674d35b1a2e957ab2a85d0"></a><a name="aea9d2e55fa674d35b1a2e957ab2a85d0"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="p123031523174010"><a name="p123031523174010"></a><a name="p123031523174010"></a>解析记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="p1030317233408"><a name="p1030317233408"></a><a name="p1030317233408"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    </td>
    </tr>
    <tr id="rc5c80bec7ff44031b3b1ad2acb0bd696"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="ac61189b5595941129e1a76e35f53bdbe"><a name="ac61189b5595941129e1a76e35f53bdbe"></a><a name="ac61189b5595941129e1a76e35f53bdbe"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="a9b3a92ea9a25418b88eac6917053c731"><a name="a9b3a92ea9a25418b88eac6917053c731"></a><a name="a9b3a92ea9a25418b88eac6917053c731"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="a0b83498fe0ed4d8bbe1e89016dae24c7"><a name="a0b83498fe0ed4d8bbe1e89016dae24c7"></a><a name="a0b83498fe0ed4d8bbe1e89016dae24c7"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="re69035799358465b94ff7c5900edeae0"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a4c335b4ca946487191fdc4cee7ea2cbe"><a name="a4c335b4ca946487191fdc4cee7ea2cbe"></a><a name="a4c335b4ca946487191fdc4cee7ea2cbe"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="a860aed6b7be54ec7ad47b1fc487a061d"><a name="a860aed6b7be54ec7ad47b1fc487a061d"></a><a name="a860aed6b7be54ec7ad47b1fc487a061d"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="ae3e6f6253abf4e8eb2202a2d732fe0e8"><a name="ae3e6f6253abf4e8eb2202a2d732fe0e8"></a><a name="ae3e6f6253abf4e8eb2202a2d732fe0e8"></a>创建时间。</p>
    <p id="p583516468316"><a name="p583516468316"></a><a name="p583516468316"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="r8d6e079ee64646e19fd40cb09cc58c1a"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="abf5c553a9661491f80686bb570b8845c"><a name="abf5c553a9661491f80686bb570b8845c"></a><a name="abf5c553a9661491f80686bb570b8845c"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="a41393e6cd8824b93b8f29817bbee026c"><a name="a41393e6cd8824b93b8f29817bbee026c"></a><a name="a41393e6cd8824b93b8f29817bbee026c"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="a2e7334dac7bd4137ae76361077a03294"><a name="a2e7334dac7bd4137ae76361077a03294"></a><a name="a2e7334dac7bd4137ae76361077a03294"></a>更新时间。</p>
    <p id="p1481431019435"><a name="p1481431019435"></a><a name="p1481431019435"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="rb8b797c6c8fd48a58590a0191b0b0fc3"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a0686f98f196f403c8f1c311ca44e0367"><a name="a0686f98f196f403c8f1c311ca44e0367"></a><a name="a0686f98f196f403c8f1c311ca44e0367"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="ae61ede6973114eafbc416d9b39c4baf9"><a name="ae61ede6973114eafbc416d9b39c4baf9"></a><a name="ae61ede6973114eafbc416d9b39c4baf9"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="a0bb61e8808d54706a5d5e2476cebd5d3"><a name="a0bb61e8808d54706a5d5e2476cebd5d3"></a><a name="a0bb61e8808d54706a5d5e2476cebd5d3"></a>资源状态。</p>
    <p id="a8c868a035f6b40b28e38a04759c1e2da"><a name="a8c868a035f6b40b28e38a04759c1e2da"></a><a name="a8c868a035f6b40b28e38a04759c1e2da"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="r06426d7d9c31484980fc6ef26d187a98"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a18eee0f064e149988ffcf1eb6866fa5d"><a name="a18eee0f064e149988ffcf1eb6866fa5d"></a><a name="a18eee0f064e149988ffcf1eb6866fa5d"></a>default</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="ac5ccf10595b04b64b648b2962b325831"><a name="ac5ccf10595b04b64b648b2962b325831"></a><a name="ac5ccf10595b04b64b648b2962b325831"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="ad656bb96bf0044d8ae836bfdf215012a"><a name="ad656bb96bf0044d8ae836bfdf215012a"></a><a name="ad656bb96bf0044d8ae836bfdf215012a"></a>标识是否由系统默认生成，系统默认生成的Record Set不能删除。</p>
    </td>
    </tr>
    <tr id="rda385837da8444e9a3cbb6a694631e52"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="ab54bcb44f53b4917b4939048043cdbd8"><a name="ab54bcb44f53b4917b4939048043cdbd8"></a><a name="ab54bcb44f53b4917b4939048043cdbd8"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="a2078468763ff4b0bbc3d09b54b525b1a"><a name="a2078468763ff4b0bbc3d09b54b525b1a"></a><a name="a2078468763ff4b0bbc3d09b54b525b1a"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="p4619625201026"><a name="p4619625201026"></a><a name="p4619625201026"></a>该Record Set所属的项目ID。</p>
    </td>
    </tr>
    <tr id="r3b1c5b92ffcf44bfb20356a8285771a3"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a96b57b88bc5b4333a0887ecf8b6aa4f1"><a name="a96b57b88bc5b4333a0887ecf8b6aa4f1"></a><a name="a96b57b88bc5b4333a0887ecf8b6aa4f1"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="a023c6a235bea4726ad4afd77648d5918"><a name="a023c6a235bea4726ad4afd77648d5918"></a><a name="a023c6a235bea4726ad4afd77648d5918"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="a41f3f8b60b9d4d89a1c10106ecbad1f0"><a name="a41f3f8b60b9d4d89a1c10106ecbad1f0"></a><a name="a41f3f8b60b9d4d89a1c10106ecbad1f0"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。详细信息请参见<a href="#table354521744216">表3</a>。</p>
    </td>
    </tr>
    <tr id="r3a791979a4974855bc1a98378abf59f6"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a85068a27fcb548d29dbc166873d72aaf"><a name="a85068a27fcb548d29dbc166873d72aaf"></a><a name="a85068a27fcb548d29dbc166873d72aaf"></a>line</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="aefea73252e5d48979c29c4607f26189f"><a name="aefea73252e5d48979c29c4607f26189f"></a><a name="aefea73252e5d48979c29c4607f26189f"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="ac347aecebea840d097bba040fd2557da"><a name="ac347aecebea840d097bba040fd2557da"></a><a name="ac347aecebea840d097bba040fd2557da"></a>解析线路ID。</p>
    </td>
    </tr>
    <tr id="re879d4dcf1c947fea7bb6770cd2b8037"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="ae9e51544b5be4018844c2495a23a4f54"><a name="ae9e51544b5be4018844c2495a23a4f54"></a><a name="ae9e51544b5be4018844c2495a23a4f54"></a>weight</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="a7c17010a66834133b2ebdba0f686c2cd"><a name="a7c17010a66834133b2ebdba0f686c2cd"></a><a name="a7c17010a66834133b2ebdba0f686c2cd"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="a5d82f0174b164a7ca35df9ed74515537"><a name="a5d82f0174b164a7ca35df9ed74515537"></a><a name="a5d82f0174b164a7ca35df9ed74515537"></a>解析记录的权重。</p>
    </td>
    </tr>
    <tr id="rbb5a78b17b6c4779a578b7e09ddbb27f"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a67e2682178f241719c53f40b3d46de0f"><a name="a67e2682178f241719c53f40b3d46de0f"></a><a name="a67e2682178f241719c53f40b3d46de0f"></a>health_check_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="ab1547ca95b4f4672a5e1726a3d0e2ded"><a name="ab1547ca95b4f4672a5e1726a3d0e2ded"></a><a name="ab1547ca95b4f4672a5e1726a3d0e2ded"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="a83f9eb4d10ab47f5983bfdf7cb3f4e35"><a name="a83f9eb4d10ab47f5983bfdf7cb3f4e35"></a><a name="a83f9eb4d10ab47f5983bfdf7cb3f4e35"></a>健康检查ID。</p>
    </td>
    </tr>
    <tr id="r1bc7a88aaf594528bd444ebb84fca36d"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="aa28212a0f23d439f87603f35dd112cce"><a name="aa28212a0f23d439f87603f35dd112cce"></a><a name="aa28212a0f23d439f87603f35dd112cce"></a>alias_target</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.37%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p477512344313"><a name="zh-cn_topic_0082840627_p477512344313"></a><a name="zh-cn_topic_0082840627_p477512344313"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.3%" headers="mcps1.2.4.1.3 "><p id="abe651c805e8e47d0b3a371ae336baddd"><a name="abe651c805e8e47d0b3a371ae336baddd"></a><a name="abe651c805e8e47d0b3a371ae336baddd"></a>别名记录。详细信息请参见<a href="数据结构.md#table11888161342410">表4</a>。</p>
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
    <tr id="row1050420481507"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
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
            "self": "https://Endpoint/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587228570158722b6ac30007"
        },
        "alias_target": null,
        "zone_id": "2c9eb155587194ec01587224c9f90149",
        "zone_name": "example.com.",
        "created_at": "2016-11-17T12:03:17.827",
        "updated_at": "2016-11-17T12:56:06.439",
        "default": false,
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
        "line": "default_view",
        "weight": 1,
        "health_check_id":null
    }
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

