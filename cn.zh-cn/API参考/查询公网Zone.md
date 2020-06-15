# 查询公网Zone<a name="dns_api_62002"></a>

## 功能介绍<a name="section55898385"></a>

查询单个公网Zone。

## URI<a name="section33323423"></a>

GET /v2/zones/\{zone\_id\}

参数说明请参见[表1](#table14024165)。

**表 1**  URI格式的参数说明

<a name="table14024165"></a>
<table><thead align="left"><tr id="row26592044"><th class="cellrowborder" valign="top" width="15.459999999999999%" id="mcps1.2.5.1.1"><p id="p6471942"><a name="p6471942"></a><a name="p6471942"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.459999999999999%" id="mcps1.2.5.1.2"><p id="p54465313"><a name="p54465313"></a><a name="p54465313"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.53%" id="mcps1.2.5.1.3"><p id="p49614245"><a name="p49614245"></a><a name="p49614245"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.55%" id="mcps1.2.5.1.4"><p id="p59330872"><a name="p59330872"></a><a name="p59330872"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row41071365"><td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.5.1.1 "><p id="p38446258"><a name="p38446258"></a><a name="p38446258"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.5.1.2 "><p id="p27139175"><a name="p27139175"></a><a name="p27139175"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.2.5.1.3 "><p id="p50789581"><a name="p50789581"></a><a name="p50789581"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.55%" headers="mcps1.2.5.1.4 "><p id="p20315403"><a name="p20315403"></a><a name="p20315403"></a>待查询zone的ID。</p>
<p id="p1669018482183"><a name="p1669018482183"></a><a name="p1669018482183"></a>可以通过<a href="查询公网Zone列表.md">查询公网Zone列表</a>获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section31475357"></a>

-   请求参数

    无

-   请求样例

    查询域名Zone ID为“2c9eb155587194ec01587224c9f90149”的域名。

    ```
    GET https://{DNS_Endpoint}/v2/zones/2c9eb155587194ec01587224c9f90149
    ```


## 响应<a name="section14842765"></a>

-   要素说明

    **表 2**  响应样例的要素说明

    <a name="table54967495"></a>
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
    </td>
    </tr>
    <tr id="r6f01d44c0047469b9ee578db3ae2e925"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="ac99c652f1d284ec496be4ad0b5364a1a"><a name="ac99c652f1d284ec496be4ad0b5364a1a"></a><a name="ac99c652f1d284ec496be4ad0b5364a1a"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="ae5ee649ac6aa4bb4a20e678d9a24e19a"><a name="ae5ee649ac6aa4bb4a20e678d9a24e19a"></a><a name="ae5ee649ac6aa4bb4a20e678d9a24e19a"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p1786474013426"><a name="p1786474013426"></a><a name="p1786474013426"></a>该zone下SOA记录中用于标识zone文件变更的序列值，用于主从节点同步。</p>
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
    <p id="a0d1ae2e82e4645939f6aa3d118f88914"><a name="a0d1ae2e82e4645939f6aa3d118f88914"></a><a name="a0d1ae2e82e4645939f6aa3d118f88914"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
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
    <p id="p286121420434"><a name="p286121420434"></a><a name="p286121420434"></a>详细信息请参见<a href="#table0172144213344">表3</a>。</p>
    </td>
    </tr>
    <tr id="r5a57c1dba2934130a772bfc188e27c7b"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="a414da27796154a8ea0f3f5d155266ce6"><a name="a414da27796154a8ea0f3f5d155266ce6"></a><a name="a414da27796154a8ea0f3f5d155266ce6"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="ac58ddffcdd4b4db48b9da9a1aa4b94b8"><a name="ac58ddffcdd4b4db48b9da9a1aa4b94b8"></a><a name="ac58ddffcdd4b4db48b9da9a1aa4b94b8"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="a67f94f4a1cee4d80ad3886d215def3de"><a name="a67f94f4a1cee4d80ad3886d215def3de"></a><a name="a67f94f4a1cee4d80ad3886d215def3de"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    <p id="zh-cn_topic_0057310891_p05918233215"><a name="zh-cn_topic_0057310891_p05918233215"></a><a name="zh-cn_topic_0057310891_p05918233215"></a>目前暂未使用。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  links对象参数说明

    <a name="table0172144213344"></a>
    <table><thead align="left"><tr id="row917304253418"><th class="cellrowborder" valign="top" width="18%" id="mcps1.2.4.1.1"><p id="p101731742153416"><a name="p101731742153416"></a><a name="p101731742153416"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.25%" id="mcps1.2.4.1.2"><p id="p0174542163418"><a name="p0174542163418"></a><a name="p0174542163418"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.74999999999999%" id="mcps1.2.4.1.3"><p id="p7174194243414"><a name="p7174194243414"></a><a name="p7174194243414"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1390694871216"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="p8907184881217"><a name="p8907184881217"></a><a name="p8907184881217"></a>self</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.25%" headers="mcps1.2.4.1.2 "><p id="p9907184891219"><a name="p9907184891219"></a><a name="p9907184891219"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.74999999999999%" headers="mcps1.2.4.1.3 "><p id="p1890754813127"><a name="p1890754813127"></a><a name="p1890754813127"></a>当前资源的链接。</p>
    </td>
    </tr>
    <tr id="row1999616550462"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.25%" headers="mcps1.2.4.1.2 "><p id="p19656144517367"><a name="p19656144517367"></a><a name="p19656144517367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.74999999999999%" headers="mcps1.2.4.1.3 "><p id="p76567451365"><a name="p76567451365"></a><a name="p76567451365"></a>下一页资源的链接。</p>
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
        "serial": 0,
        "masters": [],
        "status": "ACTIVE",
        "links": {
            "self": "https://Endpoint/v2/zones/2c9eb155587194ec01587224c9f90149"
        },
        "pool_id": "00000000570e54ee01570e9939b20019",
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
        "zone_type": "public",
        "created_at": "2016-11-17T11:56:03.439",
        "updated_at": "2016-11-17T11:56:05.528",
        "record_num": 2
    }
    
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

