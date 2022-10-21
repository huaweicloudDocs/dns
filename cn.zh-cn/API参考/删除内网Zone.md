# 删除内网Zone<a name="dns_api_63008"></a>

## 功能介绍<a name="section2763065016101"></a>

删除单个内网Zone。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=DNS&api=DeletePrivateZone)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI<a name="section53701671161015"></a>

DELETE /v2/zones/\{zone\_id\}

参数说明请参见[表1](#table56746773172616)。

**表 1**  URI格式的参数说明

<a name="table56746773172616"></a>
<table><thead align="left"><tr id="row12848229172616"><th class="cellrowborder" valign="top" width="15.459999999999999%" id="mcps1.2.5.1.1"><p id="p44975878172616"><a name="p44975878172616"></a><a name="p44975878172616"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.459999999999999%" id="mcps1.2.5.1.2"><p id="p46443918172616"><a name="p46443918172616"></a><a name="p46443918172616"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.53%" id="mcps1.2.5.1.3"><p id="p1368350172616"><a name="p1368350172616"></a><a name="p1368350172616"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.55%" id="mcps1.2.5.1.4"><p id="p24157908172616"><a name="p24157908172616"></a><a name="p24157908172616"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row39993297172616"><td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.5.1.1 "><p id="p43071797172616"><a name="p43071797172616"></a><a name="p43071797172616"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.5.1.2 "><p id="p26647585172616"><a name="p26647585172616"></a><a name="p26647585172616"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.2.5.1.3 "><p id="p21075379172616"><a name="p21075379172616"></a><a name="p21075379172616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.55%" headers="mcps1.2.5.1.4 "><p id="p4976396172616"><a name="p4976396172616"></a><a name="p4976396172616"></a>待删除zone的ID。</p>
<p id="p1669018482183"><a name="p1669018482183"></a><a name="p1669018482183"></a>可以通过<a href="查询内网Zone列表.md">查询内网Zone列表</a>获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section44958995161021"></a>

-   请求参数

    无

-   请求样例

    删除Zone ID为“ff8080825b8fc86c015b94bc6f8712c3”的域名。

    ```
    DELETE https://{DNS_Endpoint}/v2/zones/ff8080825b8fc86c015b94bc6f8712c3
    ```


## 响应<a name="section40090803161031"></a>

-   要素说明

    **表 2**  响应样例的要素说明

    <a name="table28510837181412"></a>
    <table><thead align="left"><tr id="r09b8e694666c45eb908fe31b487e92df"><th class="cellrowborder" valign="top" width="18.38%" id="mcps1.2.4.1.1"><p id="a9319797f9c7c4d68bc6ce811d54034ce"><a name="a9319797f9c7c4d68bc6ce811d54034ce"></a><a name="a9319797f9c7c4d68bc6ce811d54034ce"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.33%" id="mcps1.2.4.1.2"><p id="a90c934462eca4cda911ab28b54639489"><a name="a90c934462eca4cda911ab28b54639489"></a><a name="a90c934462eca4cda911ab28b54639489"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.29%" id="mcps1.2.4.1.3"><p id="a6c16934552484e6ba07b23f8bedcb388"><a name="a6c16934552484e6ba07b23f8bedcb388"></a><a name="a6c16934552484e6ba07b23f8bedcb388"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="rd2d27ac0d78d4e7496661d08ba127228"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="ac9dbb7a783d14d7c96a615de8798da87"><a name="ac9dbb7a783d14d7c96a615de8798da87"></a><a name="ac9dbb7a783d14d7c96a615de8798da87"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="a7e2f323d67054a42903b158e88d38267"><a name="a7e2f323d67054a42903b158e88d38267"></a><a name="a7e2f323d67054a42903b158e88d38267"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="ad67b37f588024f7182275050763cdcc5"><a name="ad67b37f588024f7182275050763cdcc5"></a><a name="ad67b37f588024f7182275050763cdcc5"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="r85b9d70aab8e410da5ee66f83e5bac5f"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="aacbfb17ef9ca45a99a97d2930519655d"><a name="aacbfb17ef9ca45a99a97d2930519655d"></a><a name="aacbfb17ef9ca45a99a97d2930519655d"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="a4d7e73845b2a4cfaaa98212cdd899413"><a name="a4d7e73845b2a4cfaaa98212cdd899413"></a><a name="a4d7e73845b2a4cfaaa98212cdd899413"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="a707105b5caa74033878b6560267c8d57"><a name="a707105b5caa74033878b6560267c8d57"></a><a name="a707105b5caa74033878b6560267c8d57"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="rd05b997d56554cd28efecc8d7d051455"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="aa3d91e099bac49b6933fdab2040ec026"><a name="aa3d91e099bac49b6933fdab2040ec026"></a><a name="aa3d91e099bac49b6933fdab2040ec026"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="a0b9881b54bc34f5481424db86386c39e"><a name="a0b9881b54bc34f5481424db86386c39e"></a><a name="a0b9881b54bc34f5481424db86386c39e"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="ad78401d7d1204d1387f6a557227d28a9"><a name="ad78401d7d1204d1387f6a557227d28a9"></a><a name="ad78401d7d1204d1387f6a557227d28a9"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="r99f1e75b11c94a549334ba75082b267b"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="ac7366ab62f2e480fbf7c21f96812a419"><a name="ac7366ab62f2e480fbf7c21f96812a419"></a><a name="ac7366ab62f2e480fbf7c21f96812a419"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="ae250b65cce6d423db9e2ee74813110a6"><a name="ae250b65cce6d423db9e2ee74813110a6"></a><a name="ae250b65cce6d423db9e2ee74813110a6"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="a56b6c6f549fa424db93fa4b49fc59dac"><a name="a56b6c6f549fa424db93fa4b49fc59dac"></a><a name="a56b6c6f549fa424db93fa4b49fc59dac"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="r735c2bc4d7354822b2f4cf82ef6aabd8"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="ab4d9fe8455c54e68862095b89e5c532d"><a name="ab4d9fe8455c54e68862095b89e5c532d"></a><a name="ab4d9fe8455c54e68862095b89e5c532d"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="a5ca4b7dd58e848abbb4205197012eac8"><a name="a5ca4b7dd58e848abbb4205197012eac8"></a><a name="a5ca4b7dd58e848abbb4205197012eac8"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p9394279212"><a name="p9394279212"></a><a name="p9394279212"></a>zone类型，公网（public）或者内网（private）。</p>
    </td>
    </tr>
    <tr id="r48f49babd1294b0caf5e735e131e1e1b"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="a6a622ccc5ae048779a0d3b6f2d724487"><a name="a6a622ccc5ae048779a0d3b6f2d724487"></a><a name="a6a622ccc5ae048779a0d3b6f2d724487"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="af2c74817f72741c2abd84000928337ba"><a name="af2c74817f72741c2abd84000928337ba"></a><a name="af2c74817f72741c2abd84000928337ba"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="af2e3122536274be8914d68cb48be3270"><a name="af2e3122536274be8914d68cb48be3270"></a><a name="af2e3122536274be8914d68cb48be3270"></a>该zone下SOA记录中的ttl值。</p>
    <p id="p0662131993410"><a name="p0662131993410"></a><a name="p0662131993410"></a>取值范围：300~2147483647</p>
    <p id="p7662111973418"><a name="p7662111973418"></a><a name="p7662111973418"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="ra00af971198943759d302cccc963e19e"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="a4379ecac2b5b413cb94e9e630a818f6e"><a name="a4379ecac2b5b413cb94e9e630a818f6e"></a><a name="a4379ecac2b5b413cb94e9e630a818f6e"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="ab68af0f690844bed8260846a8110fc7a"><a name="ab68af0f690844bed8260846a8110fc7a"></a><a name="ab68af0f690844bed8260846a8110fc7a"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p201115484116"><a name="p201115484116"></a><a name="p201115484116"></a>该zone下SOA记录中用于标识zone文件变更的序列值，用于主从节点同步。</p>
    <p id="p7524749171039"><a name="p7524749171039"></a><a name="p7524749171039"></a>该参数暂未使用。</p>
    </td>
    </tr>
    <tr id="r1c654d0f11df4bf0a5e96d6ea43472d2"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="a3fc3a842bf264c2a90d71bbbd7c6ab5d"><a name="a3fc3a842bf264c2a90d71bbbd7c6ab5d"></a><a name="a3fc3a842bf264c2a90d71bbbd7c6ab5d"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="a50d50fea604b4a7f9d3e9b666e69ceae"><a name="a50d50fea604b4a7f9d3e9b666e69ceae"></a><a name="a50d50fea604b4a7f9d3e9b666e69ceae"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="ac769d3529e8f4084bab8b6cb478fe200"><a name="ac769d3529e8f4084bab8b6cb478fe200"></a><a name="ac769d3529e8f4084bab8b6cb478fe200"></a>资源状态。</p>
    <p id="zh-cn_topic_0057311028_p186242108156"><a name="zh-cn_topic_0057311028_p186242108156"></a><a name="zh-cn_topic_0057311028_p186242108156"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="r57aea8cab7474da9bb4855744708f6f2"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="aa276a9323f454ff4ad8d0ebf1b989a49"><a name="aa276a9323f454ff4ad8d0ebf1b989a49"></a><a name="aa276a9323f454ff4ad8d0ebf1b989a49"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p252886123415"><a name="zh-cn_topic_0057311028_p252886123415"></a><a name="zh-cn_topic_0057311028_p252886123415"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="aebe806e4aba34b03aa797faad3db724c"><a name="aebe806e4aba34b03aa797faad3db724c"></a><a name="aebe806e4aba34b03aa797faad3db724c"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="r348d946027fd4935b763bcc9ea42f2a9"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="a5e3792ce45c64cbea686d758458a1946"><a name="a5e3792ce45c64cbea686d758458a1946"></a><a name="a5e3792ce45c64cbea686d758458a1946"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="aab64c548680e4dca9265ab2cf4da8fe3"><a name="aab64c548680e4dca9265ab2cf4da8fe3"></a><a name="aab64c548680e4dca9265ab2cf4da8fe3"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="a4bb2ef658ca342a8b459ad95ae4d0297"><a name="a4bb2ef658ca342a8b459ad95ae4d0297"></a><a name="a4bb2ef658ca342a8b459ad95ae4d0297"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="r25cff7b344724a7aac622926d7a38974"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="a8d3fbade5362424e848bbb8a5c6bf8c4"><a name="a8d3fbade5362424e848bbb8a5c6bf8c4"></a><a name="a8d3fbade5362424e848bbb8a5c6bf8c4"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="a08c140632a0e4ae9805386978f795c88"><a name="a08c140632a0e4ae9805386978f795c88"></a><a name="a08c140632a0e4ae9805386978f795c88"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="aed5627a5e7ff417eab7b19bad2e0abd3"><a name="aed5627a5e7ff417eab7b19bad2e0abd3"></a><a name="aed5627a5e7ff417eab7b19bad2e0abd3"></a>zone所属的项目ID。</p>
    </td>
    </tr>
    <tr id="rd1d3f0bf80a34e168097e9e6f50baa5d"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="ad843f00078994b1f8ab1f00c717a1313"><a name="ad843f00078994b1f8ab1f00c717a1313"></a><a name="ad843f00078994b1f8ab1f00c717a1313"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="a865ba28ed9694d8a9f7222ddc64ac270"><a name="a865ba28ed9694d8a9f7222ddc64ac270"></a><a name="a865ba28ed9694d8a9f7222ddc64ac270"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="acd1a824892924ba080165e3eebcaa625"><a name="acd1a824892924ba080165e3eebcaa625"></a><a name="acd1a824892924ba080165e3eebcaa625"></a>创建时间。</p>
    <p id="p583516468316"><a name="p583516468316"></a><a name="p583516468316"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="rf36129b6c1144868b41c28bc6c9c957c"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="a373ea4a89f8a4e7281c47f0ebe2859bd"><a name="a373ea4a89f8a4e7281c47f0ebe2859bd"></a><a name="a373ea4a89f8a4e7281c47f0ebe2859bd"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="a42c304a0fdcc404ebeb6960101eb5991"><a name="a42c304a0fdcc404ebeb6960101eb5991"></a><a name="a42c304a0fdcc404ebeb6960101eb5991"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="aaef7e595fc1e4e2c89f404a691b5fb48"><a name="aaef7e595fc1e4e2c89f404a691b5fb48"></a><a name="aaef7e595fc1e4e2c89f404a691b5fb48"></a>更新时间。</p>
    <p id="a1cb952018c5e4d6ca060703f4d2b0e8f"><a name="a1cb952018c5e4d6ca060703f4d2b0e8f"></a><a name="a1cb952018c5e4d6ca060703f4d2b0e8f"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="r33e863bac9d7497fb2883d57100a4334"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="a41def7ce09ec4c56b4834ba1f1e1e3c8"><a name="a41def7ce09ec4c56b4834ba1f1e1e3c8"></a><a name="a41def7ce09ec4c56b4834ba1f1e1e3c8"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="a936de5899d714ff8bad947d990573d16"><a name="a936de5899d714ff8bad947d990573d16"></a><a name="a936de5899d714ff8bad947d990573d16"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="a9f64ab6d947b4b1fb4302b22dfbf5f43"><a name="a9f64ab6d947b4b1fb4302b22dfbf5f43"></a><a name="a9f64ab6d947b4b1fb4302b22dfbf5f43"></a>指向当前资源或者其他资源的链接。</p>
    <p id="a592d9d56c5a5494bb4f91667a042a40e"><a name="a592d9d56c5a5494bb4f91667a042a40e"></a><a name="a592d9d56c5a5494bb4f91667a042a40e"></a>当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p946815102468"><a name="p946815102468"></a><a name="p946815102468"></a>详细信息请参见<a href="#table52442344175457">表3</a>。</p>
    </td>
    </tr>
    <tr id="re0c1a336d78e476e9a92af4699cd15f6"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="afa4e8d609031485988fbbb1110017770"><a name="afa4e8d609031485988fbbb1110017770"></a><a name="afa4e8d609031485988fbbb1110017770"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p1926195132219"><a name="p1926195132219"></a><a name="p1926195132219"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="aa6945a0932194e7d96b63a9cd5fbf016"><a name="aa6945a0932194e7d96b63a9cd5fbf016"></a><a name="aa6945a0932194e7d96b63a9cd5fbf016"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    <p id="zh-cn_topic_0057311028_p376119772512"><a name="zh-cn_topic_0057311028_p376119772512"></a><a name="zh-cn_topic_0057311028_p376119772512"></a>目前暂未使用。</p>
    </td>
    </tr>
    <tr id="r54c70c563ba7448dac6b1af69f74ea78"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="a6a1a1c3445ea4d0da40f1d6c10bd0e77"><a name="a6a1a1c3445ea4d0da40f1d6c10bd0e77"></a><a name="a6a1a1c3445ea4d0da40f1d6c10bd0e77"></a>routers</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="a782bdeb1040b4a44aa0e86848b06d6a5"><a name="a782bdeb1040b4a44aa0e86848b06d6a5"></a><a name="a782bdeb1040b4a44aa0e86848b06d6a5"></a>Array of object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="a156b4435a50b49628fc39c7721779bf9"><a name="a156b4435a50b49628fc39c7721779bf9"></a><a name="a156b4435a50b49628fc39c7721779bf9"></a>与该zone关联的Router(VPC)列表。详细信息请参见<a href="#table4448008117179">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  links参数说明

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
    <tr id="row152946184813"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.591959195919593%" headers="mcps1.2.4.1.2 "><p id="p19656144517367"><a name="p19656144517367"></a><a name="p19656144517367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.10621062106211%" headers="mcps1.2.4.1.3 "><p id="p76567451365"><a name="p76567451365"></a><a name="p76567451365"></a>下一页资源的链接。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  routers对象参数说明

    <a name="table4448008117179"></a>
    <table><thead align="left"><tr id="row6132935617179"><th class="cellrowborder" valign="top" width="18.538146185381464%" id="mcps1.2.4.1.1"><p id="p36588677171719"><a name="p36588677171719"></a><a name="p36588677171719"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.708029197080293%" id="mcps1.2.4.1.2"><p id="p9906869171719"><a name="p9906869171719"></a><a name="p9906869171719"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="61.75382461753826%" id="mcps1.2.4.1.3"><p id="p64258954171719"><a name="p64258954171719"></a><a name="p64258954171719"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1024510342619"><td class="cellrowborder" valign="top" width="18.538146185381464%" headers="mcps1.2.4.1.1 "><p id="p38120631175524"><a name="p38120631175524"></a><a name="p38120631175524"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.708029197080293%" headers="mcps1.2.4.1.2 "><p id="p57184665175519"><a name="p57184665175519"></a><a name="p57184665175519"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.75382461753826%" headers="mcps1.2.4.1.3 "><p id="p1635999216648"><a name="p1635999216648"></a><a name="p1635999216648"></a>资源状态。</p>
    <p id="p656495918714"><a name="p656495918714"></a><a name="p656495918714"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="row266872817179"><td class="cellrowborder" valign="top" width="18.538146185381464%" headers="mcps1.2.4.1.1 "><p id="p25118582171719"><a name="p25118582171719"></a><a name="p25118582171719"></a>router_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.708029197080293%" headers="mcps1.2.4.1.2 "><p id="p50755907171719"><a name="p50755907171719"></a><a name="p50755907171719"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.75382461753826%" headers="mcps1.2.4.1.3 "><p id="p17587794171719"><a name="p17587794171719"></a><a name="p17587794171719"></a>Router(VPC)所属VPC的ID。</p>
    <p id="p143411822947"><a name="p143411822947"></a><a name="p143411822947"></a>该参数的值可以通过如下两种方式获取：</p>
    <a name="ul1938314911411"></a><a name="ul1938314911411"></a><ul id="ul1938314911411"><li>通过虚拟私有云的管理控制台，在VPC的详情页面中获取VPC的ID。</li><li>通过<a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0003.html" target="_blank" rel="noopener noreferrer">查询VPC列表</a>获取VPC ID。</li></ul>
    </td>
    </tr>
    <tr id="row6657832817179"><td class="cellrowborder" valign="top" width="18.538146185381464%" headers="mcps1.2.4.1.1 "><p id="p3709384171719"><a name="p3709384171719"></a><a name="p3709384171719"></a>router_region</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.708029197080293%" headers="mcps1.2.4.1.2 "><p id="p43861924171719"><a name="p43861924171719"></a><a name="p43861924171719"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.75382461753826%" headers="mcps1.2.4.1.3 "><p id="p63154928171719"><a name="p63154928171719"></a><a name="p63154928171719"></a>Router(VPC)所在的region。</p>
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
        "status": "PENDING_DELETE",
        "links": {
            "self": "https://Endpoint/v2/zones/ff8080825b8fc86c015b94bc6f8712c3"
        },
        "pool_id": "ff8080825ab738f4015ab7513298010e",
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
        "zone_type": "private",
        "created_at": "2017-04-22T10:05:23.110",
        "updated_at": "2017-04-22T10:05:23.959",
        "record_num": 0,
        "routers": [
            {
                "status": "ACTIVE",
                "router_id": "19664294-0bf6-4271-ad3a-94b8c79c6558",
                "router_region": "xx"
            },
            {
                "status": "ACTIVE",
                "router_id": "f0791650-db8c-4a20-8a44-a06c6e24b15b",
                "router_region": "xx"
            }
        ]
    }
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

