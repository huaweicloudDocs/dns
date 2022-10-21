# 修改内网Zone<a name="dns_api_63009"></a>

## 功能介绍<a name="section3569153217343"></a>

修改单个Zone。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=DNS&api=UpdatePrivateZone)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI<a name="section6163262617350"></a>

PATCH /v2/zones/\{zone\_id\}

参数说明请参见[表1](#tacd282d91a914e70a7e35f44180b61aa)。

**表 1**  URI格式的参数说明

<a name="tacd282d91a914e70a7e35f44180b61aa"></a>
<table><thead align="left"><tr id="r461951832c9c4a788d3a29813fd6006d"><th class="cellrowborder" valign="top" width="15.459999999999999%" id="mcps1.2.5.1.1"><p id="acf0cac48978e4f96b71afbec7f79576e"><a name="acf0cac48978e4f96b71afbec7f79576e"></a><a name="acf0cac48978e4f96b71afbec7f79576e"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.459999999999999%" id="mcps1.2.5.1.2"><p id="ac42fd57c878140d7b0459137e8babd55"><a name="ac42fd57c878140d7b0459137e8babd55"></a><a name="ac42fd57c878140d7b0459137e8babd55"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.53%" id="mcps1.2.5.1.3"><p id="aabaec6aa7c8443d59fa706845ff1d28b"><a name="aabaec6aa7c8443d59fa706845ff1d28b"></a><a name="aabaec6aa7c8443d59fa706845ff1d28b"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.55%" id="mcps1.2.5.1.4"><p id="ae870f28af9f7424185040e4540001949"><a name="ae870f28af9f7424185040e4540001949"></a><a name="ae870f28af9f7424185040e4540001949"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="r458847e9fb5647bf9d773276361fe788"><td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.5.1.1 "><p id="ab6bccc4405ed4594930f55ae38209450"><a name="ab6bccc4405ed4594930f55ae38209450"></a><a name="ab6bccc4405ed4594930f55ae38209450"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.5.1.2 "><p id="a2d45a5f16c804754aa263637564eec4c"><a name="a2d45a5f16c804754aa263637564eec4c"></a><a name="a2d45a5f16c804754aa263637564eec4c"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.2.5.1.3 "><p id="a10129d8fbda642759f1eb05715b5b5bc"><a name="a10129d8fbda642759f1eb05715b5b5bc"></a><a name="a10129d8fbda642759f1eb05715b5b5bc"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.55%" headers="mcps1.2.5.1.4 "><p id="ae6c59bfcf6a341dd9d9d8b7908c7db8a"><a name="ae6c59bfcf6a341dd9d9d8b7908c7db8a"></a><a name="ae6c59bfcf6a341dd9d9d8b7908c7db8a"></a>待修改zone的ID。</p>
<p id="p1669018482183"><a name="p1669018482183"></a><a name="p1669018482183"></a>可以通过<a href="查询内网Zone列表.md">查询内网Zone列表</a>获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section4207148117353"></a>

-   参数说明

    **表 2**  请求样例的参数说明

    <a name="tc108ce509e2d411fa6cfb6f193f37133"></a>
    <table><thead align="left"><tr id="r139885ec379f4f19b8d830dd368d368e"><th class="cellrowborder" valign="top" width="14.52%" id="mcps1.2.5.1.1"><p id="adcd0fcfe879d404ca45d675c00467a67"><a name="adcd0fcfe879d404ca45d675c00467a67"></a><a name="adcd0fcfe879d404ca45d675c00467a67"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.55%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0080995382_p473035017742"><a name="zh-cn_topic_0080995382_p473035017742"></a><a name="zh-cn_topic_0080995382_p473035017742"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.33%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0080995382_p386753717742"><a name="zh-cn_topic_0080995382_p386753717742"></a><a name="zh-cn_topic_0080995382_p386753717742"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.6%" id="mcps1.2.5.1.4"><p id="af771f63bb344447ca66df90f12e29e47"><a name="af771f63bb344447ca66df90f12e29e47"></a><a name="af771f63bb344447ca66df90f12e29e47"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r79d4ffb128df44eea2fe028e9ee95caf"><td class="cellrowborder" valign="top" width="14.52%" headers="mcps1.2.5.1.1 "><p id="a09232732617f4165b17554a4a672d0b8"><a name="a09232732617f4165b17554a4a672d0b8"></a><a name="a09232732617f4165b17554a4a672d0b8"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0080995382_p759162017742"><a name="zh-cn_topic_0080995382_p759162017742"></a><a name="zh-cn_topic_0080995382_p759162017742"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.5.1.3 "><p id="afc615a782a7c4f438473ad20495eaff1"><a name="afc615a782a7c4f438473ad20495eaff1"></a><a name="afc615a782a7c4f438473ad20495eaff1"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.6%" headers="mcps1.2.5.1.4 "><p id="a55e92ec653404fe69560006cf9dc32f0"><a name="a55e92ec653404fe69560006cf9dc32f0"></a><a name="a55e92ec653404fe69560006cf9dc32f0"></a>域名的描述信息。长度不超过255个字符。</p>
    <p id="zh-cn_topic_0080995382_p37540522006"><a name="zh-cn_topic_0080995382_p37540522006"></a><a name="zh-cn_topic_0080995382_p37540522006"></a>如果为空，表示维持原值。</p>
    <p id="zh-cn_topic_0080995382_p474692155919"><a name="zh-cn_topic_0080995382_p474692155919"></a><a name="zh-cn_topic_0080995382_p474692155919"></a>默认值为空。</p>
    </td>
    </tr>
    <tr id="rc1f8751e7f854985901c5de652daa580"><td class="cellrowborder" valign="top" width="14.52%" headers="mcps1.2.5.1.1 "><p id="afab6fc762eb743c29c1cb7f17b880a85"><a name="afab6fc762eb743c29c1cb7f17b880a85"></a><a name="afab6fc762eb743c29c1cb7f17b880a85"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.55%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0080995382_p650279617742"><a name="zh-cn_topic_0080995382_p650279617742"></a><a name="zh-cn_topic_0080995382_p650279617742"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.5.1.3 "><p id="ab8eae8645e994984aa6ff68bf125f05e"><a name="ab8eae8645e994984aa6ff68bf125f05e"></a><a name="ab8eae8645e994984aa6ff68bf125f05e"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.6%" headers="mcps1.2.5.1.4 "><p id="a540d928c47974814bb0784174ff1d23f"><a name="a540d928c47974814bb0784174ff1d23f"></a><a name="a540d928c47974814bb0784174ff1d23f"></a>管理该zone的管理员邮箱。</p>
    <p id="zh-cn_topic_0080995382_p16253220614"><a name="zh-cn_topic_0080995382_p16253220614"></a><a name="zh-cn_topic_0080995382_p16253220614"></a>如果为空，表示维持原值。</p>
    <p id="a28fb1a83bf20491b87499617246a4e58"><a name="a28fb1a83bf20491b87499617246a4e58"></a><a name="a28fb1a83bf20491b87499617246a4e58"></a>默认值为空。</p>
    </td>
    </tr>
    <tr id="ra92fe0b0bea5467696ded2189261f7e1"><td class="cellrowborder" valign="top" width="14.52%" headers="mcps1.2.5.1.1 "><p id="a14a07b00a14d405aa692873540c982cc"><a name="a14a07b00a14d405aa692873540c982cc"></a><a name="a14a07b00a14d405aa692873540c982cc"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.55%" headers="mcps1.2.5.1.2 "><p id="a85d682d35d8146f88b4efa38861c2441"><a name="a85d682d35d8146f88b4efa38861c2441"></a><a name="a85d682d35d8146f88b4efa38861c2441"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.5.1.3 "><p id="a40f021a44f29448d975126c695fb4e94"><a name="a40f021a44f29448d975126c695fb4e94"></a><a name="a40f021a44f29448d975126c695fb4e94"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.6%" headers="mcps1.2.5.1.4 "><p id="a968c40752cbb4776b95995372f3b7c1a"><a name="a968c40752cbb4776b95995372f3b7c1a"></a><a name="a968c40752cbb4776b95995372f3b7c1a"></a>用于填写默认生成的SOA记录中有效缓存时间，以秒为单位。</p>
    <p id="affaa28ae17564304bca18b476a63f0b4"><a name="affaa28ae17564304bca18b476a63f0b4"></a><a name="affaa28ae17564304bca18b476a63f0b4"></a>取值范围：</p>
    <p id="abdfd7506c98f46e5bfe546be775b52f4"><a name="abdfd7506c98f46e5bfe546be775b52f4"></a><a name="abdfd7506c98f46e5bfe546be775b52f4"></a>300~2147483647。</p>
    <p id="zh-cn_topic_0080995382_p52661425313"><a name="zh-cn_topic_0080995382_p52661425313"></a><a name="zh-cn_topic_0080995382_p52661425313"></a>如果为空，表示维持原值。</p>
    <p id="abf25df523584405790017ac5004fb6f5"><a name="abf25df523584405790017ac5004fb6f5"></a><a name="abf25df523584405790017ac5004fb6f5"></a>默认值为空。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    修改Zone ID为“2c9eb155587194ec01587224c9f90149”的域名信息。

    ```
    PATCH https://{DNS_Endpoint}/v2/zones/2c9eb155587194ec01587224c9f90149
    ```

    ```
    {
        "description": "This is an example zone.",
        "email": "xx@example.org",
        "ttl": 300
    }
    ```


## 响应<a name="section2142173017358"></a>

-   要素说明

    **表 3**  响应样例的要素说明

    <a name="table54601120171039"></a>
    <table><thead align="left"><tr id="r318933e6ce9c44e2a969016a56f54b87"><th class="cellrowborder" valign="top" width="18.37%" id="mcps1.2.4.1.1"><p id="afdb5e5497eb64a139f0d2c21f6ff1d94"><a name="afdb5e5497eb64a139f0d2c21f6ff1d94"></a><a name="afdb5e5497eb64a139f0d2c21f6ff1d94"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.39%" id="mcps1.2.4.1.2"><p id="a4c97f3baac734b45ae85d89e44bef37e"><a name="a4c97f3baac734b45ae85d89e44bef37e"></a><a name="a4c97f3baac734b45ae85d89e44bef37e"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.239999999999995%" id="mcps1.2.4.1.3"><p id="aa1f0887180484d7db960c625ed02b017"><a name="aa1f0887180484d7db960c625ed02b017"></a><a name="aa1f0887180484d7db960c625ed02b017"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r94cb17ae3b13430e98670a32a63a5caa"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a351211b9573245c7ace8b11f91e5aac5"><a name="a351211b9573245c7ace8b11f91e5aac5"></a><a name="a351211b9573245c7ace8b11f91e5aac5"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="a47667ac4d8b34540a85f994f7bb88f3e"><a name="a47667ac4d8b34540a85f994f7bb88f3e"></a><a name="a47667ac4d8b34540a85f994f7bb88f3e"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="ad6877fe93324416aab90b84e6d04169d"><a name="ad6877fe93324416aab90b84e6d04169d"></a><a name="ad6877fe93324416aab90b84e6d04169d"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="r2229bfd978d44b73814a6e7d879b6454"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="af8bb7c6911a841379501b3d3313e2c00"><a name="af8bb7c6911a841379501b3d3313e2c00"></a><a name="af8bb7c6911a841379501b3d3313e2c00"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="aa17915fbec1f4b118c7c85033f381a59"><a name="aa17915fbec1f4b118c7c85033f381a59"></a><a name="aa17915fbec1f4b118c7c85033f381a59"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="ad8eefd35bde147c68ae7abe18f72c2d6"><a name="ad8eefd35bde147c68ae7abe18f72c2d6"></a><a name="ad8eefd35bde147c68ae7abe18f72c2d6"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="r993e4cdcd1be41bb83c1f85c3fb6d7d6"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a5da8a442117c4dc6b2c9175ec6e6ddee"><a name="a5da8a442117c4dc6b2c9175ec6e6ddee"></a><a name="a5da8a442117c4dc6b2c9175ec6e6ddee"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="a1887e3805d0343e8acf2185e6853652a"><a name="a1887e3805d0343e8acf2185e6853652a"></a><a name="a1887e3805d0343e8acf2185e6853652a"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a34c95c53bd9b46a698bcdcac2d17e7e9"><a name="a34c95c53bd9b46a698bcdcac2d17e7e9"></a><a name="a34c95c53bd9b46a698bcdcac2d17e7e9"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="r59fc719cd95348fe8a030e073b85a209"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="ae2111a24793940ef80c619950e599192"><a name="ae2111a24793940ef80c619950e599192"></a><a name="ae2111a24793940ef80c619950e599192"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p336297171039"><a name="zh-cn_topic_0057311027_p336297171039"></a><a name="zh-cn_topic_0057311027_p336297171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a147f90e4636f4ae3b13182d32996c6c5"><a name="a147f90e4636f4ae3b13182d32996c6c5"></a><a name="a147f90e4636f4ae3b13182d32996c6c5"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="rbaa55719838a49d8ade18f21c00b1bd6"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a43a238d9dfe041cfa878dd5b96760604"><a name="a43a238d9dfe041cfa878dd5b96760604"></a><a name="a43a238d9dfe041cfa878dd5b96760604"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="a95e13dfe14c942ccb9b1f2b560c7430c"><a name="a95e13dfe14c942ccb9b1f2b560c7430c"></a><a name="a95e13dfe14c942ccb9b1f2b560c7430c"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p9394279212"><a name="p9394279212"></a><a name="p9394279212"></a>zone类型，公网（public）或者内网（private）。</p>
    </td>
    </tr>
    <tr id="re3b052108fa34b5e9c0a6bb456009250"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="afafe865e8e534c168eec8c44822c10a9"><a name="afafe865e8e534c168eec8c44822c10a9"></a><a name="afafe865e8e534c168eec8c44822c10a9"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="a9bd9de54fdcb4a77bc408a76a9f7a999"><a name="a9bd9de54fdcb4a77bc408a76a9f7a999"></a><a name="a9bd9de54fdcb4a77bc408a76a9f7a999"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a3a912cb7fb2e4d579e84296f9637a0dc"><a name="a3a912cb7fb2e4d579e84296f9637a0dc"></a><a name="a3a912cb7fb2e4d579e84296f9637a0dc"></a>该zone下SOA记录中的ttl值。</p>
    <p id="p0662131993410"><a name="p0662131993410"></a><a name="p0662131993410"></a>取值范围：300~2147483647</p>
    <p id="p7662111973418"><a name="p7662111973418"></a><a name="p7662111973418"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="race7c02633d648eeb49e7fcf89da86ad"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="adc16ebab44594ab096fb4516c4f597e3"><a name="adc16ebab44594ab096fb4516c4f597e3"></a><a name="adc16ebab44594ab096fb4516c4f597e3"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="a123548da301b40baa49f08a0f8f4129c"><a name="a123548da301b40baa49f08a0f8f4129c"></a><a name="a123548da301b40baa49f08a0f8f4129c"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p201115484116"><a name="p201115484116"></a><a name="p201115484116"></a>该zone下SOA记录中用于标识zone文件变更的序列值，用于主从节点同步。</p>
    <p id="p7524749171039"><a name="p7524749171039"></a><a name="p7524749171039"></a>该参数暂未使用。</p>
    </td>
    </tr>
    <tr id="re58847a4e7ac4c16af7f937d50f6be75"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="ae7b5fed19fe444a481e02e979ce2c3e3"><a name="ae7b5fed19fe444a481e02e979ce2c3e3"></a><a name="ae7b5fed19fe444a481e02e979ce2c3e3"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="a482a529c94cb443bafc545b8b309c654"><a name="a482a529c94cb443bafc545b8b309c654"></a><a name="a482a529c94cb443bafc545b8b309c654"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a30277a50368848b38e746604761c5d65"><a name="a30277a50368848b38e746604761c5d65"></a><a name="a30277a50368848b38e746604761c5d65"></a>资源状态。</p>
    <p id="zh-cn_topic_0057311027_p878313571410"><a name="zh-cn_topic_0057311027_p878313571410"></a><a name="zh-cn_topic_0057311027_p878313571410"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="r106f4bb096fe493895f95610909a5695"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a55ed88eabe20430dbb7c174ccb9f9098"><a name="a55ed88eabe20430dbb7c174ccb9f9098"></a><a name="a55ed88eabe20430dbb7c174ccb9f9098"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="ad6b67a0a5d8247c48c27e3f98b580421"><a name="ad6b67a0a5d8247c48c27e3f98b580421"></a><a name="ad6b67a0a5d8247c48c27e3f98b580421"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a23d48313d540467893d2e8ed2745df7f"><a name="a23d48313d540467893d2e8ed2745df7f"></a><a name="a23d48313d540467893d2e8ed2745df7f"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="r836f1aa44d6d4677957fcd1b16d80b05"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="aba20c68200f546629198b4c7ae4b51e5"><a name="aba20c68200f546629198b4c7ae4b51e5"></a><a name="aba20c68200f546629198b4c7ae4b51e5"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="a042da40702f840c4ad8c5854ca7c130b"><a name="a042da40702f840c4ad8c5854ca7c130b"></a><a name="a042da40702f840c4ad8c5854ca7c130b"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a3fd761e1538a41dab5a2accafe081021"><a name="a3fd761e1538a41dab5a2accafe081021"></a><a name="a3fd761e1538a41dab5a2accafe081021"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="r297bd05aa41f4ea49a13759d9418f43e"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a61fe74ffa6624d65ba007fe8d3d01ede"><a name="a61fe74ffa6624d65ba007fe8d3d01ede"></a><a name="a61fe74ffa6624d65ba007fe8d3d01ede"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="ae0bffeb0816e42b789c4d583e004818f"><a name="ae0bffeb0816e42b789c4d583e004818f"></a><a name="ae0bffeb0816e42b789c4d583e004818f"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p8704812171039"><a name="p8704812171039"></a><a name="p8704812171039"></a>zone所属的项目ID。</p>
    </td>
    </tr>
    <tr id="r8463bc32c80b46e5aea56e1008192352"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a5f328d90b9494167974374d31c2fbbd8"><a name="a5f328d90b9494167974374d31c2fbbd8"></a><a name="a5f328d90b9494167974374d31c2fbbd8"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="ade042db7b99e42f589039904ed0d1c9b"><a name="ade042db7b99e42f589039904ed0d1c9b"></a><a name="ade042db7b99e42f589039904ed0d1c9b"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a0a619f7bac0c48acbf17c43865c0dafb"><a name="a0a619f7bac0c48acbf17c43865c0dafb"></a><a name="a0a619f7bac0c48acbf17c43865c0dafb"></a>创建时间。</p>
    <p id="p583516468316"><a name="p583516468316"></a><a name="p583516468316"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="r42fdbc0229d94cf78b006ba57b634f2e"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a10297bac5cde43b3a82a514ab7c3b51f"><a name="a10297bac5cde43b3a82a514ab7c3b51f"></a><a name="a10297bac5cde43b3a82a514ab7c3b51f"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="a83919e1000ce4c20811d75e9d5572c7a"><a name="a83919e1000ce4c20811d75e9d5572c7a"></a><a name="a83919e1000ce4c20811d75e9d5572c7a"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a05f275c2fe0d4ba38dc5f2942b24e0a2"><a name="a05f275c2fe0d4ba38dc5f2942b24e0a2"></a><a name="a05f275c2fe0d4ba38dc5f2942b24e0a2"></a>更新时间。</p>
    <p id="zh-cn_topic_0057311027_p799714202510"><a name="zh-cn_topic_0057311027_p799714202510"></a><a name="zh-cn_topic_0057311027_p799714202510"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="ra3bcb082cd044c249c0384dbc9d797ce"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p288749251572"><a name="zh-cn_topic_0057311027_p288749251572"></a><a name="zh-cn_topic_0057311027_p288749251572"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p571676251572"><a name="zh-cn_topic_0057311027_p571676251572"></a><a name="zh-cn_topic_0057311027_p571676251572"></a>Object</p>
    <p id="p7650618171011"><a name="p7650618171011"></a><a name="p7650618171011"></a></p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a070f1d50477745b5882c7d4f45018aff"><a name="a070f1d50477745b5882c7d4f45018aff"></a><a name="a070f1d50477745b5882c7d4f45018aff"></a>指向当前资源或者其他资源的链接。</p>
    <p id="zh-cn_topic_0057311027_p660161572"><a name="zh-cn_topic_0057311027_p660161572"></a><a name="zh-cn_topic_0057311027_p660161572"></a>当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p4628317174618"><a name="p4628317174618"></a><a name="p4628317174618"></a>详细信息请参见<a href="#table52442344175457">表4</a>。</p>
    </td>
    </tr>
    <tr id="rc90495e06a7e4457b95cc2d940940567"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="afcba5be99ef0439f8b0ca0e558f90e8b"><a name="afcba5be99ef0439f8b0ca0e558f90e8b"></a><a name="afcba5be99ef0439f8b0ca0e558f90e8b"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="a24cc31056df64a4794ccb3989b481240"><a name="a24cc31056df64a4794ccb3989b481240"></a><a name="a24cc31056df64a4794ccb3989b481240"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="aecd21264341f447998b070e439eca8a0"><a name="aecd21264341f447998b070e439eca8a0"></a><a name="aecd21264341f447998b070e439eca8a0"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    <p id="zh-cn_topic_0057311027_p9475575518"><a name="zh-cn_topic_0057311027_p9475575518"></a><a name="zh-cn_topic_0057311027_p9475575518"></a>目前暂未使用。</p>
    </td>
    </tr>
    <tr id="r926630e41cb24a96818249071f58c48a"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a3c260ed464664ec7a1078e96c6fa2e82"><a name="a3c260ed464664ec7a1078e96c6fa2e82"></a><a name="a3c260ed464664ec7a1078e96c6fa2e82"></a>routers</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="af4d8729ebfa6438aaa842810310f4cec"><a name="af4d8729ebfa6438aaa842810310f4cec"></a><a name="af4d8729ebfa6438aaa842810310f4cec"></a>Array of object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a1ab67663b21049b49f722e4cef72c56c"><a name="a1ab67663b21049b49f722e4cef72c56c"></a><a name="a1ab67663b21049b49f722e4cef72c56c"></a>Private zone关联的Router(VPC)信息。详细信息请参见<a href="#table4448008117179">表5</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  links参数说明

    <a name="table52442344175457"></a>
    <table><thead align="left"><tr id="row58979189175457"><th class="cellrowborder" valign="top" width="18.3018301830183%" id="mcps1.2.4.1.1"><p id="p46156243175457"><a name="p46156243175457"></a><a name="p46156243175457"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.591959195919593%" id="mcps1.2.4.1.2"><p id="p47668234175457"><a name="p47668234175457"></a><a name="p47668234175457"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.10621062106211%" id="mcps1.2.4.1.3"><p id="p35921708175457"><a name="p35921708175457"></a><a name="p35921708175457"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row54859922175457"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p14468674175457"><a name="p14468674175457"></a><a name="p14468674175457"></a>self</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.591959195919593%" headers="mcps1.2.4.1.2 "><p id="p31111955175457"><a name="p31111955175457"></a><a name="p31111955175457"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.10621062106211%" headers="mcps1.2.4.1.3 "><p id="p37040428175457"><a name="p37040428175457"></a><a name="p37040428175457"></a>当前资源的链接。</p>
    </td>
    </tr>
    <tr id="row13441257174812"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.591959195919593%" headers="mcps1.2.4.1.2 "><p id="p19656144517367"><a name="p19656144517367"></a><a name="p19656144517367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.10621062106211%" headers="mcps1.2.4.1.3 "><p id="p76567451365"><a name="p76567451365"></a><a name="p76567451365"></a>下一页资源的链接。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  routers对象参数说明

    <a name="table4448008117179"></a>
    <table><thead align="left"><tr id="row6132935617179"><th class="cellrowborder" valign="top" width="18.538146185381464%" id="mcps1.2.4.1.1"><p id="p36588677171719"><a name="p36588677171719"></a><a name="p36588677171719"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.668033196680334%" id="mcps1.2.4.1.2"><p id="p9906869171719"><a name="p9906869171719"></a><a name="p9906869171719"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="61.79382061793821%" id="mcps1.2.4.1.3"><p id="p64258954171719"><a name="p64258954171719"></a><a name="p64258954171719"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1024510342619"><td class="cellrowborder" valign="top" width="18.538146185381464%" headers="mcps1.2.4.1.1 "><p id="p38120631175524"><a name="p38120631175524"></a><a name="p38120631175524"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.668033196680334%" headers="mcps1.2.4.1.2 "><p id="p57184665175519"><a name="p57184665175519"></a><a name="p57184665175519"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.79382061793821%" headers="mcps1.2.4.1.3 "><p id="p1635999216648"><a name="p1635999216648"></a><a name="p1635999216648"></a>资源状态。</p>
    <p id="p656495918714"><a name="p656495918714"></a><a name="p656495918714"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="row266872817179"><td class="cellrowborder" valign="top" width="18.538146185381464%" headers="mcps1.2.4.1.1 "><p id="p25118582171719"><a name="p25118582171719"></a><a name="p25118582171719"></a>router_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.668033196680334%" headers="mcps1.2.4.1.2 "><p id="p50755907171719"><a name="p50755907171719"></a><a name="p50755907171719"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.79382061793821%" headers="mcps1.2.4.1.3 "><p id="p17587794171719"><a name="p17587794171719"></a><a name="p17587794171719"></a>Router(VPC)所属VPC的ID。</p>
    <p id="p143411822947"><a name="p143411822947"></a><a name="p143411822947"></a>该参数的值可以通过如下两种方式获取：</p>
    <a name="ul1938314911411"></a><a name="ul1938314911411"></a><ul id="ul1938314911411"><li>通过虚拟私有云的管理控制台，在VPC的详情页面中获取VPC的ID。</li><li>通过<a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0003.html" target="_blank" rel="noopener noreferrer">查询VPC列表</a>获取VPC ID。</li></ul>
    </td>
    </tr>
    <tr id="row6657832817179"><td class="cellrowborder" valign="top" width="18.538146185381464%" headers="mcps1.2.4.1.1 "><p id="p3709384171719"><a name="p3709384171719"></a><a name="p3709384171719"></a>router_region</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.668033196680334%" headers="mcps1.2.4.1.2 "><p id="p43861924171719"><a name="p43861924171719"></a><a name="p43861924171719"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.79382061793821%" headers="mcps1.2.4.1.3 "><p id="p63154928171719"><a name="p63154928171719"></a><a name="p63154928171719"></a>Router(VPC)所在的region。</p>
    <p id="p38645142171939"><a name="p38645142171939"></a><a name="p38645142171939"></a>如果为空，默认为token中project所在的region。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "id": "ff8080825b8fc86c015b94bc6f8712c3",
        "name": "example.com.",
        "description": "This is an example zone.",
        "email": "xx@example.com",
        "ttl": 300,
        "serial": 1,
        "masters": [],
        "status": "ACTIVE",
        "links": {
            "self": "https://Endpoint/v2/zones/ff8080825b8fc86c015b94bc6f8712c3"
        },
        "pool_id": "ff8080825ab738f4015ab7513298010e",
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
        "zone_type": "private",
        "created_at": "2017-04-22T08:17:08.997",
        "updated_at": "2017-04-22T08:17:10.849",
        "record_num": 2,
        "routers": [
          {
              "status": "ACTIVE",
              "router_id": "19664294-0bf6-4271-ad3a-94b8c79c6558",
              "router_region": "xx"
            }
        ]
    }
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

