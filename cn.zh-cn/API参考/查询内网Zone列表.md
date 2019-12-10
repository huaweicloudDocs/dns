# 查询内网Zone列表<a name="zh-cn_topic_0057311029"></a>

## 功能介绍<a name="section2763065016101"></a>

查询内网Zone的列表。

## URI<a name="section53701671161015"></a>

GET /v2/zones?type=\{type\}&limit=\{limit\}&marker=\{marker\}&offset=\{offset\}&tags=\{tags\}&name=\{name\}

参数说明请参见[表1](#table36421405182556)。

**表 1**  URI格式的参数说明

<a name="table36421405182556"></a>
<table><thead align="left"><tr id="row35113810182556"><th class="cellrowborder" valign="top" width="10.89%" id="mcps1.2.5.1.1"><p id="p29205341182624"><a name="p29205341182624"></a><a name="p29205341182624"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.740000000000004%" id="mcps1.2.5.1.2"><p id="p16822416182624"><a name="p16822416182624"></a><a name="p16822416182624"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.350000000000001%" id="mcps1.2.5.1.3"><p id="p20438464182624"><a name="p20438464182624"></a><a name="p20438464182624"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="59.02%" id="mcps1.2.5.1.4"><p id="p44902868182624"><a name="p44902868182624"></a><a name="p44902868182624"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7883687182556"><td class="cellrowborder" valign="top" width="10.89%" headers="mcps1.2.5.1.1 "><p id="p29178851182717"><a name="p29178851182717"></a><a name="p29178851182717"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="15.740000000000004%" headers="mcps1.2.5.1.2 "><p id="p2590622182717"><a name="p2590622182717"></a><a name="p2590622182717"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.350000000000001%" headers="mcps1.2.5.1.3 "><p id="p66359104182717"><a name="p66359104182717"></a><a name="p66359104182717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59.02%" headers="mcps1.2.5.1.4 "><p id="p41213064154029"><a name="p41213064154029"></a><a name="p41213064154029"></a>待查询的zone的类型。</p>
<p id="p35373258154029"><a name="p35373258154029"></a><a name="p35373258154029"></a>取值范围：private</p>
<p id="p426025714343"><a name="p426025714343"></a><a name="p426025714343"></a>表示查询内网类型的zone。</p>
</td>
</tr>
<tr id="row12208459182556"><td class="cellrowborder" valign="top" width="10.89%" headers="mcps1.2.5.1.1 "><p id="p17456213182720"><a name="p17456213182720"></a><a name="p17456213182720"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="15.740000000000004%" headers="mcps1.2.5.1.2 "><p id="p4667185182720"><a name="p4667185182720"></a><a name="p4667185182720"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.350000000000001%" headers="mcps1.2.5.1.3 "><p id="p42497672182720"><a name="p42497672182720"></a><a name="p42497672182720"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59.02%" headers="mcps1.2.5.1.4 "><p id="p352216816854"><a name="p352216816854"></a><a name="p352216816854"></a>分页查询起始的资源ID。</p>
<p id="p19759428182720"><a name="p19759428182720"></a><a name="p19759428182720"></a>如果为空，表示查询第一页。</p>
<p id="p1451994172211"><a name="p1451994172211"></a><a name="p1451994172211"></a>默认值为空。</p>
</td>
</tr>
<tr id="row29489517182630"><td class="cellrowborder" valign="top" width="10.89%" headers="mcps1.2.5.1.1 "><p id="p43326778182720"><a name="p43326778182720"></a><a name="p43326778182720"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="15.740000000000004%" headers="mcps1.2.5.1.2 "><p id="p19808096182720"><a name="p19808096182720"></a><a name="p19808096182720"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.350000000000001%" headers="mcps1.2.5.1.3 "><p id="p60951943182720"><a name="p60951943182720"></a><a name="p60951943182720"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59.02%" headers="mcps1.2.5.1.4 "><p id="p230120311413"><a name="p230120311413"></a><a name="p230120311413"></a>每页返回的资源个数。</p>
<p id="p147131447514"><a name="p147131447514"></a><a name="p147131447514"></a>取值范围：0~500</p>
<p id="p1385813431412"><a name="p1385813431412"></a><a name="p1385813431412"></a>取值一般为10，20，50。默认值为500。</p>
</td>
</tr>
<tr id="row2721615319547"><td class="cellrowborder" valign="top" width="10.89%" headers="mcps1.2.5.1.1 "><p id="p626980719549"><a name="p626980719549"></a><a name="p626980719549"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="15.740000000000004%" headers="mcps1.2.5.1.2 "><p id="p3809236019549"><a name="p3809236019549"></a><a name="p3809236019549"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.350000000000001%" headers="mcps1.2.5.1.3 "><p id="p6558235419549"><a name="p6558235419549"></a><a name="p6558235419549"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="59.02%" headers="mcps1.2.5.1.4 "><p id="p35951433204916"><a name="p35951433204916"></a><a name="p35951433204916"></a>分页查询起始偏移量，表示从偏移量的下一个资源开始查询。</p>
<p id="p18898143914915"><a name="p18898143914915"></a><a name="p18898143914915"></a>取值范围：0~2147483647</p>
<p id="p13209172234718"><a name="p13209172234718"></a><a name="p13209172234718"></a>默认值为0。</p>
<p id="p167712216335"><a name="p167712216335"></a><a name="p167712216335"></a>当前设置marker不为空时，以marker为分页起始标识。</p>
</td>
</tr>
<tr id="row58681680125046"><td class="cellrowborder" valign="top" width="10.89%" headers="mcps1.2.5.1.1 "><p id="p47666033125046"><a name="p47666033125046"></a><a name="p47666033125046"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="15.740000000000004%" headers="mcps1.2.5.1.2 "><p id="p35743447125046"><a name="p35743447125046"></a><a name="p35743447125046"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.350000000000001%" headers="mcps1.2.5.1.3 "><p id="p9538131125046"><a name="p9538131125046"></a><a name="p9538131125046"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59.02%" headers="mcps1.2.5.1.4 "><p id="p34391114125046"><a name="p34391114125046"></a><a name="p34391114125046"></a>资源标签。</p>
<p id="p41084576125046"><a name="p41084576125046"></a><a name="p41084576125046"></a>取值格式：key1,value1|key2,value2</p>
<p id="p34216870125046"><a name="p34216870125046"></a><a name="p34216870125046"></a>多个标签之间用"|"分开，每个标签的键值用英文逗号","相隔。</p>
<p id="p1526014454308"><a name="p1526014454308"></a><a name="p1526014454308"></a>多个标签之间为“与”的关系。</p>
<p id="p16628284115121"><a name="p16628284115121"></a><a name="p16628284115121"></a>关于资源标签，请参见<a href="添加资源标签.md">添加资源标签</a>。</p>
<p id="p116996555212"><a name="p116996555212"></a><a name="p116996555212"></a>默认值为空。</p>
</td>
</tr>
<tr id="row7779132921"><td class="cellrowborder" valign="top" width="10.89%" headers="mcps1.2.5.1.1 "><p id="p1933113222124"><a name="p1933113222124"></a><a name="p1933113222124"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="15.740000000000004%" headers="mcps1.2.5.1.2 "><p id="p1833110221120"><a name="p1833110221120"></a><a name="p1833110221120"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.350000000000001%" headers="mcps1.2.5.1.3 "><p id="p1533162211129"><a name="p1533162211129"></a><a name="p1533162211129"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59.02%" headers="mcps1.2.5.1.4 "><p id="p113313225126"><a name="p113313225126"></a><a name="p113313225126"></a>zone名称。</p>
<p id="p159771524568"><a name="p159771524568"></a><a name="p159771524568"></a>搜索模式默认为模糊搜索。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section44958995161021"></a>

-   请求参数

    无

-   请求样例

    查询域名类型为内网，且资源标签键为key1、值为value1的前10个域名。

    ```
    GET https://{DNS_Endpoint}/v2/zones?type=private&limit=10&offset=0&tags=key1,value1
    ```


## 响应<a name="section40090803161031"></a>

-   要素说明

    **表 2**  响应样例的要素说明

    <a name="table6655637171923"></a>
    <table><thead align="left"><tr id="row12436182171923"><th class="cellrowborder" valign="top" width="18.41%" id="mcps1.2.4.1.1"><p id="p18040723171923"><a name="p18040723171923"></a><a name="p18040723171923"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.1%" id="mcps1.2.4.1.2"><p id="p12288867171923"><a name="p12288867171923"></a><a name="p12288867171923"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.49%" id="mcps1.2.4.1.3"><p id="p16021685171923"><a name="p16021685171923"></a><a name="p16021685171923"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row14234124965913"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p121914507594"><a name="p121914507594"></a><a name="p121914507594"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.1%" headers="mcps1.2.4.1.2 "><p id="p119265015599"><a name="p119265015599"></a><a name="p119265015599"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.49%" headers="mcps1.2.4.1.3 "><p id="p2192145010591"><a name="p2192145010591"></a><a name="p2192145010591"></a>指向当前资源或者其他资源的链接。</p>
    <p id="p1419219504593"><a name="p1419219504593"></a><a name="p1419219504593"></a>当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p1619213506597"><a name="p1619213506597"></a><a name="p1619213506597"></a>详细信息请参见<a href="#table0172144213344">表5</a>。</p>
    </td>
    </tr>
    <tr id="row33084878171923"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p10518479171923"><a name="p10518479171923"></a><a name="p10518479171923"></a>zones</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.1%" headers="mcps1.2.4.1.2 "><p id="p17816324171923"><a name="p17816324171923"></a><a name="p17816324171923"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.49%" headers="mcps1.2.4.1.3 "><p id="p64387025171923"><a name="p64387025171923"></a><a name="p64387025171923"></a>zone列表对象，详细内容请参见<a href="#table10871190151410">表3</a>。</p>
    </td>
    </tr>
    <tr id="row45921614175143"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p10641344175143"><a name="p10641344175143"></a><a name="p10641344175143"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.1%" headers="mcps1.2.4.1.2 "><p id="p24643947175143"><a name="p24643947175143"></a><a name="p24643947175143"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.49%" headers="mcps1.2.4.1.3 "><p id="p50002691175143"><a name="p50002691175143"></a><a name="p50002691175143"></a>返回满足过滤条件的资源总数，详细内容请参见<a href="#table141615131414">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  zones参数说明

    <a name="table10871190151410"></a>
    <table><thead align="left"><tr id="row1187914015145"><th class="cellrowborder" valign="top" width="18.38%" id="mcps1.2.4.1.1"><p id="p488213014145"><a name="p488213014145"></a><a name="p488213014145"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.33%" id="mcps1.2.4.1.2"><p id="p1388515051418"><a name="p1388515051418"></a><a name="p1388515051418"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.29%" id="mcps1.2.4.1.3"><p id="p8887707143"><a name="p8887707143"></a><a name="p8887707143"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row14889200191410"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p11890180121420"><a name="p11890180121420"></a><a name="p11890180121420"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p178921305144"><a name="p178921305144"></a><a name="p178921305144"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p1589419081418"><a name="p1589419081418"></a><a name="p1589419081418"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="row208952016144"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p198981207149"><a name="p198981207149"></a><a name="p198981207149"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p0901205148"><a name="p0901205148"></a><a name="p0901205148"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p5904140161420"><a name="p5904140161420"></a><a name="p5904140161420"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="row1905180111413"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p129067010142"><a name="p129067010142"></a><a name="p129067010142"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p1890800161415"><a name="p1890800161415"></a><a name="p1890800161415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p790916010141"><a name="p790916010141"></a><a name="p790916010141"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="row89101018143"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p791270191413"><a name="p791270191413"></a><a name="p791270191413"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p09136021413"><a name="p09136021413"></a><a name="p09136021413"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p791613013147"><a name="p791613013147"></a><a name="p791613013147"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="row69166031414"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p179190018143"><a name="p179190018143"></a><a name="p179190018143"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p292119018147"><a name="p292119018147"></a><a name="p292119018147"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p9394279212"><a name="p9394279212"></a><a name="p9394279212"></a>zone类型，公网（public）或者内网（private）。</p>
    </td>
    </tr>
    <tr id="row1792616091413"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p109283011142"><a name="p109283011142"></a><a name="p109283011142"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p189301209147"><a name="p189301209147"></a><a name="p189301209147"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p1893460141411"><a name="p1893460141411"></a><a name="p1893460141411"></a>该zone下SOA记录中的ttl值。</p>
    </td>
    </tr>
    <tr id="row49346041419"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p193630171412"><a name="p193630171412"></a><a name="p193630171412"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p19940160111416"><a name="p19940160111416"></a><a name="p19940160111416"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p201115484116"><a name="p201115484116"></a><a name="p201115484116"></a>该zone下SOA记录中用于标识zone文件变更的序列值，用于主从节点同步。</p>
    <p id="p7524749171039"><a name="p7524749171039"></a><a name="p7524749171039"></a>该参数暂未使用。</p>
    </td>
    </tr>
    <tr id="row1494311013144"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p1394519012141"><a name="p1394519012141"></a><a name="p1394519012141"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p199461401144"><a name="p199461401144"></a><a name="p199461401144"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p494720017143"><a name="p494720017143"></a><a name="p494720017143"></a>资源状态。</p>
    <p id="p17698116181717"><a name="p17698116181717"></a><a name="p17698116181717"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="row1595113017149"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p1395410081413"><a name="p1395410081413"></a><a name="p1395410081413"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p179551801147"><a name="p179551801147"></a><a name="p179551801147"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p595712021413"><a name="p595712021413"></a><a name="p595712021413"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="row69595020143"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p15962150151419"><a name="p15962150151419"></a><a name="p15962150151419"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p6965803142"><a name="p6965803142"></a><a name="p6965803142"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p1596710031411"><a name="p1596710031411"></a><a name="p1596710031411"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="row49683010141"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p2097010181418"><a name="p2097010181418"></a><a name="p2097010181418"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p1397430121412"><a name="p1397430121412"></a><a name="p1397430121412"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p8704812171039"><a name="p8704812171039"></a><a name="p8704812171039"></a>zone所属的项目ID。</p>
    </td>
    </tr>
    <tr id="row129774031419"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p15980200171419"><a name="p15980200171419"></a><a name="p15980200171419"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p69816019146"><a name="p69816019146"></a><a name="p69816019146"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p159835018143"><a name="p159835018143"></a><a name="p159835018143"></a>创建时间。</p>
    <p id="p583516468316"><a name="p583516468316"></a><a name="p583516468316"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="row1498413011412"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p398715081417"><a name="p398715081417"></a><a name="p398715081417"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p1988190121420"><a name="p1988190121420"></a><a name="p1988190121420"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p169905051413"><a name="p169905051413"></a><a name="p169905051413"></a>更新时间。</p>
    <p id="p1133918273234"><a name="p1133918273234"></a><a name="p1133918273234"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="row999050111419"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p8993407142"><a name="p8993407142"></a><a name="p8993407142"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p899518011417"><a name="p899518011417"></a><a name="p899518011417"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p1799719041413"><a name="p1799719041413"></a><a name="p1799719041413"></a>指向当前资源或者其他资源的链接。</p>
    <p id="p109986017142"><a name="p109986017142"></a><a name="p109986017142"></a>当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p8722659124511"><a name="p8722659124511"></a><a name="p8722659124511"></a>详细信息请参见<a href="#table0172144213344">表5</a>。</p>
    </td>
    </tr>
    <tr id="row29991001416"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p1311419142"><a name="p1311419142"></a><a name="p1311419142"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p9449603510"><a name="p9449603510"></a><a name="p9449603510"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p1876191410"><a name="p1876191410"></a><a name="p1876191410"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    <p id="p14810145782211"><a name="p14810145782211"></a><a name="p14810145782211"></a>目前暂未使用。</p>
    </td>
    </tr>
    <tr id="row18881161418"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p6114111411"><a name="p6114111411"></a><a name="p6114111411"></a>routers</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p10131212146"><a name="p10131212146"></a><a name="p10131212146"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p161561141410"><a name="p161561141410"></a><a name="p161561141410"></a>与该zone关联的Router(VPC)列表。详细信息请参见<a href="#table4448008117179">表6</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  metadata参数说明

    <a name="table141615131414"></a>
    <table><thead align="left"><tr id="row223813147"><th class="cellrowborder" valign="top" width="18.13181318131813%" id="mcps1.2.4.1.1"><p id="p1266151412"><a name="p1266151412"></a><a name="p1266151412"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.46194619461946%" id="mcps1.2.4.1.2"><p id="p12286121410"><a name="p12286121410"></a><a name="p12286121410"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.406240624062406%" id="mcps1.2.4.1.3"><p id="p02911119140"><a name="p02911119140"></a><a name="p02911119140"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row33219131412"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.4.1.1 "><p id="p8341314143"><a name="p8341314143"></a><a name="p8341314143"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46194619461946%" headers="mcps1.2.4.1.2 "><p id="p123671111420"><a name="p123671111420"></a><a name="p123671111420"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.406240624062406%" headers="mcps1.2.4.1.3 "><p id="p1339111149"><a name="p1339111149"></a><a name="p1339111149"></a>满足查询条件的资源总数，不受分页（即limit、offset参数）影响。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  links参数说明

    <a name="table0172144213344"></a>
    <table><thead align="left"><tr id="row917304253418"><th class="cellrowborder" valign="top" width="18.13181318131813%" id="mcps1.2.4.1.1"><p id="p101731742153416"><a name="p101731742153416"></a><a name="p101731742153416"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.77197719771977%" id="mcps1.2.4.1.2"><p id="p0174542163418"><a name="p0174542163418"></a><a name="p0174542163418"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.09620962096209%" id="mcps1.2.4.1.3"><p id="p7174194243414"><a name="p7174194243414"></a><a name="p7174194243414"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1917494211345"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.4.1.1 "><p id="p13174134215348"><a name="p13174134215348"></a><a name="p13174134215348"></a>self</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77197719771977%" headers="mcps1.2.4.1.2 "><p id="p181741642173417"><a name="p181741642173417"></a><a name="p181741642173417"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.09620962096209%" headers="mcps1.2.4.1.3 "><p id="p1017434223419"><a name="p1017434223419"></a><a name="p1017434223419"></a>当前资源的链接。</p>
    </td>
    </tr>
    <tr id="row7655245133611"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77197719771977%" headers="mcps1.2.4.1.2 "><p id="p19656144517367"><a name="p19656144517367"></a><a name="p19656144517367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.09620962096209%" headers="mcps1.2.4.1.3 "><p id="p76567451365"><a name="p76567451365"></a><a name="p76567451365"></a>下一页资源的链接。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  router对象参数说明

    <a name="table4448008117179"></a>
    <table><thead align="left"><tr id="row6132935617179"><th class="cellrowborder" valign="top" width="18.32816718328167%" id="mcps1.2.4.1.1"><p id="p36588677171719"><a name="p36588677171719"></a><a name="p36588677171719"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.878012198780123%" id="mcps1.2.4.1.2"><p id="p9906869171719"><a name="p9906869171719"></a><a name="p9906869171719"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="61.79382061793821%" id="mcps1.2.4.1.3"><p id="p64258954171719"><a name="p64258954171719"></a><a name="p64258954171719"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1024510342619"><td class="cellrowborder" valign="top" width="18.32816718328167%" headers="mcps1.2.4.1.1 "><p id="p38120631175524"><a name="p38120631175524"></a><a name="p38120631175524"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.878012198780123%" headers="mcps1.2.4.1.2 "><p id="p57184665175519"><a name="p57184665175519"></a><a name="p57184665175519"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.79382061793821%" headers="mcps1.2.4.1.3 "><p id="p1635999216648"><a name="p1635999216648"></a><a name="p1635999216648"></a>资源状态。</p>
    <p id="p656495918714"><a name="p656495918714"></a><a name="p656495918714"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="row266872817179"><td class="cellrowborder" valign="top" width="18.32816718328167%" headers="mcps1.2.4.1.1 "><p id="p25118582171719"><a name="p25118582171719"></a><a name="p25118582171719"></a>router_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.878012198780123%" headers="mcps1.2.4.1.2 "><p id="p50755907171719"><a name="p50755907171719"></a><a name="p50755907171719"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.79382061793821%" headers="mcps1.2.4.1.3 "><p id="p17587794171719"><a name="p17587794171719"></a><a name="p17587794171719"></a>Router(VPC)所属VPC的ID。</p>
    <p id="p143411822947"><a name="p143411822947"></a><a name="p143411822947"></a>该参数的值可以通过如下两种方式获取：</p>
    <a name="ul1938314911411"></a><a name="ul1938314911411"></a><ul id="ul1938314911411"><li>通过虚拟私有云的管理控制台，在VPC的详情页面中获取VPC的ID。</li><li>通过<a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090625.html" target="_blank" rel="noopener noreferrer">查询VPC列表</a>获取VPC ID。</li></ul>
    </td>
    </tr>
    <tr id="row6657832817179"><td class="cellrowborder" valign="top" width="18.32816718328167%" headers="mcps1.2.4.1.1 "><p id="p3709384171719"><a name="p3709384171719"></a><a name="p3709384171719"></a>router_region</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.878012198780123%" headers="mcps1.2.4.1.2 "><p id="p43861924171719"><a name="p43861924171719"></a><a name="p43861924171719"></a>String</p>
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
        "links": {
            "self": "https://Endpoint/v2/zones?type=private&limit=11",
            "next": "https://Endpoint/v2/zones?type=private&limit=11&marker=ff8080825b8fc86c015b94bc6f8712c3"
        },
        "zones": [
            {
                "id": "ff8080825b8fc86c015b94bc6f8712c3",
                "name": "example.com.",
                "description": "This is an example zone.",
                "email": "xx@example.com",
                "ttl": 300,
                "serial": 0,
                "masters": [],
                "status": "ACTIVE",
                "links": {
                    "self": "https://Endpoint/v2/zones/ff8080825b8fc86c015b94bc6f8712c3"
                },
                "pool_id": "ff8080825ab738f4015ab7513298010e",
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
                "zone_type": "private",
                "created_at": "2017-04-22T08:17:08.997",
                "updated_at": "2017-04-22T08:17:09.997",
                "record_num": 2,
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
            },
            {
                "id": "ff8080825b95142f015b951f87280029",
                "name": "example.org.",
                "description": "This is an example zone.",
                "email": "xx@example.org",
                "ttl": 300,
                "serial": 0,
                "masters": [],
                "status": "ACTIVE",
                "links": {
                    "self": "https://Endpoint/v2/zones/ff8080825b95142f015b951f87280029"
                },
                "pool_id": "ff8080825ab738f4015ab7513298010e",
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
                "zone_type": "private",
                "created_at": "2017-04-22T08:17:08.997",
                "updated_at": "2017-04-22T08:17:09.997",
                "record_num": 2,
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
        ],
        "metadata": {
            "total_count": 2
        }
    }
    
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

