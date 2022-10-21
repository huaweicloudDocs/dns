# 修改公网Zone<a name="dns_api_62006"></a>

## 功能介绍<a name="section2763065016101"></a>

修改单个Zone。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=DNS&api=UpdatePublicZone)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI<a name="section53701671161015"></a>

PATCH /v2/zones/\{zone\_id\}

参数说明请参见[表1](#table56746773172616)。

**表 1**  URI格式的参数说明

<a name="table56746773172616"></a>
<table><thead align="left"><tr id="row12848229172616"><th class="cellrowborder" valign="top" width="16.75%" id="mcps1.2.5.1.1"><p id="p44975878172616"><a name="p44975878172616"></a><a name="p44975878172616"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.67%" id="mcps1.2.5.1.2"><p id="p46443918172616"><a name="p46443918172616"></a><a name="p46443918172616"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.23%" id="mcps1.2.5.1.3"><p id="p1368350172616"><a name="p1368350172616"></a><a name="p1368350172616"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="49.35%" id="mcps1.2.5.1.4"><p id="p24157908172616"><a name="p24157908172616"></a><a name="p24157908172616"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row39993297172616"><td class="cellrowborder" valign="top" width="16.75%" headers="mcps1.2.5.1.1 "><p id="p43071797172616"><a name="p43071797172616"></a><a name="p43071797172616"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.67%" headers="mcps1.2.5.1.2 "><p id="p26647585172616"><a name="p26647585172616"></a><a name="p26647585172616"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.5.1.3 "><p id="p21075379172616"><a name="p21075379172616"></a><a name="p21075379172616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.35%" headers="mcps1.2.5.1.4 "><p id="p4976396172616"><a name="p4976396172616"></a><a name="p4976396172616"></a>待修改zone的ID。</p>
<p id="p1669018482183"><a name="p1669018482183"></a><a name="p1669018482183"></a>可以通过<a href="查询公网Zone列表.md">查询公网Zone列表</a>获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section44958995161021"></a>

-   参数说明

    **表 2**  请求样例的参数说明

    <a name="table3720408817742"></a>
    <table><thead align="left"><tr id="row6225671717742"><th class="cellrowborder" valign="top" width="16.32%" id="mcps1.2.5.1.1"><p id="p5153686617742"><a name="p5153686617742"></a><a name="p5153686617742"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.97%" id="mcps1.2.5.1.2"><p id="p473035017742"><a name="p473035017742"></a><a name="p473035017742"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.41%" id="mcps1.2.5.1.3"><p id="p386753717742"><a name="p386753717742"></a><a name="p386753717742"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="50.3%" id="mcps1.2.5.1.4"><p id="p5956810717742"><a name="p5956810717742"></a><a name="p5956810717742"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1973909717742"><td class="cellrowborder" valign="top" width="16.32%" headers="mcps1.2.5.1.1 "><p id="p5474826717742"><a name="p5474826717742"></a><a name="p5474826717742"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.97%" headers="mcps1.2.5.1.2 "><p id="p759162017742"><a name="p759162017742"></a><a name="p759162017742"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.5.1.3 "><p id="p3220634117742"><a name="p3220634117742"></a><a name="p3220634117742"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.3%" headers="mcps1.2.5.1.4 "><p id="p6675950017742"><a name="p6675950017742"></a><a name="p6675950017742"></a>域名的描述信息。长度不超过255个字符。</p>
    <p id="p37540522006"><a name="p37540522006"></a><a name="p37540522006"></a>如果为空，表示维持原值。</p>
    <p id="p474692155919"><a name="p474692155919"></a><a name="p474692155919"></a>默认值为空。</p>
    </td>
    </tr>
    <tr id="row4358988017742"><td class="cellrowborder" valign="top" width="16.32%" headers="mcps1.2.5.1.1 "><p id="p6536976617742"><a name="p6536976617742"></a><a name="p6536976617742"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.97%" headers="mcps1.2.5.1.2 "><p id="p650279617742"><a name="p650279617742"></a><a name="p650279617742"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.5.1.3 "><p id="p2054573717742"><a name="p2054573717742"></a><a name="p2054573717742"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.3%" headers="mcps1.2.5.1.4 "><p id="p1997196517742"><a name="p1997196517742"></a><a name="p1997196517742"></a>管理该zone的管理员邮箱。</p>
    <p id="p16253220614"><a name="p16253220614"></a><a name="p16253220614"></a>如果为空，表示维持原值。</p>
    <p id="p8877142595919"><a name="p8877142595919"></a><a name="p8877142595919"></a>默认值为空。</p>
    </td>
    </tr>
    <tr id="row13489593141045"><td class="cellrowborder" valign="top" width="16.32%" headers="mcps1.2.5.1.1 "><p id="p18915273141045"><a name="p18915273141045"></a><a name="p18915273141045"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.97%" headers="mcps1.2.5.1.2 "><p id="p55742162141045"><a name="p55742162141045"></a><a name="p55742162141045"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.5.1.3 "><p id="p18821243141045"><a name="p18821243141045"></a><a name="p18821243141045"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.3%" headers="mcps1.2.5.1.4 "><p id="p3447255141334"><a name="p3447255141334"></a><a name="p3447255141334"></a>用于填写默认生成的SOA记录中有效缓存时间，以秒为单位。</p>
    <p id="p5335091141210"><a name="p5335091141210"></a><a name="p5335091141210"></a>取值范围：</p>
    <p id="p43707626141214"><a name="p43707626141214"></a><a name="p43707626141214"></a>300~2147483647。</p>
    <p id="p52661425313"><a name="p52661425313"></a><a name="p52661425313"></a>如果为空，表示维持原值。</p>
    <p id="p61411742165919"><a name="p61411742165919"></a><a name="p61411742165919"></a>默认值为空。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    修改域名Zone ID为“2c9eb155587194ec01587224c9f90149”的域名信息。

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


## 响应<a name="section40090803161031"></a>

-   要素说明

    **表 3**  响应样例的要素说明

    <a name="table3873760215524"></a>
    <table><thead align="left"><tr id="rcb8f5a6dbdc841d5b61b57c9a7f3946c"><th class="cellrowborder" valign="top" width="18.41%" id="mcps1.2.4.1.1"><p id="a562463c38c994a46a5042605cbae16a2"><a name="a562463c38c994a46a5042605cbae16a2"></a><a name="a562463c38c994a46a5042605cbae16a2"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.35%" id="mcps1.2.4.1.2"><p id="a037a944fa232408f9eb6d06f523458c3"><a name="a037a944fa232408f9eb6d06f523458c3"></a><a name="a037a944fa232408f9eb6d06f523458c3"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.239999999999995%" id="mcps1.2.4.1.3"><p id="ab503838cab8b41b5aacf832f2abc24e4"><a name="ab503838cab8b41b5aacf832f2abc24e4"></a><a name="ab503838cab8b41b5aacf832f2abc24e4"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r90f043c750eb4b4e8d242b7f8db14709"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="a8bb1298f194542789a4889ca1ecb0500"><a name="a8bb1298f194542789a4889ca1ecb0500"></a><a name="a8bb1298f194542789a4889ca1ecb0500"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="ae7f12de3cd5143d9b7c81746c73de547"><a name="ae7f12de3cd5143d9b7c81746c73de547"></a><a name="ae7f12de3cd5143d9b7c81746c73de547"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="af2aa29bf11dc4ede8a83ffe698c6d015"><a name="af2aa29bf11dc4ede8a83ffe698c6d015"></a><a name="af2aa29bf11dc4ede8a83ffe698c6d015"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="rd94a8eae3993428ba58b7935d38f2c42"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="a5b7f90ac0e964a4e8d5c3b54801a0263"><a name="a5b7f90ac0e964a4e8d5c3b54801a0263"></a><a name="a5b7f90ac0e964a4e8d5c3b54801a0263"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="a7f54cec7482f402295ad3e3bbf884023"><a name="a7f54cec7482f402295ad3e3bbf884023"></a><a name="a7f54cec7482f402295ad3e3bbf884023"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a84a47ec529944403bd51bd1a130bfa9a"><a name="a84a47ec529944403bd51bd1a130bfa9a"></a><a name="a84a47ec529944403bd51bd1a130bfa9a"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="r8a93c0d071624062b4332156e7c1afd3"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="ac8461d5571384d2f99735f4dd17f36e4"><a name="ac8461d5571384d2f99735f4dd17f36e4"></a><a name="ac8461d5571384d2f99735f4dd17f36e4"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="ac782ad392b6549dc9a55042f0e89e799"><a name="ac782ad392b6549dc9a55042f0e89e799"></a><a name="ac782ad392b6549dc9a55042f0e89e799"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="abf3153770d0a4cf8a9ee79c8455167d5"><a name="abf3153770d0a4cf8a9ee79c8455167d5"></a><a name="abf3153770d0a4cf8a9ee79c8455167d5"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="rd2df7eeb23d348c3825c57d44911c2c0"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="a5228458b23264d239a4eee40c3001c4f"><a name="a5228458b23264d239a4eee40c3001c4f"></a><a name="a5228458b23264d239a4eee40c3001c4f"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p336297171039"><a name="zh-cn_topic_0057310891_p336297171039"></a><a name="zh-cn_topic_0057310891_p336297171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a72bf01280e51418ea295143d10e30fdb"><a name="a72bf01280e51418ea295143d10e30fdb"></a><a name="a72bf01280e51418ea295143d10e30fdb"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="rf57ffed6121d407da625ad56b3b3741f"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="ac0b14f3593ff4331b7cd6056c8d36a44"><a name="ac0b14f3593ff4331b7cd6056c8d36a44"></a><a name="ac0b14f3593ff4331b7cd6056c8d36a44"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="aab451733f1be44f8ac79d479ca1093f3"><a name="aab451733f1be44f8ac79d479ca1093f3"></a><a name="aab451733f1be44f8ac79d479ca1093f3"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a57638dc3c92f4e10850d4d6ad42a846e"><a name="a57638dc3c92f4e10850d4d6ad42a846e"></a><a name="a57638dc3c92f4e10850d4d6ad42a846e"></a>zone类型，公网（public）或者内网（private）。</p>
    </td>
    </tr>
    <tr id="ra6a15f87215c470e8c2fa6d2aa4a8ccc"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="a2e889a776aeb42f59e288b92b372bd70"><a name="a2e889a776aeb42f59e288b92b372bd70"></a><a name="a2e889a776aeb42f59e288b92b372bd70"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="a292032dd82fe4a0dbf0ff69bfd93d876"><a name="a292032dd82fe4a0dbf0ff69bfd93d876"></a><a name="a292032dd82fe4a0dbf0ff69bfd93d876"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="ab96c3883e8424c3187881c9ea265794f"><a name="ab96c3883e8424c3187881c9ea265794f"></a><a name="ab96c3883e8424c3187881c9ea265794f"></a>该zone下SOA记录中的ttl值。</p>
    <p id="p0662131993410"><a name="p0662131993410"></a><a name="p0662131993410"></a>取值范围：1~2147483647。</p>
    <p id="p7662111973418"><a name="p7662111973418"></a><a name="p7662111973418"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="r6f01d44c0047469b9ee578db3ae2e925"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="ac99c652f1d284ec496be4ad0b5364a1a"><a name="ac99c652f1d284ec496be4ad0b5364a1a"></a><a name="ac99c652f1d284ec496be4ad0b5364a1a"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="ae5ee649ac6aa4bb4a20e678d9a24e19a"><a name="ae5ee649ac6aa4bb4a20e678d9a24e19a"></a><a name="ae5ee649ac6aa4bb4a20e678d9a24e19a"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p201115484116"><a name="p201115484116"></a><a name="p201115484116"></a>该zone下SOA记录中用于标识zone文件变更的序列值，用于主从节点同步。</p>
    <p id="p7524749171039"><a name="p7524749171039"></a><a name="p7524749171039"></a>该参数暂未使用。</p>
    </td>
    </tr>
    <tr id="r50c368b3aa0b46f38a4617b7f797786f"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="a1d2ec6fad225464f9732756d33a337b2"><a name="a1d2ec6fad225464f9732756d33a337b2"></a><a name="a1d2ec6fad225464f9732756d33a337b2"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="a62bc066b1f5844588aa3d383f46fe71f"><a name="a62bc066b1f5844588aa3d383f46fe71f"></a><a name="a62bc066b1f5844588aa3d383f46fe71f"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="aa34a63cd4c824904be6636a6daaa09a9"><a name="aa34a63cd4c824904be6636a6daaa09a9"></a><a name="aa34a63cd4c824904be6636a6daaa09a9"></a>资源状态。</p>
    <p id="a0a74025bb90644338ac11860b3ef9f42"><a name="a0a74025bb90644338ac11860b3ef9f42"></a><a name="a0a74025bb90644338ac11860b3ef9f42"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="r3d7c6c02e04d40c0bdd0ef0a8a6045f9"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="a4873ee3d3c85419b9aba19243d2c84a7"><a name="a4873ee3d3c85419b9aba19243d2c84a7"></a><a name="a4873ee3d3c85419b9aba19243d2c84a7"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="a162e7c19e8be4764a2becf7706a46e6e"><a name="a162e7c19e8be4764a2becf7706a46e6e"></a><a name="a162e7c19e8be4764a2becf7706a46e6e"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="ab88a87d30e8e491f99661f9757711d6d"><a name="ab88a87d30e8e491f99661f9757711d6d"></a><a name="ab88a87d30e8e491f99661f9757711d6d"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="rfba699f600ef424cadbca2cd85b60887"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="a2271452821c249cb9f3a445fcf60a03f"><a name="a2271452821c249cb9f3a445fcf60a03f"></a><a name="a2271452821c249cb9f3a445fcf60a03f"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="a3fbd39a058f042e190756f9b4f941e56"><a name="a3fbd39a058f042e190756f9b4f941e56"></a><a name="a3fbd39a058f042e190756f9b4f941e56"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a8caf365222c34b929a1501acd4493bd1"><a name="a8caf365222c34b929a1501acd4493bd1"></a><a name="a8caf365222c34b929a1501acd4493bd1"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="ra366d35afa104cab8a41e36b89ca0e82"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="a3026f7c44fdc4ca887f0469710558f47"><a name="a3026f7c44fdc4ca887f0469710558f47"></a><a name="a3026f7c44fdc4ca887f0469710558f47"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="ac54288dbf5be47a98690cfeff1e25721"><a name="ac54288dbf5be47a98690cfeff1e25721"></a><a name="ac54288dbf5be47a98690cfeff1e25721"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="ad419bb0aafcd4bd2adf188dbd375f71e"><a name="ad419bb0aafcd4bd2adf188dbd375f71e"></a><a name="ad419bb0aafcd4bd2adf188dbd375f71e"></a>zone所属的项目ID。</p>
    </td>
    </tr>
    <tr id="r3bb52953237f4d90883feb17321b3754"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="aa1ed0627514440769d59691c0297bb20"><a name="aa1ed0627514440769d59691c0297bb20"></a><a name="aa1ed0627514440769d59691c0297bb20"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="a5131a3345de141acba4d51eceb924480"><a name="a5131a3345de141acba4d51eceb924480"></a><a name="a5131a3345de141acba4d51eceb924480"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a4c5d9647086944e888608bc848e37e4c"><a name="a4c5d9647086944e888608bc848e37e4c"></a><a name="a4c5d9647086944e888608bc848e37e4c"></a>创建时间。</p>
    <p id="p583516468316"><a name="p583516468316"></a><a name="p583516468316"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="rf0e8562b23244c968c21c2f7ffc1e376"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="a27068ff11a0443f9ad9964f4934f1be6"><a name="a27068ff11a0443f9ad9964f4934f1be6"></a><a name="a27068ff11a0443f9ad9964f4934f1be6"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="a8d6c4b16bc5c4b42a86e2ea9ebdff263"><a name="a8d6c4b16bc5c4b42a86e2ea9ebdff263"></a><a name="a8d6c4b16bc5c4b42a86e2ea9ebdff263"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a904e167e17d0450aa1f324b045fb7f4f"><a name="a904e167e17d0450aa1f324b045fb7f4f"></a><a name="a904e167e17d0450aa1f324b045fb7f4f"></a>更新时间。</p>
    <p id="zh-cn_topic_0057310891_p583516468316"><a name="zh-cn_topic_0057310891_p583516468316"></a><a name="zh-cn_topic_0057310891_p583516468316"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="rc71d074f37b143968b8b33fb7d0887c8"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p288749251572"><a name="zh-cn_topic_0057310891_p288749251572"></a><a name="zh-cn_topic_0057310891_p288749251572"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p571676251572"><a name="zh-cn_topic_0057310891_p571676251572"></a><a name="zh-cn_topic_0057310891_p571676251572"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p660161572"><a name="zh-cn_topic_0057310891_p660161572"></a><a name="zh-cn_topic_0057310891_p660161572"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p202920222455"><a name="p202920222455"></a><a name="p202920222455"></a>详细信息请参见<a href="#table0172144213344">表4</a>。</p>
    </td>
    </tr>
    <tr id="r5a57c1dba2934130a772bfc188e27c7b"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="a414da27796154a8ea0f3f5d155266ce6"><a name="a414da27796154a8ea0f3f5d155266ce6"></a><a name="a414da27796154a8ea0f3f5d155266ce6"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="ac58ddffcdd4b4db48b9da9a1aa4b94b8"><a name="ac58ddffcdd4b4db48b9da9a1aa4b94b8"></a><a name="ac58ddffcdd4b4db48b9da9a1aa4b94b8"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a67f94f4a1cee4d80ad3886d215def3de"><a name="a67f94f4a1cee4d80ad3886d215def3de"></a><a name="a67f94f4a1cee4d80ad3886d215def3de"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    <p id="zh-cn_topic_0057310891_p05918233215"><a name="zh-cn_topic_0057310891_p05918233215"></a><a name="zh-cn_topic_0057310891_p05918233215"></a>目前暂未使用。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  links对象参数说明

    <a name="table0172144213344"></a>
    <table><thead align="left"><tr id="row917304253418"><th class="cellrowborder" valign="top" width="18.099999999999998%" id="mcps1.2.4.1.1"><p id="p101731742153416"><a name="p101731742153416"></a><a name="p101731742153416"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.88%" id="mcps1.2.4.1.2"><p id="p0174542163418"><a name="p0174542163418"></a><a name="p0174542163418"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.019999999999996%" id="mcps1.2.4.1.3"><p id="p7174194243414"><a name="p7174194243414"></a><a name="p7174194243414"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1390694871216"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.2.4.1.1 "><p id="p8907184881217"><a name="p8907184881217"></a><a name="p8907184881217"></a>self</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.88%" headers="mcps1.2.4.1.2 "><p id="p9907184891219"><a name="p9907184891219"></a><a name="p9907184891219"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.019999999999996%" headers="mcps1.2.4.1.3 "><p id="p1890754813127"><a name="p1890754813127"></a><a name="p1890754813127"></a>当前资源的链接。</p>
    </td>
    </tr>
    <tr id="row15778204719370"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.88%" headers="mcps1.2.4.1.2 "><p id="p19656144517367"><a name="p19656144517367"></a><a name="p19656144517367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.019999999999996%" headers="mcps1.2.4.1.3 "><p id="p76567451365"><a name="p76567451365"></a><a name="p76567451365"></a>下一页资源的链接。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "id": "2c9eb155587194ec01587224c9f90149",
        "name": "example.com.",
        "description": "This is an example zone.",
        "email": "xx@example.com",
        "ttl": 300,
        "serial": 1,
        "masters": [],
        "status": "ACTIVE",
        "links": {
            "self": "https://Endpoint/v2/zones/2c9eb155587194ec01587224c9f90149"
        },
        "pool_id": "00000000570e54ee01570e9939b20019",
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
        "zone_type": "public",
        "created_at": "2016-11-17T11:56:03.439",
        "updated_at": "2016-11-17T11:56:05.749",
        "record_num": 2
    }
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

