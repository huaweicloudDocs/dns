# 查询单个Zone下Record Set列表<a name="dns_api_65004"></a>

## 功能介绍<a name="section8391370"></a>

查询单个Zone下Record Set列表。

## URI<a name="section8413469"></a>

GET /v2.1/zones/\{zone\_id\}/recordsets?limit=\{limit\}&offset=\{offset\}&marker=\{marker\}&line\_id=\{line\_id\}&tags=\{tags\}&status=\{status\}&type=\{type\}&name=\{name\}&id=\{id\}&sort\_key=\{sort\_key\}&sort\_dir=\{sort\_dir\}&search\_mode=\{search\_mode\}

参数说明请参见[表1](#table48883615)。

**表 1**  URI格式的参数说明

<a name="table48883615"></a>
<table><thead align="left"><tr id="row57562809"><th class="cellrowborder" valign="top" width="17.511751175117514%" id="mcps1.2.5.1.1"><p id="p32075938"><a name="p32075938"></a><a name="p32075938"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.231423142314231%" id="mcps1.2.5.1.2"><p id="p48014184"><a name="p48014184"></a><a name="p48014184"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.531453145314533%" id="mcps1.2.5.1.3"><p id="p63943666"><a name="p63943666"></a><a name="p63943666"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.725372537253726%" id="mcps1.2.5.1.4"><p id="p12054440"><a name="p12054440"></a><a name="p12054440"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row36885620"><td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.1 "><p id="p34945211"><a name="p34945211"></a><a name="p34945211"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.231423142314231%" headers="mcps1.2.5.1.2 "><p id="p11989863"><a name="p11989863"></a><a name="p11989863"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.531453145314533%" headers="mcps1.2.5.1.3 "><p id="p31654880"><a name="p31654880"></a><a name="p31654880"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.725372537253726%" headers="mcps1.2.5.1.4 "><p id="p13908493"><a name="p13908493"></a><a name="p13908493"></a>所属zone id。仅支持公网zone。</p>
<p id="p22777371252"><a name="p22777371252"></a><a name="p22777371252"></a>可以通过<a href="查询公网Zone列表.md">查询公网Zone列表</a>获取。</p>
</td>
</tr>
<tr id="row58067579"><td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.1 "><p id="p5853458"><a name="p5853458"></a><a name="p5853458"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="14.231423142314231%" headers="mcps1.2.5.1.2 "><p id="p4368081"><a name="p4368081"></a><a name="p4368081"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.531453145314533%" headers="mcps1.2.5.1.3 "><p id="p18270305"><a name="p18270305"></a><a name="p18270305"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.725372537253726%" headers="mcps1.2.5.1.4 "><p id="p3499754"><a name="p3499754"></a><a name="p3499754"></a>分页查询起始的资源ID，为空时为查询第一页。</p>
<p id="p191113424551"><a name="p191113424551"></a><a name="p191113424551"></a>默认值为空。</p>
</td>
</tr>
<tr id="row31497787"><td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.1 "><p id="p1183915"><a name="p1183915"></a><a name="p1183915"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="14.231423142314231%" headers="mcps1.2.5.1.2 "><p id="p28788263"><a name="p28788263"></a><a name="p28788263"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.531453145314533%" headers="mcps1.2.5.1.3 "><p id="p50147992"><a name="p50147992"></a><a name="p50147992"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="53.725372537253726%" headers="mcps1.2.5.1.4 "><p id="p230120311413"><a name="p230120311413"></a><a name="p230120311413"></a>每页返回的资源个数。</p>
<p id="p147131447514"><a name="p147131447514"></a><a name="p147131447514"></a>取值范围：0~500</p>
<p id="p1385813431412"><a name="p1385813431412"></a><a name="p1385813431412"></a>取值一般为10，20，50。默认值为500。</p>
</td>
</tr>
<tr id="row194111235714"><td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.1 "><p id="p8880515195550"><a name="p8880515195550"></a><a name="p8880515195550"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="14.231423142314231%" headers="mcps1.2.5.1.2 "><p id="p48233143195550"><a name="p48233143195550"></a><a name="p48233143195550"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.531453145314533%" headers="mcps1.2.5.1.3 "><p id="p14570511195550"><a name="p14570511195550"></a><a name="p14570511195550"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="53.725372537253726%" headers="mcps1.2.5.1.4 "><p id="p35951433204916"><a name="p35951433204916"></a><a name="p35951433204916"></a>分页查询起始偏移量，表示从偏移量的下一个资源开始查询。</p>
<p id="p18898143914915"><a name="p18898143914915"></a><a name="p18898143914915"></a>取值范围：0~2147483647</p>
<p id="p13209172234718"><a name="p13209172234718"></a><a name="p13209172234718"></a>默认值为0。</p>
<p id="p167712216335"><a name="p167712216335"></a><a name="p167712216335"></a>当前设置marker不为空时，以marker为分页起始标识。</p>
</td>
</tr>
<tr id="row15709056145520"><td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.1 "><p id="p55549708145520"><a name="p55549708145520"></a><a name="p55549708145520"></a>line_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.231423142314231%" headers="mcps1.2.5.1.2 "><p id="p3232537145520"><a name="p3232537145520"></a><a name="p3232537145520"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.531453145314533%" headers="mcps1.2.5.1.3 "><p id="p60508934145520"><a name="p60508934145520"></a><a name="p60508934145520"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.725372537253726%" headers="mcps1.2.5.1.4 "><p id="p2276603145520"><a name="p2276603145520"></a><a name="p2276603145520"></a>解析线路ID。请参见<a href="解析线路类型.md">解析线路类型</a>。</p>
<p id="p879811229562"><a name="p879811229562"></a><a name="p879811229562"></a>搜索模式默认为模糊搜索。</p>
<p id="p44937551555"><a name="p44937551555"></a><a name="p44937551555"></a>默认值为空。</p>
</td>
</tr>
<tr id="row16748840142918"><td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.1 "><p id="p5356332712210"><a name="p5356332712210"></a><a name="p5356332712210"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="14.231423142314231%" headers="mcps1.2.5.1.2 "><p id="p4366222612210"><a name="p4366222612210"></a><a name="p4366222612210"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.531453145314533%" headers="mcps1.2.5.1.3 "><p id="p4697942612210"><a name="p4697942612210"></a><a name="p4697942612210"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.725372537253726%" headers="mcps1.2.5.1.4 "><p id="p4723714212210"><a name="p4723714212210"></a><a name="p4723714212210"></a>资源标签。</p>
<p id="p2248109712210"><a name="p2248109712210"></a><a name="p2248109712210"></a>取值格式：key1,value1|key2,value2</p>
<p id="p52490216114132"><a name="p52490216114132"></a><a name="p52490216114132"></a>多个标签之间用"|"分开，每个标签的键值用英文逗号","相隔。</p>
<p id="p100328712210"><a name="p100328712210"></a><a name="p100328712210"></a>多个标签之间为“与”的关系。</p>
<p id="p60075024115136"><a name="p60075024115136"></a><a name="p60075024115136"></a>关于资源标签，请参见<a href="添加资源标签.md">添加资源标签</a>。</p>
<p id="p1770514714203"><a name="p1770514714203"></a><a name="p1770514714203"></a>搜索模式为精确搜索。如果资源标签值value是以*开头时，则按照*后面的值全模糊匹配。</p>
<p id="p71284149127"><a name="p71284149127"></a><a name="p71284149127"></a>默认值为空。</p>
</td>
</tr>
<tr id="row1051011382294"><td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.1 "><p id="p15187431105515"><a name="p15187431105515"></a><a name="p15187431105515"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="14.231423142314231%" headers="mcps1.2.5.1.2 "><p id="p21877311559"><a name="p21877311559"></a><a name="p21877311559"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.531453145314533%" headers="mcps1.2.5.1.3 "><p id="p18187143110551"><a name="p18187143110551"></a><a name="p18187143110551"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.725372537253726%" headers="mcps1.2.5.1.4 "><p id="p181873314559"><a name="p181873314559"></a><a name="p181873314559"></a>待查询的Record Set的状态。</p>
<p id="p447517111159"><a name="p447517111159"></a><a name="p447517111159"></a>取值范围：ACTIVE、ERROR、DISABLE、FREEZE、PENDING_CREATE、PENDING_UPDATE、PENDING_DELETE</p>
<p id="p1249182022812"><a name="p1249182022812"></a><a name="p1249182022812"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
<p id="p1289715373203"><a name="p1289715373203"></a><a name="p1289715373203"></a>搜索模式默认为模糊搜索。</p>
<p id="p1135030171215"><a name="p1135030171215"></a><a name="p1135030171215"></a>默认值为空。</p>
</td>
</tr>
<tr id="row14164736132914"><td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.1 "><p id="p4998111210116"><a name="p4998111210116"></a><a name="p4998111210116"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="14.231423142314231%" headers="mcps1.2.5.1.2 "><p id="p89981512101120"><a name="p89981512101120"></a><a name="p89981512101120"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.531453145314533%" headers="mcps1.2.5.1.3 "><p id="p399821215119"><a name="p399821215119"></a><a name="p399821215119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.725372537253726%" headers="mcps1.2.5.1.4 "><p id="p109982012141111"><a name="p109982012141111"></a><a name="p109982012141111"></a>待查询的Record Set的记录集类型。</p>
<p id="p20817123416132"><a name="p20817123416132"></a><a name="p20817123416132"></a>取值范围：A、CNAME、MX、AAAA、TXT、SRV、NS、CAA</p>
<p id="p1360713682913"><a name="p1360713682913"></a><a name="p1360713682913"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a>。</p>
<p id="p1043618556290"><a name="p1043618556290"></a><a name="p1043618556290"></a>如果为空，表示查询所有类型的Record Set。</p>
<p id="p7802199183214"><a name="p7802199183214"></a><a name="p7802199183214"></a>搜索模式固定为精确搜索。</p>
</td>
</tr>
<tr id="row16853432913"><td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.1 "><p id="p189276527168"><a name="p189276527168"></a><a name="p189276527168"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.231423142314231%" headers="mcps1.2.5.1.2 "><p id="p19927752151617"><a name="p19927752151617"></a><a name="p19927752151617"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.531453145314533%" headers="mcps1.2.5.1.3 "><p id="p1492719522167"><a name="p1492719522167"></a><a name="p1492719522167"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.725372537253726%" headers="mcps1.2.5.1.4 "><p id="p11927252121613"><a name="p11927252121613"></a><a name="p11927252121613"></a>待查询的Record Set的域名中包含此name。</p>
<p id="p1586175254812"><a name="p1586175254812"></a><a name="p1586175254812"></a>搜索模式默认为模糊搜索。</p>
<p id="p1158615213489"><a name="p1158615213489"></a><a name="p1158615213489"></a>默认值为空。</p>
</td>
</tr>
<tr id="row1088413162919"><td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.1 "><p id="p13604691913"><a name="p13604691913"></a><a name="p13604691913"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="14.231423142314231%" headers="mcps1.2.5.1.2 "><p id="p15360960192"><a name="p15360960192"></a><a name="p15360960192"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.531453145314533%" headers="mcps1.2.5.1.3 "><p id="p4360869195"><a name="p4360869195"></a><a name="p4360869195"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.725372537253726%" headers="mcps1.2.5.1.4 "><p id="p173609610193"><a name="p173609610193"></a><a name="p173609610193"></a>待查询的Record Set的id包含此id。</p>
<p id="p189538469489"><a name="p189538469489"></a><a name="p189538469489"></a>搜索模式默认为模糊搜索。</p>
<p id="p16953846104816"><a name="p16953846104816"></a><a name="p16953846104816"></a>默认值为空。</p>
</td>
</tr>
<tr id="row9685158173314"><td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.1 "><p id="p15674182317363"><a name="p15674182317363"></a><a name="p15674182317363"></a>sort_key</p>
</td>
<td class="cellrowborder" valign="top" width="14.231423142314231%" headers="mcps1.2.5.1.2 "><p id="p206741223103614"><a name="p206741223103614"></a><a name="p206741223103614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.531453145314533%" headers="mcps1.2.5.1.3 "><p id="p7674132316360"><a name="p7674132316360"></a><a name="p7674132316360"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.725372537253726%" headers="mcps1.2.5.1.4 "><p id="p4674182316366"><a name="p4674182316366"></a><a name="p4674182316366"></a>查询结果中Record Set列表的排序字段。</p>
<p id="p161032135113"><a name="p161032135113"></a><a name="p161032135113"></a>取值范围：</p>
<a name="ul0957431182915"></a><a name="ul0957431182915"></a><ul id="ul0957431182915"><li>name：域名</li><li>type：记录集类型</li></ul>
<p id="p1627913348564"><a name="p1627913348564"></a><a name="p1627913348564"></a>默认值为空，表示不排序。</p>
</td>
</tr>
<tr id="row5685558123311"><td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.1 "><p id="p208891026103817"><a name="p208891026103817"></a><a name="p208891026103817"></a>sort_dir</p>
</td>
<td class="cellrowborder" valign="top" width="14.231423142314231%" headers="mcps1.2.5.1.2 "><p id="p4889162653813"><a name="p4889162653813"></a><a name="p4889162653813"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.531453145314533%" headers="mcps1.2.5.1.3 "><p id="p128891626133813"><a name="p128891626133813"></a><a name="p128891626133813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.725372537253726%" headers="mcps1.2.5.1.4 "><p id="p116071347131216"><a name="p116071347131216"></a><a name="p116071347131216"></a>查询结果中Record Set列表的排序方式。</p>
<p id="p1791903818290"><a name="p1791903818290"></a><a name="p1791903818290"></a>取值范围：</p>
<a name="ul4952114912919"></a><a name="ul4952114912919"></a><ul id="ul4952114912919"><li>desc：降序排序</li><li>asc：升序排序</li></ul>
<p id="p654483914567"><a name="p654483914567"></a><a name="p654483914567"></a>默认值为空，表示不排序。</p>
</td>
</tr>
<tr id="row1726461293718"><td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.1 "><p id="p18706105912812"><a name="p18706105912812"></a><a name="p18706105912812"></a>search_mode</p>
</td>
<td class="cellrowborder" valign="top" width="14.231423142314231%" headers="mcps1.2.5.1.2 "><p id="p1170612591285"><a name="p1170612591285"></a><a name="p1170612591285"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.531453145314533%" headers="mcps1.2.5.1.3 "><p id="p1224515100294"><a name="p1224515100294"></a><a name="p1224515100294"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53.725372537253726%" headers="mcps1.2.5.1.4 "><p id="p58943176292"><a name="p58943176292"></a><a name="p58943176292"></a>查询条件搜索模式。</p>
<p id="p789417178294"><a name="p789417178294"></a><a name="p789417178294"></a>取值范围：</p>
<a name="ul1789514177290"></a><a name="ul1789514177290"></a><ul id="ul1789514177290"><li>like：模糊搜索</li><li>equal：精确搜索</li></ul>
<p id="p199619457301"><a name="p199619457301"></a><a name="p199619457301"></a>默认值为模糊搜索。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section8612359"></a>

-   请求参数

    无

-   请求样例

    查询域名的记录集列表，域名的Zone ID为“2c9eb155587194ec01587224c9f90149”，线路ID为“default\_view”。

    ```
    GET https://{DNS_Endpoint}/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets?limit=&offset=&line_id=default_view
    ```


## 响应<a name="section10402369"></a>

-   要素说明

    **表 2**  响应样例的要素说明

    <a name="table53402119"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0037129969_row41580444"><th class="cellrowborder" valign="top" width="18.64%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0037129969_p12572829"><a name="zh-cn_topic_0037129969_p12572829"></a><a name="zh-cn_topic_0037129969_p12572829"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.740000000000002%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0037129969_p13543581"><a name="zh-cn_topic_0037129969_p13543581"></a><a name="zh-cn_topic_0037129969_p13543581"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.62%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0037129969_p23288300"><a name="zh-cn_topic_0037129969_p23288300"></a><a name="zh-cn_topic_0037129969_p23288300"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1133192112515"><td class="cellrowborder" valign="top" width="18.64%" headers="mcps1.2.4.1.1 "><p id="a96b57b88bc5b4333a0887ecf8b6aa4f1"><a name="a96b57b88bc5b4333a0887ecf8b6aa4f1"></a><a name="a96b57b88bc5b4333a0887ecf8b6aa4f1"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.740000000000002%" headers="mcps1.2.4.1.2 "><p id="a023c6a235bea4726ad4afd77648d5918"><a name="a023c6a235bea4726ad4afd77648d5918"></a><a name="a023c6a235bea4726ad4afd77648d5918"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.62%" headers="mcps1.2.4.1.3 "><p id="a41f3f8b60b9d4d89a1c10106ecbad1f0"><a name="a41f3f8b60b9d4d89a1c10106ecbad1f0"></a><a name="a41f3f8b60b9d4d89a1c10106ecbad1f0"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。详细信息请参见<a href="#table354521744216">表5</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129969_row7304143"><td class="cellrowborder" valign="top" width="18.64%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129969_p54764719"><a name="zh-cn_topic_0037129969_p54764719"></a><a name="zh-cn_topic_0037129969_p54764719"></a>recordsets</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.740000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129969_p10465156"><a name="zh-cn_topic_0037129969_p10465156"></a><a name="zh-cn_topic_0037129969_p10465156"></a>Array of object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.62%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129969_p45797138"><a name="zh-cn_topic_0037129969_p45797138"></a><a name="zh-cn_topic_0037129969_p45797138"></a>recordset列表对象，详细信息请参见<a href="#table7192645154740">表3</a>。</p>
    </td>
    </tr>
    <tr id="ra36d54752ed44415a573a743060b4dc8"><td class="cellrowborder" valign="top" width="18.64%" headers="mcps1.2.4.1.1 "><p id="acfae956c5b3948318d1c49c7521cace4"><a name="acfae956c5b3948318d1c49c7521cace4"></a><a name="acfae956c5b3948318d1c49c7521cace4"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.740000000000002%" headers="mcps1.2.4.1.2 "><p id="aef6bb96f7ac64bef8949bb9d76432fd4"><a name="aef6bb96f7ac64bef8949bb9d76432fd4"></a><a name="aef6bb96f7ac64bef8949bb9d76432fd4"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.62%" headers="mcps1.2.4.1.3 "><p id="aa2edc4c85ec14e53bf99f656877a8cb6"><a name="aa2edc4c85ec14e53bf99f656877a8cb6"></a><a name="aa2edc4c85ec14e53bf99f656877a8cb6"></a>返回满足过滤条件的资源总数，详细信息请参见<a href="#table2908319718932">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  recordsets字段说明

    <a name="table7192645154740"></a>
    <table><thead align="left"><tr id="r1e1c128f84704d9d8858c2e0cc8049be"><th class="cellrowborder" valign="top" width="18.33%" id="mcps1.2.4.1.1"><p id="a47357ec60283412e9897cd0a22b6a0c3"><a name="a47357ec60283412e9897cd0a22b6a0c3"></a><a name="a47357ec60283412e9897cd0a22b6a0c3"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.95%" id="mcps1.2.4.1.2"><p id="af1d10def3811489faeb6324c8c5959ae"><a name="af1d10def3811489faeb6324c8c5959ae"></a><a name="af1d10def3811489faeb6324c8c5959ae"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.72%" id="mcps1.2.4.1.3"><p id="ae0a7865b82b14931a8d9a55961d44788"><a name="ae0a7865b82b14931a8d9a55961d44788"></a><a name="ae0a7865b82b14931a8d9a55961d44788"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="rde37e2b42d744b86980b261586f1ffb7"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="ad2d4146e7bbc44af868bd92eb385e665"><a name="ad2d4146e7bbc44af868bd92eb385e665"></a><a name="ad2d4146e7bbc44af868bd92eb385e665"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="af96a1ffa52d04ff294081eb82e501a92"><a name="af96a1ffa52d04ff294081eb82e501a92"></a><a name="af96a1ffa52d04ff294081eb82e501a92"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="a9f17739bff234a47bf293f848c4344d8"><a name="a9f17739bff234a47bf293f848c4344d8"></a><a name="a9f17739bff234a47bf293f848c4344d8"></a>Record Set的ID。</p>
    </td>
    </tr>
    <tr id="r78cca1480c6d47e68aef8f2128f96637"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a23c483d0fc634e0a8c41762e691c4d0b"><a name="a23c483d0fc634e0a8c41762e691c4d0b"></a><a name="a23c483d0fc634e0a8c41762e691c4d0b"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="a2e378b055c8b4e1e9cfdbca2c3320a4b"><a name="a2e378b055c8b4e1e9cfdbca2c3320a4b"></a><a name="a2e378b055c8b4e1e9cfdbca2c3320a4b"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="aaa79ddd8103f462bacf7ee1742390f7d"><a name="aaa79ddd8103f462bacf7ee1742390f7d"></a><a name="aaa79ddd8103f462bacf7ee1742390f7d"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="r3b1c5aeb8c864adb87b229f9a623cd18"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="ac12845ea83a74b2886de2a84b26694f1"><a name="ac12845ea83a74b2886de2a84b26694f1"></a><a name="ac12845ea83a74b2886de2a84b26694f1"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="a13a616f04c3544baacce34c089e3b36c"><a name="a13a616f04c3544baacce34c089e3b36c"></a><a name="a13a616f04c3544baacce34c089e3b36c"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="a2a5366f74f5944d7b8e1453e3630d59b"><a name="a2a5366f74f5944d7b8e1453e3630d59b"></a><a name="a2a5366f74f5944d7b8e1453e3630d59b"></a>Record Set的描述信息。</p>
    </td>
    </tr>
    <tr id="r590d49c6db954543963214db92cd258b"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a23b85fe289494bff9b2672c867ec3093"><a name="a23b85fe289494bff9b2672c867ec3093"></a><a name="a23b85fe289494bff9b2672c867ec3093"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="a0b95f536a1664ddaa5cd687025d6a127"><a name="a0b95f536a1664ddaa5cd687025d6a127"></a><a name="a0b95f536a1664ddaa5cd687025d6a127"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="a8b502134467d4da0b67621d575aec531"><a name="a8b502134467d4da0b67621d575aec531"></a><a name="a8b502134467d4da0b67621d575aec531"></a>托管该记录的zone_id。</p>
    </td>
    </tr>
    <tr id="r914aa6319cb54a04a5aa8feb584f3427"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a9b5efe8df8b641ccbc601260c4837686"><a name="a9b5efe8df8b641ccbc601260c4837686"></a><a name="a9b5efe8df8b641ccbc601260c4837686"></a>zone_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="a6325c837211a4c0697fe0fbe3ea02be1"><a name="a6325c837211a4c0697fe0fbe3ea02be1"></a><a name="a6325c837211a4c0697fe0fbe3ea02be1"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="a5cb1bbf7d3cc4e79b21020f8b4c83c74"><a name="a5cb1bbf7d3cc4e79b21020f8b4c83c74"></a><a name="a5cb1bbf7d3cc4e79b21020f8b4c83c74"></a>托管该记录的zone_name。</p>
    </td>
    </tr>
    <tr id="r881963e6a69d4813a968631198d5d171"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a73f48e61c4c346b69ff6c3a7f91506ad"><a name="a73f48e61c4c346b69ff6c3a7f91506ad"></a><a name="a73f48e61c4c346b69ff6c3a7f91506ad"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="a15ea7f0f8def4cd8a8e0bdcdf99df87a"><a name="a15ea7f0f8def4cd8a8e0bdcdf99df87a"></a><a name="a15ea7f0f8def4cd8a8e0bdcdf99df87a"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="ada51b2d4b5e343a4a944f0c5d2c11763"><a name="ada51b2d4b5e343a4a944f0c5d2c11763"></a><a name="ada51b2d4b5e343a4a944f0c5d2c11763"></a>记录类型。</p>
    <p id="a71343e00a16842a389149e6702d24cc8"><a name="a71343e00a16842a389149e6702d24cc8"></a><a name="a71343e00a16842a389149e6702d24cc8"></a>取值范围：A、AAAA、MX、CNAME、TXT、NS、SRV、CAA。</p>
    <p id="zh-cn_topic_0082840629_p190917111419"><a name="zh-cn_topic_0082840629_p190917111419"></a><a name="zh-cn_topic_0082840629_p190917111419"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a>。</p>
    </td>
    </tr>
    <tr id="r63e8e50968df4dbc9a1eaa0eb80d5e3a"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="ab8f56bedc1914f489aa5864d019ea48c"><a name="ab8f56bedc1914f489aa5864d019ea48c"></a><a name="ab8f56bedc1914f489aa5864d019ea48c"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="a496ff269cab64ca6891d044bc9ec629a"><a name="a496ff269cab64ca6891d044bc9ec629a"></a><a name="a496ff269cab64ca6891d044bc9ec629a"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="p123031523174010"><a name="p123031523174010"></a><a name="p123031523174010"></a>解析记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="p1030317233408"><a name="p1030317233408"></a><a name="p1030317233408"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    </td>
    </tr>
    <tr id="rdb895ebca3c443f89c18fe7b6197f05b"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a2f11d54099fb47f09bee139b961775fa"><a name="a2f11d54099fb47f09bee139b961775fa"></a><a name="a2f11d54099fb47f09bee139b961775fa"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="a564302f3c406442bae9ee32a3273a28d"><a name="a564302f3c406442bae9ee32a3273a28d"></a><a name="a564302f3c406442bae9ee32a3273a28d"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="a1564c41ab4194359b85b6c7d290d6c08"><a name="a1564c41ab4194359b85b6c7d290d6c08"></a><a name="a1564c41ab4194359b85b6c7d290d6c08"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="r112c25618e7349c188cbca0926d7047c"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="aeb8cbc37eafc4b66a9b36c5e9a2497e4"><a name="aeb8cbc37eafc4b66a9b36c5e9a2497e4"></a><a name="aeb8cbc37eafc4b66a9b36c5e9a2497e4"></a>create_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="a22e929037d3d4e7281eb6a53c50c41a9"><a name="a22e929037d3d4e7281eb6a53c50c41a9"></a><a name="a22e929037d3d4e7281eb6a53c50c41a9"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="ab89dc0e78e494dccbcea7f54f3c34c50"><a name="ab89dc0e78e494dccbcea7f54f3c34c50"></a><a name="ab89dc0e78e494dccbcea7f54f3c34c50"></a>创建时间。</p>
    <p id="p583516468316"><a name="p583516468316"></a><a name="p583516468316"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="r54b90d4feda7405eb5c7e794db5fae31"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a46f8ddfd55a74ac1a2249ce568489558"><a name="a46f8ddfd55a74ac1a2249ce568489558"></a><a name="a46f8ddfd55a74ac1a2249ce568489558"></a>update_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="ab1c3d9aa0d8f424187ba65966054b255"><a name="ab1c3d9aa0d8f424187ba65966054b255"></a><a name="ab1c3d9aa0d8f424187ba65966054b255"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="ac1d22d91bda24ac4b43a669a6e0a50ab"><a name="ac1d22d91bda24ac4b43a669a6e0a50ab"></a><a name="ac1d22d91bda24ac4b43a669a6e0a50ab"></a>更新时间。</p>
    <p id="p1481431019435"><a name="p1481431019435"></a><a name="p1481431019435"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="rb5357a35fa8e402aa600113d6a0f2dd4"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a484cc633a10f4add9ccf9937688f94d3"><a name="a484cc633a10f4add9ccf9937688f94d3"></a><a name="a484cc633a10f4add9ccf9937688f94d3"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="a52f4743953d941a4b9f648daf7450f47"><a name="a52f4743953d941a4b9f648daf7450f47"></a><a name="a52f4743953d941a4b9f648daf7450f47"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="a300a6ef4814a48ed850ab725d74c36f0"><a name="a300a6ef4814a48ed850ab725d74c36f0"></a><a name="a300a6ef4814a48ed850ab725d74c36f0"></a>资源状态。</p>
    <p id="zh-cn_topic_0082840629_p173273316513"><a name="zh-cn_topic_0082840629_p173273316513"></a><a name="zh-cn_topic_0082840629_p173273316513"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="recd834eb2cde45919ed4c0b8e04b1300"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="ae54641c970664b869f723feae0f7109d"><a name="ae54641c970664b869f723feae0f7109d"></a><a name="ae54641c970664b869f723feae0f7109d"></a>default</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="a532521ef797145d49c441c42b666b2c5"><a name="a532521ef797145d49c441c42b666b2c5"></a><a name="a532521ef797145d49c441c42b666b2c5"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="a6053108c64844350ad488fe71da32cb5"><a name="a6053108c64844350ad488fe71da32cb5"></a><a name="a6053108c64844350ad488fe71da32cb5"></a>标识是否由系统默认生成，系统默认生成的Record Set不能删除。</p>
    </td>
    </tr>
    <tr id="r5381b89f9b6a4c67b9627a3ecc4c6dde"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="acfd894c51cd249b8a799cc1321047b84"><a name="acfd894c51cd249b8a799cc1321047b84"></a><a name="acfd894c51cd249b8a799cc1321047b84"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="a863f4837ee554d0e916c2a353c1200fb"><a name="a863f4837ee554d0e916c2a353c1200fb"></a><a name="a863f4837ee554d0e916c2a353c1200fb"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="p4619625201026"><a name="p4619625201026"></a><a name="p4619625201026"></a>该Record Set所属的项目ID。</p>
    </td>
    </tr>
    <tr id="rc1cde3b896614a61a47991413acf50e4"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="aef1ec992ca8f4cfdbc4b0652cf99c78f"><a name="aef1ec992ca8f4cfdbc4b0652cf99c78f"></a><a name="aef1ec992ca8f4cfdbc4b0652cf99c78f"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="a71d4145b459c4a6bbacb6db08780fd39"><a name="a71d4145b459c4a6bbacb6db08780fd39"></a><a name="a71d4145b459c4a6bbacb6db08780fd39"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="a9aee8ca227104938bb4c8b64a562a036"><a name="a9aee8ca227104938bb4c8b64a562a036"></a><a name="a9aee8ca227104938bb4c8b64a562a036"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。详细信息请参见<a href="#table354521744216">表5</a>。</p>
    </td>
    </tr>
    <tr id="r163c7219674c428d9ba004bd34b126fc"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="adfe87a219834453f9ea477e8407de277"><a name="adfe87a219834453f9ea477e8407de277"></a><a name="adfe87a219834453f9ea477e8407de277"></a>line</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="ab06ef153bc8040f0bd13dbc98044da7a"><a name="ab06ef153bc8040f0bd13dbc98044da7a"></a><a name="ab06ef153bc8040f0bd13dbc98044da7a"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="a637c5d1a91694ab3966aff7158dc1be5"><a name="a637c5d1a91694ab3966aff7158dc1be5"></a><a name="a637c5d1a91694ab3966aff7158dc1be5"></a>解析线路ID。</p>
    </td>
    </tr>
    <tr id="r3d57eda3e7264894adbbc618c2d89631"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="af1c5cd90adcb4cc5870d69418ef4cdd7"><a name="af1c5cd90adcb4cc5870d69418ef4cdd7"></a><a name="af1c5cd90adcb4cc5870d69418ef4cdd7"></a>weight</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="af7d6437881b448a4b83ee32775cdcb65"><a name="af7d6437881b448a4b83ee32775cdcb65"></a><a name="af7d6437881b448a4b83ee32775cdcb65"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="aab650b22ad8c44dca30b84deec2c56a9"><a name="aab650b22ad8c44dca30b84deec2c56a9"></a><a name="aab650b22ad8c44dca30b84deec2c56a9"></a>解析记录的权重。</p>
    </td>
    </tr>
    <tr id="rda71fe5cc0ce4dd7abc1936b71c5028a"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="a168b1911cd8b4de4bb4e634f8eb23a8c"><a name="a168b1911cd8b4de4bb4e634f8eb23a8c"></a><a name="a168b1911cd8b4de4bb4e634f8eb23a8c"></a>health_check_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="a4512be7e447441ad8461ace549dc5f3a"><a name="a4512be7e447441ad8461ace549dc5f3a"></a><a name="a4512be7e447441ad8461ace549dc5f3a"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="a9f18725197d34f5e82f204b1ea0daf26"><a name="a9f18725197d34f5e82f204b1ea0daf26"></a><a name="a9f18725197d34f5e82f204b1ea0daf26"></a>健康检查ID。</p>
    </td>
    </tr>
    <tr id="rf458b12e8c3541a6a36e5f74d6410c84"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_p47860618461"><a name="zh-cn_topic_0082840629_p47860618461"></a><a name="zh-cn_topic_0082840629_p47860618461"></a>alias_target</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.95%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_p979319654615"><a name="zh-cn_topic_0082840629_p979319654615"></a><a name="zh-cn_topic_0082840629_p979319654615"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.72%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_p5112227475"><a name="zh-cn_topic_0082840629_p5112227475"></a><a name="zh-cn_topic_0082840629_p5112227475"></a>别名记录。详细信息请参见<a href="数据结构.md#table11888161342410">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  metadata参数说明

    <a name="table2908319718932"></a>
    <table><thead align="left"><tr id="r1ee98e923a7c4bfcaa89e708d3fca79e"><th class="cellrowborder" valign="top" width="18.43184318431843%" id="mcps1.2.4.1.1"><p id="af493c2fde22f44069c2b5ea0467dfe89"><a name="af493c2fde22f44069c2b5ea0467dfe89"></a><a name="af493c2fde22f44069c2b5ea0467dfe89"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.26192619261926%" id="mcps1.2.4.1.2"><p id="a581940a484df4c8294e51f11391a23c8"><a name="a581940a484df4c8294e51f11391a23c8"></a><a name="a581940a484df4c8294e51f11391a23c8"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.306230623062305%" id="mcps1.2.4.1.3"><p id="a0301bbf5a1234ea3a88a104e1b4cff92"><a name="a0301bbf5a1234ea3a88a104e1b4cff92"></a><a name="a0301bbf5a1234ea3a88a104e1b4cff92"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r7cc02a0ecbd24482bca90faa98114b18"><td class="cellrowborder" valign="top" width="18.43184318431843%" headers="mcps1.2.4.1.1 "><p id="a9234858cb2f447539b4b85a307884322"><a name="a9234858cb2f447539b4b85a307884322"></a><a name="a9234858cb2f447539b4b85a307884322"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.26192619261926%" headers="mcps1.2.4.1.2 "><p id="af14a2a2c8f0345f4811bb21dd2a9b667"><a name="af14a2a2c8f0345f4811bb21dd2a9b667"></a><a name="af14a2a2c8f0345f4811bb21dd2a9b667"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.306230623062305%" headers="mcps1.2.4.1.3 "><p id="a39058f9901c84eb9a776ca5cd44ede29"><a name="a39058f9901c84eb9a776ca5cd44ede29"></a><a name="a39058f9901c84eb9a776ca5cd44ede29"></a>满足查询条件的资源总数，不受分页（即limit、offset参数）影响。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  links参数说明

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
    <tr id="row147656409503"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
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
        "links": {
            "self": "https://Endpoint/v2.1/recordsets?limit=1&marker=&name=&status=&zone_id=2c9eb155587194ec01587224c9f90149",
            "next": "https://Endpoint/v2.1/recordsets?limit=11&marker=2c9eb155587194ec01587224c9f9014a&name=&status=&zone_id=2c9eb155587194ec01587224c9f90149"
        },
        "recordsets": [
            {
                "id": "2c9eb155587194ec01587224c9f9014a",
                "name": "example.com.",
                "type": "SOA",
                "ttl": 300,
                "records": [
                    "ns1.hotrot.de. xx.example.com. (1 7200 900 1209600 300)"
                ],
                "status": "ACTIVE",
                "links": {
                    "self": "https://Endpoint/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587194ec01587224c9f9014a"
                },
                "alias_target": null,
                "zone_id": "2c9eb155587194ec01587224c9f90149",
                "zone_name": "example.com.",
                "create_at": "2016-11-17T11:56:03.439",
                "update_at": "2016-11-17T11:56:06.439",
                "default": true,
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
                "line": "default_view",
                "weight": 1,
                "health_check_id":null
            },
            {
                "id": "2c9eb155587194ec01587224c9f9014c",
                "name": "example.com.",
                "type": "NS",
                "ttl": 172800,
                "records": [
                    "ns2.hotrot.de.",
                    "ns1.hotrot.de."
                ],
                "status": "ACTIVE",
                "links": {
                    "self": "https://Endpoint/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587194ec01587224c9f9014c"
                },
                "alias_target": null,
                "zone_id": "2c9eb155587194ec01587224c9f90149",
                "zone_name": "example.com.",
                "create_at": "2016-11-17T11:56:03.439",
                "update_at": "2016-11-17T11:56:06.439",
                "default": true,
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
                "line": "default_view",
                "weight": 1,
                "health_check_id":null
            },
            {
                "id": "2c9eb155587228570158722b6ac30007",
                "name": "www.example.com.",
                "description": "This is an example record set.",
                "type": "A",
                "ttl": 300,
                "records": [
                    "192.168.10.2",
                    "192.168.10.1"
                ],
                "status": "PENDING_CREATE",
                "links": {
                    "self": "https://Endpoint/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587228570158722b6ac30007"
                },
                "alias_target": null,
                "zone_id": "2c9eb155587194ec01587224c9f90149",
                "zone_name": "example.com.",
                "create_at": "2016-11-17T12:03:17.827",
                "update_at": "2016-11-17T12:56:06.439",
                "default": false,
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
                "line": "default_view",
                "weight": 1,
                "health_check_id":null
            }
        ],
        "metadata": {
            "total_count": 3
        }
    }
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

