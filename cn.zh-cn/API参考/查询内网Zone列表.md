# 查询内网Zone列表<a name="ZH-CN_TOPIC_0057311029"></a>

## 功能介绍<a name="section2763065016101"></a>

查询内网Zone的列表。

## URI<a name="section53701671161015"></a>

GET /v2/zones?type=\{type\}&limit=\{limit\}&marker=\{marker\}&offset=\{offset\}&tags=\{tags\}

参数说明请参见[表1](#table36421405182556)。

**表 1**  URI格式的参数说明

<a name="table36421405182556"></a>
<table><thead align="left"><tr id="row35113810182556"><th class="cellrowborder" valign="top" width="10.900000000000002%" id="mcps1.2.5.1.1"><p id="p29205341182624"><a name="p29205341182624"></a><a name="p29205341182624"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.730000000000002%" id="mcps1.2.5.1.2"><p id="p16822416182624"><a name="p16822416182624"></a><a name="p16822416182624"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.350000000000001%" id="mcps1.2.5.1.3"><p id="p20438464182624"><a name="p20438464182624"></a><a name="p20438464182624"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="59.02%" id="mcps1.2.5.1.4"><p id="p44902868182624"><a name="p44902868182624"></a><a name="p44902868182624"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7883687182556"><td class="cellrowborder" valign="top" width="10.900000000000002%" headers="mcps1.2.5.1.1 "><p id="p29178851182717"><a name="p29178851182717"></a><a name="p29178851182717"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="15.730000000000002%" headers="mcps1.2.5.1.2 "><p id="p2590622182717"><a name="p2590622182717"></a><a name="p2590622182717"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.350000000000001%" headers="mcps1.2.5.1.3 "><p id="p66359104182717"><a name="p66359104182717"></a><a name="p66359104182717"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="59.02%" headers="mcps1.2.5.1.4 "><p id="p41213064154029"><a name="p41213064154029"></a><a name="p41213064154029"></a>待查询的zone的类型。</p>
<p id="p35373258154029"><a name="p35373258154029"></a><a name="p35373258154029"></a>取值范围：private</p>
<p id="p426025714343"><a name="p426025714343"></a><a name="p426025714343"></a>表示查询内网类型的zone。</p>
</td>
</tr>
<tr id="row12208459182556"><td class="cellrowborder" valign="top" width="10.900000000000002%" headers="mcps1.2.5.1.1 "><p id="p17456213182720"><a name="p17456213182720"></a><a name="p17456213182720"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="15.730000000000002%" headers="mcps1.2.5.1.2 "><p id="p4667185182720"><a name="p4667185182720"></a><a name="p4667185182720"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.350000000000001%" headers="mcps1.2.5.1.3 "><p id="p42497672182720"><a name="p42497672182720"></a><a name="p42497672182720"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="59.02%" headers="mcps1.2.5.1.4 "><p id="p352216816854"><a name="p352216816854"></a><a name="p352216816854"></a>分页查询起始的资源ID。</p>
<p id="p19759428182720"><a name="p19759428182720"></a><a name="p19759428182720"></a>如果为空，表示查询第一页。</p>
</td>
</tr>
<tr id="row29489517182630"><td class="cellrowborder" valign="top" width="10.900000000000002%" headers="mcps1.2.5.1.1 "><p id="p43326778182720"><a name="p43326778182720"></a><a name="p43326778182720"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="15.730000000000002%" headers="mcps1.2.5.1.2 "><p id="p19808096182720"><a name="p19808096182720"></a><a name="p19808096182720"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.350000000000001%" headers="mcps1.2.5.1.3 "><p id="p60951943182720"><a name="p60951943182720"></a><a name="p60951943182720"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="59.02%" headers="mcps1.2.5.1.4 "><a name="ul38160342182720"></a><a name="ul38160342182720"></a><ul id="ul38160342182720"><li>取值范围：0~500<p id="p3980022182720"><a name="p3980022182720"></a><a name="p3980022182720"></a>取值一般为10，20，50</p>
</li><li>功能说明：每页返回的资源个数。</li></ul>
</td>
</tr>
<tr id="row2721615319547"><td class="cellrowborder" valign="top" width="10.900000000000002%" headers="mcps1.2.5.1.1 "><p id="p626980719549"><a name="p626980719549"></a><a name="p626980719549"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="15.730000000000002%" headers="mcps1.2.5.1.2 "><p id="p3809236019549"><a name="p3809236019549"></a><a name="p3809236019549"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.350000000000001%" headers="mcps1.2.5.1.3 "><p id="p6558235419549"><a name="p6558235419549"></a><a name="p6558235419549"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="59.02%" headers="mcps1.2.5.1.4 "><a name="ul1057048519549"></a><a name="ul1057048519549"></a><ul id="ul1057048519549"><li>取值范围：0~2147483647</li><li>分页查询起始页码，起始值为0。当前设置marker不为空时，以marker为分页起始标识。</li></ul>
</td>
</tr>
<tr id="row58681680125046"><td class="cellrowborder" valign="top" width="10.900000000000002%" headers="mcps1.2.5.1.1 "><p id="p47666033125046"><a name="p47666033125046"></a><a name="p47666033125046"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="15.730000000000002%" headers="mcps1.2.5.1.2 "><p id="p35743447125046"><a name="p35743447125046"></a><a name="p35743447125046"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.350000000000001%" headers="mcps1.2.5.1.3 "><p id="p9538131125046"><a name="p9538131125046"></a><a name="p9538131125046"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="59.02%" headers="mcps1.2.5.1.4 "><p id="p34391114125046"><a name="p34391114125046"></a><a name="p34391114125046"></a>资源标签。</p>
<p id="p41084576125046"><a name="p41084576125046"></a><a name="p41084576125046"></a>取值格式：key1,value1|key2,value2</p>
<p id="p34216870125046"><a name="p34216870125046"></a><a name="p34216870125046"></a>多个标签之间用"|"分开，每个标签的键值用英文逗号","相隔。</p>
<p id="p1526014454308"><a name="p1526014454308"></a><a name="p1526014454308"></a>多个标签之间为“与”的关系。</p>
<p id="p16628284115121"><a name="p16628284115121"></a><a name="p16628284115121"></a>关于资源标签，请参见<a href="添加资源标签.md">添加资源标签</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section44958995161021"></a>

无

## 响应<a name="section40090803161031"></a>

-   要素说明

    **表 2**  响应样例的要素说明

    <a name="table6655637171923"></a>
    <table><thead align="left"><tr id="row12436182171923"><th class="cellrowborder" valign="top" width="20.41%" id="mcps1.2.4.1.1"><p id="p18040723171923"><a name="p18040723171923"></a><a name="p18040723171923"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="28.57%" id="mcps1.2.4.1.2"><p id="p12288867171923"><a name="p12288867171923"></a><a name="p12288867171923"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.019999999999996%" id="mcps1.2.4.1.3"><p id="p16021685171923"><a name="p16021685171923"></a><a name="p16021685171923"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row33084878171923"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.1 "><p id="p10518479171923"><a name="p10518479171923"></a><a name="p10518479171923"></a>zones</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p17816324171923"><a name="p17816324171923"></a><a name="p17816324171923"></a><em id="i1686651617218"><a name="i1686651617218"></a><a name="i1686651617218"></a>列表数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="51.019999999999996%" headers="mcps1.2.4.1.3 "><p id="p64387025171923"><a name="p64387025171923"></a><a name="p64387025171923"></a>zone列表对象。</p>
    </td>
    </tr>
    <tr id="row45921614175143"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.1 "><p id="p10641344175143"><a name="p10641344175143"></a><a name="p10641344175143"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.2.4.1.2 "><p id="p24643947175143"><a name="p24643947175143"></a><a name="p24643947175143"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.019999999999996%" headers="mcps1.2.4.1.3 "><p id="p50002691175143"><a name="p50002691175143"></a><a name="p50002691175143"></a>返回满足过滤条件的资源总数。</p>
    </td>
    </tr>
    </tbody>
    </table>

    其中，[表2](#table6655637171923)中的zones参数说明，请参见[表3](#table10871190151410)；metadata参数说明，请参见[表4](#table141615131414)。

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
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p178921305144"><a name="p178921305144"></a><a name="p178921305144"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p1589419081418"><a name="p1589419081418"></a><a name="p1589419081418"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="row208952016144"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p198981207149"><a name="p198981207149"></a><a name="p198981207149"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p0901205148"><a name="p0901205148"></a><a name="p0901205148"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p5904140161420"><a name="p5904140161420"></a><a name="p5904140161420"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="row1905180111413"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p129067010142"><a name="p129067010142"></a><a name="p129067010142"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p1890800161415"><a name="p1890800161415"></a><a name="p1890800161415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p790916010141"><a name="p790916010141"></a><a name="p790916010141"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="row89101018143"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p791270191413"><a name="p791270191413"></a><a name="p791270191413"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p09136021413"><a name="p09136021413"></a><a name="p09136021413"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p791613013147"><a name="p791613013147"></a><a name="p791613013147"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="row69166031414"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p179190018143"><a name="p179190018143"></a><a name="p179190018143"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p292119018147"><a name="p292119018147"></a><a name="p292119018147"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p492370131414"><a name="p492370131414"></a><a name="p492370131414"></a>zone类型，公网或者内网。</p>
    </td>
    </tr>
    <tr id="row1792616091413"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p109283011142"><a name="p109283011142"></a><a name="p109283011142"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p189301209147"><a name="p189301209147"></a><a name="p189301209147"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p1893460141411"><a name="p1893460141411"></a><a name="p1893460141411"></a>该zone下SOA记录中的ttl值。</p>
    </td>
    </tr>
    <tr id="row49346041419"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p193630171412"><a name="p193630171412"></a><a name="p193630171412"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p19940160111416"><a name="p19940160111416"></a><a name="p19940160111416"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p1894211012145"><a name="p1894211012145"></a><a name="p1894211012145"></a>该zone下SOA记录中用于标识变更的序列值。</p>
    </td>
    </tr>
    <tr id="row1494311013144"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p1394519012141"><a name="p1394519012141"></a><a name="p1394519012141"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p199461401144"><a name="p199461401144"></a><a name="p199461401144"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p494720017143"><a name="p494720017143"></a><a name="p494720017143"></a>资源状态。</p>
    <p id="p29501003143"><a name="p29501003143"></a><a name="p29501003143"></a>取值范围：PENDING_CREATE, ACTIVE, PENDING_DELETE, ERROR。</p>
    </td>
    </tr>
    <tr id="row1595113017149"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p1395410081413"><a name="p1395410081413"></a><a name="p1395410081413"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p179551801147"><a name="p179551801147"></a><a name="p179551801147"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p595712021413"><a name="p595712021413"></a><a name="p595712021413"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="row69595020143"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p15962150151419"><a name="p15962150151419"></a><a name="p15962150151419"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p6965803142"><a name="p6965803142"></a><a name="p6965803142"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p1596710031411"><a name="p1596710031411"></a><a name="p1596710031411"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="row49683010141"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p2097010181418"><a name="p2097010181418"></a><a name="p2097010181418"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p1397430121412"><a name="p1397430121412"></a><a name="p1397430121412"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p149761809149"><a name="p149761809149"></a><a name="p149761809149"></a>zone所属的租户ID。</p>
    </td>
    </tr>
    <tr id="row129774031419"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p15980200171419"><a name="p15980200171419"></a><a name="p15980200171419"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p69816019146"><a name="p69816019146"></a><a name="p69816019146"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p159835018143"><a name="p159835018143"></a><a name="p159835018143"></a>创建时间。</p>
    </td>
    </tr>
    <tr id="row1498413011412"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p398715081417"><a name="p398715081417"></a><a name="p398715081417"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p1988190121420"><a name="p1988190121420"></a><a name="p1988190121420"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p169905051413"><a name="p169905051413"></a><a name="p169905051413"></a>更新时间。</p>
    </td>
    </tr>
    <tr id="row999050111419"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p8993407142"><a name="p8993407142"></a><a name="p8993407142"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p899518011417"><a name="p899518011417"></a><a name="p899518011417"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p1799719041413"><a name="p1799719041413"></a><a name="p1799719041413"></a>指向当前资源或者其他资源的链接。</p>
    <p id="p109986017142"><a name="p109986017142"></a><a name="p109986017142"></a>当查询需要分页时，需要包含一个next链接指向下一页。</p>
    </td>
    </tr>
    <tr id="row29991001416"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p1311419142"><a name="p1311419142"></a><a name="p1311419142"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p185151151417"><a name="p185151151417"></a><a name="p185151151417"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p1876191410"><a name="p1876191410"></a><a name="p1876191410"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    </td>
    </tr>
    <tr id="row18881161418"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p6114111411"><a name="p6114111411"></a><a name="p6114111411"></a>routers</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p10131212146"><a name="p10131212146"></a><a name="p10131212146"></a>List&lt;Router&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p161561141410"><a name="p161561141410"></a><a name="p161561141410"></a>与该zone关联的Router(VPC)列表。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  metadata参数说明

    <a name="table141615131414"></a>
    <table><thead align="left"><tr id="row223813147"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p1266151412"><a name="p1266151412"></a><a name="p1266151412"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p12286121410"><a name="p12286121410"></a><a name="p12286121410"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p02911119140"><a name="p02911119140"></a><a name="p02911119140"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row33219131412"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p8341314143"><a name="p8341314143"></a><a name="p8341314143"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p123671111420"><a name="p123671111420"></a><a name="p123671111420"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p1339111149"><a name="p1339111149"></a><a name="p1339111149"></a>资源总数</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "links": {
            "self": "https://Endpoint/v2/zones?type=private&limit=11&marker=&name=&status="
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


## 返回值<a name="section42637797161043"></a>

请参考[通用请求返回值](通用请求返回值.md)。

