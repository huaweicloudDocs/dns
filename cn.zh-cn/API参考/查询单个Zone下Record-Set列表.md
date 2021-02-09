# 查询单个Zone下Record Set列表<a name="dns_api_64004"></a>

## 功能介绍<a name="section8391370"></a>

查询单个Zone下Record Set列表。

## URI<a name="section8413469"></a>

GET /v2/zones/\{zone\_id\}/recordsets?limit=\{limit\}&offset=\{offset\}&marker=\{marker\}&tags=\{tags\}&status=\{status\}&type=\{type\}&name=\{name\}&id=\{id\}&sort\_key=\{sort\_key\}&sort\_dir=\{sort\_dir\}

参数说明请参见[表1](#table48883615)。

**表 1**  URI格式的参数说明

<a name="table48883615"></a>
<table><thead align="left"><tr id="row57562809"><th class="cellrowborder" valign="top" width="16.221622162216224%" id="mcps1.2.5.1.1"><p id="p32075938"><a name="p32075938"></a><a name="p32075938"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.311731173117312%" id="mcps1.2.5.1.2"><p id="p48014184"><a name="p48014184"></a><a name="p48014184"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.981798179817982%" id="mcps1.2.5.1.3"><p id="p63943666"><a name="p63943666"></a><a name="p63943666"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.2.5.1.4"><p id="p12054440"><a name="p12054440"></a><a name="p12054440"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row36885620"><td class="cellrowborder" valign="top" width="16.221622162216224%" headers="mcps1.2.5.1.1 "><p id="p34945211"><a name="p34945211"></a><a name="p34945211"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.311731173117312%" headers="mcps1.2.5.1.2 "><p id="p11989863"><a name="p11989863"></a><a name="p11989863"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.981798179817982%" headers="mcps1.2.5.1.3 "><p id="p31654880"><a name="p31654880"></a><a name="p31654880"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p13908493"><a name="p13908493"></a><a name="p13908493"></a>所属zone id。</p>
<p id="p380212115399"><a name="p380212115399"></a><a name="p380212115399"></a>公网Zone ID可以通过<a href="查询公网Zone列表.md">查询公网Zone列表</a>获取。</p>
<p id="p22777371252"><a name="p22777371252"></a><a name="p22777371252"></a>内网Zone ID可以通过<a href="查询内网Zone列表.md">查询内网Zone列表</a>获取。</p>
</td>
</tr>
<tr id="row58067579"><td class="cellrowborder" valign="top" width="16.221622162216224%" headers="mcps1.2.5.1.1 "><p id="p5853458"><a name="p5853458"></a><a name="p5853458"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="17.311731173117312%" headers="mcps1.2.5.1.2 "><p id="p4368081"><a name="p4368081"></a><a name="p4368081"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.981798179817982%" headers="mcps1.2.5.1.3 "><p id="p18270305"><a name="p18270305"></a><a name="p18270305"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p3499754"><a name="p3499754"></a><a name="p3499754"></a>分页查询起始的资源ID，为空时为查询第一页。</p>
</td>
</tr>
<tr id="row31497787"><td class="cellrowborder" valign="top" width="16.221622162216224%" headers="mcps1.2.5.1.1 "><p id="p1183915"><a name="p1183915"></a><a name="p1183915"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="17.311731173117312%" headers="mcps1.2.5.1.2 "><p id="p28788263"><a name="p28788263"></a><a name="p28788263"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.981798179817982%" headers="mcps1.2.5.1.3 "><p id="p50147992"><a name="p50147992"></a><a name="p50147992"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p230120311413"><a name="p230120311413"></a><a name="p230120311413"></a>每页返回的资源个数。</p>
<p id="p147131447514"><a name="p147131447514"></a><a name="p147131447514"></a>取值范围：0~500</p>
<p id="p1385813431412"><a name="p1385813431412"></a><a name="p1385813431412"></a>取值一般为10，20，50。默认值为500。</p>
</td>
</tr>
<tr id="row202841732113114"><td class="cellrowborder" valign="top" width="16.221622162216224%" headers="mcps1.2.5.1.1 "><p id="p5702070419554"><a name="p5702070419554"></a><a name="p5702070419554"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="17.311731173117312%" headers="mcps1.2.5.1.2 "><p id="p5527430219554"><a name="p5527430219554"></a><a name="p5527430219554"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.981798179817982%" headers="mcps1.2.5.1.3 "><p id="p4803348119554"><a name="p4803348119554"></a><a name="p4803348119554"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p35951433204916"><a name="p35951433204916"></a><a name="p35951433204916"></a>分页查询起始偏移量，表示从偏移量的下一个资源开始查询。</p>
<p id="p18898143914915"><a name="p18898143914915"></a><a name="p18898143914915"></a>取值范围：0~2147483647</p>
<p id="p13209172234718"><a name="p13209172234718"></a><a name="p13209172234718"></a>默认值为0。</p>
<p id="p167712216335"><a name="p167712216335"></a><a name="p167712216335"></a>当前设置marker不为空时，以marker为分页起始标识。</p>
</td>
</tr>
<tr id="row186731721123014"><td class="cellrowborder" valign="top" width="16.221622162216224%" headers="mcps1.2.5.1.1 "><p id="p216770371221"><a name="p216770371221"></a><a name="p216770371221"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="17.311731173117312%" headers="mcps1.2.5.1.2 "><p id="p110096061221"><a name="p110096061221"></a><a name="p110096061221"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.981798179817982%" headers="mcps1.2.5.1.3 "><p id="p193628991221"><a name="p193628991221"></a><a name="p193628991221"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p248910051221"><a name="p248910051221"></a><a name="p248910051221"></a>资源标签。</p>
<p id="p226924561221"><a name="p226924561221"></a><a name="p226924561221"></a>取值格式：key1,value1|key2,value2</p>
<p id="p40552875114139"><a name="p40552875114139"></a><a name="p40552875114139"></a>多个标签之间用"|"分开，每个标签的键值用英文逗号","相隔。</p>
<p id="p29055151221"><a name="p29055151221"></a><a name="p29055151221"></a>多个标签之间为“与”的关系。</p>
<p id="p59717447115129"><a name="p59717447115129"></a><a name="p59717447115129"></a>关于资源标签，请参见<a href="添加资源标签.md">添加资源标签</a>。</p>
<p id="p1770514714203"><a name="p1770514714203"></a><a name="p1770514714203"></a>搜索模式为精确搜索。如果资源标签值value是以*开头时，则按照*后面的值全模糊匹配。</p>
<p id="p71284149127"><a name="p71284149127"></a><a name="p71284149127"></a>默认值为空。</p>
</td>
</tr>
<tr id="row1860117192306"><td class="cellrowborder" valign="top" width="16.221622162216224%" headers="mcps1.2.5.1.1 "><p id="p77524811122"><a name="p77524811122"></a><a name="p77524811122"></a></p>
<p id="p15187431105515"><a name="p15187431105515"></a><a name="p15187431105515"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="17.311731173117312%" headers="mcps1.2.5.1.2 "><p id="p21877311559"><a name="p21877311559"></a><a name="p21877311559"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.981798179817982%" headers="mcps1.2.5.1.3 "><p id="p18187143110551"><a name="p18187143110551"></a><a name="p18187143110551"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p181873314559"><a name="p181873314559"></a><a name="p181873314559"></a>待查询的Record Set的状态。</p>
<p id="p447517111159"><a name="p447517111159"></a><a name="p447517111159"></a>取值范围：ACTIVE、ERROR、DISABLE、FREEZE、PENDING_CREATE、PENDING_UPDATE、PENDING_DELETE</p>
<p id="p1641444019533"><a name="p1641444019533"></a><a name="p1641444019533"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
<p id="p1289715373203"><a name="p1289715373203"></a><a name="p1289715373203"></a>搜索模式默认为模糊搜索。</p>
<p id="p1135030171215"><a name="p1135030171215"></a><a name="p1135030171215"></a>默认值为空。</p>
</td>
</tr>
<tr id="row667218174302"><td class="cellrowborder" valign="top" width="16.221622162216224%" headers="mcps1.2.5.1.1 "><p id="p4998111210116"><a name="p4998111210116"></a><a name="p4998111210116"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="17.311731173117312%" headers="mcps1.2.5.1.2 "><p id="p89981512101120"><a name="p89981512101120"></a><a name="p89981512101120"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.981798179817982%" headers="mcps1.2.5.1.3 "><p id="p399821215119"><a name="p399821215119"></a><a name="p399821215119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p109982012141111"><a name="p109982012141111"></a><a name="p109982012141111"></a>待查询的Record Set的记录集类型。</p>
<p id="p20817123416132"><a name="p20817123416132"></a><a name="p20817123416132"></a>取值范围：A、AAAA、MX、CNAME、TXT、NS（仅限公网Zone）、SRV、PTR（仅限内网Zone）、CAA（仅限公网Zone）。</p>
<p id="p111997895417"><a name="p111997895417"></a><a name="p111997895417"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a>。</p>
<p id="p13289122841911"><a name="p13289122841911"></a><a name="p13289122841911"></a>搜索模式固定为精确搜索。</p>
<p id="p8193193917127"><a name="p8193193917127"></a><a name="p8193193917127"></a>默认值为空。</p>
</td>
</tr>
<tr id="row17597315113020"><td class="cellrowborder" valign="top" width="16.221622162216224%" headers="mcps1.2.5.1.1 "><p id="p189276527168"><a name="p189276527168"></a><a name="p189276527168"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="17.311731173117312%" headers="mcps1.2.5.1.2 "><p id="p19927752151617"><a name="p19927752151617"></a><a name="p19927752151617"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.981798179817982%" headers="mcps1.2.5.1.3 "><p id="p1492719522167"><a name="p1492719522167"></a><a name="p1492719522167"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p11927252121613"><a name="p11927252121613"></a><a name="p11927252121613"></a>待查询的Record Set的域名中包含此name。</p>
<p id="p16251111519186"><a name="p16251111519186"></a><a name="p16251111519186"></a>搜索模式默认为模糊搜索。</p>
<p id="p1242174471218"><a name="p1242174471218"></a><a name="p1242174471218"></a>默认值为空。</p>
</td>
</tr>
<tr id="row17376313103015"><td class="cellrowborder" valign="top" width="16.221622162216224%" headers="mcps1.2.5.1.1 "><p id="p13604691913"><a name="p13604691913"></a><a name="p13604691913"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.311731173117312%" headers="mcps1.2.5.1.2 "><p id="p15360960192"><a name="p15360960192"></a><a name="p15360960192"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.981798179817982%" headers="mcps1.2.5.1.3 "><p id="p4360869195"><a name="p4360869195"></a><a name="p4360869195"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p173609610193"><a name="p173609610193"></a><a name="p173609610193"></a>待查询的Record Set的id包含此id。</p>
<p id="p20802163115183"><a name="p20802163115183"></a><a name="p20802163115183"></a>搜索模式默认为模糊搜索。</p>
<p id="p19284124741213"><a name="p19284124741213"></a><a name="p19284124741213"></a>默认值为空。</p>
</td>
</tr>
<tr id="row178226411313"><td class="cellrowborder" valign="top" width="16.221622162216224%" headers="mcps1.2.5.1.1 "><p id="p464071413114"><a name="p464071413114"></a><a name="p464071413114"></a>sort_key</p>
</td>
<td class="cellrowborder" valign="top" width="17.311731173117312%" headers="mcps1.2.5.1.2 "><p id="p76401414163117"><a name="p76401414163117"></a><a name="p76401414163117"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.981798179817982%" headers="mcps1.2.5.1.3 "><p id="p166419143319"><a name="p166419143319"></a><a name="p166419143319"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p764161483117"><a name="p764161483117"></a><a name="p764161483117"></a>查询结果中Record Set列表的排序字段。</p>
<p id="p14641814193118"><a name="p14641814193118"></a><a name="p14641814193118"></a>取值范围为：</p>
<a name="ul1864191483114"></a><a name="ul1864191483114"></a><ul id="ul1864191483114"><li>name：域名</li><li>type：记录集类型</li></ul>
<p id="p1164171483115"><a name="p1164171483115"></a><a name="p1164171483115"></a>默认值为空，表示不排序。</p>
</td>
</tr>
<tr id="row114021662226"><td class="cellrowborder" valign="top" width="16.221622162216224%" headers="mcps1.2.5.1.1 "><p id="p208891026103817"><a name="p208891026103817"></a><a name="p208891026103817"></a>sort_dir</p>
</td>
<td class="cellrowborder" valign="top" width="17.311731173117312%" headers="mcps1.2.5.1.2 "><p id="p4889162653813"><a name="p4889162653813"></a><a name="p4889162653813"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.981798179817982%" headers="mcps1.2.5.1.3 "><p id="p128891626133813"><a name="p128891626133813"></a><a name="p128891626133813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p116071347131216"><a name="p116071347131216"></a><a name="p116071347131216"></a>查询结果中Record Set列表的排序方式。</p>
<p id="p199381616161315"><a name="p199381616161315"></a><a name="p199381616161315"></a>取值范围：</p>
<a name="ul15224144943012"></a><a name="ul15224144943012"></a><ul id="ul15224144943012"><li>desc：降序排序</li><li>asc：升序排序</li></ul>
<p id="p15614185443318"><a name="p15614185443318"></a><a name="p15614185443318"></a>默认值为空，表示不排序。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section8612359"></a>

-   请求参数

    无

-   请求样例

    查询Zone ID为“2c9eb155587194ec01587224c9f90149”的域名的记录集列表。

    ```
    GET https://{DNS_Endpoint}/v2/zones/2c9eb155587194ec01587224c9f90149/recordsets?limit=&offset=
    ```


## 响应<a name="section10402369"></a>

-   要素说明

    **表 2**  响应样例的要素说明

    <a name="table53402119"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0037129969_row41580444"><th class="cellrowborder" valign="top" width="18.85%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0037129969_p12572829"><a name="zh-cn_topic_0037129969_p12572829"></a><a name="zh-cn_topic_0037129969_p12572829"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.54%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0037129969_p13543581"><a name="zh-cn_topic_0037129969_p13543581"></a><a name="zh-cn_topic_0037129969_p13543581"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.61%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0037129969_p23288300"><a name="zh-cn_topic_0037129969_p23288300"></a><a name="zh-cn_topic_0037129969_p23288300"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1945012598719"><td class="cellrowborder" valign="top" width="18.85%" headers="mcps1.2.4.1.1 "><p id="a8779f70c5dc4414c8df0c2950001a653"><a name="a8779f70c5dc4414c8df0c2950001a653"></a><a name="a8779f70c5dc4414c8df0c2950001a653"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.2 "><p id="a51104ec0822b4bf4bf9018680539141a"><a name="a51104ec0822b4bf4bf9018680539141a"></a><a name="a51104ec0822b4bf4bf9018680539141a"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.61%" headers="mcps1.2.4.1.3 "><p id="aa2a07c69de424ee5bd26b246f46c26c1"><a name="aa2a07c69de424ee5bd26b246f46c26c1"></a><a name="aa2a07c69de424ee5bd26b246f46c26c1"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p1226974804620"><a name="p1226974804620"></a><a name="p1226974804620"></a>详细信息请参见<a href="#table354521744216">表5</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129969_row7304143"><td class="cellrowborder" valign="top" width="18.85%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129969_p54764719"><a name="zh-cn_topic_0037129969_p54764719"></a><a name="zh-cn_topic_0037129969_p54764719"></a>recordsets</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129969_p10465156"><a name="zh-cn_topic_0037129969_p10465156"></a><a name="zh-cn_topic_0037129969_p10465156"></a>Array of object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.61%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129969_p45797138"><a name="zh-cn_topic_0037129969_p45797138"></a><a name="zh-cn_topic_0037129969_p45797138"></a>recordset列表对象，详细信息请参见<a href="#table7192645154740">表3</a>。</p>
    </td>
    </tr>
    <tr id="ra36d54752ed44415a573a743060b4dc8"><td class="cellrowborder" valign="top" width="18.85%" headers="mcps1.2.4.1.1 "><p id="acfae956c5b3948318d1c49c7521cace4"><a name="acfae956c5b3948318d1c49c7521cace4"></a><a name="acfae956c5b3948318d1c49c7521cace4"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.2 "><p id="aef6bb96f7ac64bef8949bb9d76432fd4"><a name="aef6bb96f7ac64bef8949bb9d76432fd4"></a><a name="aef6bb96f7ac64bef8949bb9d76432fd4"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.61%" headers="mcps1.2.4.1.3 "><p id="aa2edc4c85ec14e53bf99f656877a8cb6"><a name="aa2edc4c85ec14e53bf99f656877a8cb6"></a><a name="aa2edc4c85ec14e53bf99f656877a8cb6"></a>返回满足过滤条件的资源总数，详细信息请参见<a href="#table2908319718932">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  recordsets字段说明

    <a name="table7192645154740"></a>
    <table><thead align="left"><tr id="r0af5587c948d46d8a15423493000e6e3"><th class="cellrowborder" valign="top" width="18.43%" id="mcps1.2.4.1.1"><p id="a8adba83845e444c7bf910c07317dc670"><a name="a8adba83845e444c7bf910c07317dc670"></a><a name="a8adba83845e444c7bf910c07317dc670"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.05%" id="mcps1.2.4.1.2"><p id="abe1dbdba2c604202aafd8faf8c3cfeb1"><a name="abe1dbdba2c604202aafd8faf8c3cfeb1"></a><a name="abe1dbdba2c604202aafd8faf8c3cfeb1"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.519999999999996%" id="mcps1.2.4.1.3"><p id="aa6b52f60e9a745cbb6d91de6da250130"><a name="aa6b52f60e9a745cbb6d91de6da250130"></a><a name="aa6b52f60e9a745cbb6d91de6da250130"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r15a90d66e19644d2b048f68e4641dfbd"><td class="cellrowborder" valign="top" width="18.43%" headers="mcps1.2.4.1.1 "><p id="a4cf2a527bdf54c9aa9f24774cb97d3ef"><a name="a4cf2a527bdf54c9aa9f24774cb97d3ef"></a><a name="a4cf2a527bdf54c9aa9f24774cb97d3ef"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.2 "><p id="a54396be1dd35484ea5bbb76c4a6a97c5"><a name="a54396be1dd35484ea5bbb76c4a6a97c5"></a><a name="a54396be1dd35484ea5bbb76c4a6a97c5"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.519999999999996%" headers="mcps1.2.4.1.3 "><p id="afd5e43bb0e5a4e21b27c223a3d6fede5"><a name="afd5e43bb0e5a4e21b27c223a3d6fede5"></a><a name="afd5e43bb0e5a4e21b27c223a3d6fede5"></a>Record Set的ID。</p>
    </td>
    </tr>
    <tr id="rd729baffede54ccc905a7b1ba90560d2"><td class="cellrowborder" valign="top" width="18.43%" headers="mcps1.2.4.1.1 "><p id="aa48e4bbb14d640888bc92cc4f5099114"><a name="aa48e4bbb14d640888bc92cc4f5099114"></a><a name="aa48e4bbb14d640888bc92cc4f5099114"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.2 "><p id="a64dc6625596f4cc1b4009afad4ffd978"><a name="a64dc6625596f4cc1b4009afad4ffd978"></a><a name="a64dc6625596f4cc1b4009afad4ffd978"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.519999999999996%" headers="mcps1.2.4.1.3 "><p id="a8431a47b4d684b84a8892686d49572a1"><a name="a8431a47b4d684b84a8892686d49572a1"></a><a name="a8431a47b4d684b84a8892686d49572a1"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="rf79f0ca4f9984aa095a1cd76e6eb67c4"><td class="cellrowborder" valign="top" width="18.43%" headers="mcps1.2.4.1.1 "><p id="ace30dcdf68ff463f85024b388cb4e90b"><a name="ace30dcdf68ff463f85024b388cb4e90b"></a><a name="ace30dcdf68ff463f85024b388cb4e90b"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.2 "><p id="ac14bda5751f247fc86b91f168ce4d8c0"><a name="ac14bda5751f247fc86b91f168ce4d8c0"></a><a name="ac14bda5751f247fc86b91f168ce4d8c0"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.519999999999996%" headers="mcps1.2.4.1.3 "><p id="a6e545c57b85a45adb0b6e47b27332ebc"><a name="a6e545c57b85a45adb0b6e47b27332ebc"></a><a name="a6e545c57b85a45adb0b6e47b27332ebc"></a>Record Set的描述信息。</p>
    </td>
    </tr>
    <tr id="r9f4660e6890545df864cf94d9226d1eb"><td class="cellrowborder" valign="top" width="18.43%" headers="mcps1.2.4.1.1 "><p id="a5c1a273d855c4198abadda4ac5e784b7"><a name="a5c1a273d855c4198abadda4ac5e784b7"></a><a name="a5c1a273d855c4198abadda4ac5e784b7"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.2 "><p id="ab84442897fc845ab8bcbb24947f8e943"><a name="ab84442897fc845ab8bcbb24947f8e943"></a><a name="ab84442897fc845ab8bcbb24947f8e943"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.519999999999996%" headers="mcps1.2.4.1.3 "><p id="a5abdb6f7c1d1497babfdc68ce867b937"><a name="a5abdb6f7c1d1497babfdc68ce867b937"></a><a name="a5abdb6f7c1d1497babfdc68ce867b937"></a>托管该记录的zone_id。</p>
    </td>
    </tr>
    <tr id="r5b8f62b5503b42c0a76565e98b01f37d"><td class="cellrowborder" valign="top" width="18.43%" headers="mcps1.2.4.1.1 "><p id="a97bb7c3123ed4896b410b56fb8b1a6e8"><a name="a97bb7c3123ed4896b410b56fb8b1a6e8"></a><a name="a97bb7c3123ed4896b410b56fb8b1a6e8"></a>zone_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.2 "><p id="ad4c239292930467d8bd59f801a2d29e2"><a name="ad4c239292930467d8bd59f801a2d29e2"></a><a name="ad4c239292930467d8bd59f801a2d29e2"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.519999999999996%" headers="mcps1.2.4.1.3 "><p id="a0baf79ddce9f4dd7afdb0516ebb6da1e"><a name="a0baf79ddce9f4dd7afdb0516ebb6da1e"></a><a name="a0baf79ddce9f4dd7afdb0516ebb6da1e"></a>托管该记录的zone_name。</p>
    </td>
    </tr>
    <tr id="r47e64be1e24d4566b613ceadf1051ca0"><td class="cellrowborder" valign="top" width="18.43%" headers="mcps1.2.4.1.1 "><p id="aa3fbb0a6ce484e64963d2e66d18c0d66"><a name="aa3fbb0a6ce484e64963d2e66d18c0d66"></a><a name="aa3fbb0a6ce484e64963d2e66d18c0d66"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.2 "><p id="a0b4010d60b6b47d1be3e8ce3e44e3a36"><a name="a0b4010d60b6b47d1be3e8ce3e44e3a36"></a><a name="a0b4010d60b6b47d1be3e8ce3e44e3a36"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.519999999999996%" headers="mcps1.2.4.1.3 "><p id="a10d6bdb86d61410f8ccad0af27bf792b"><a name="a10d6bdb86d61410f8ccad0af27bf792b"></a><a name="a10d6bdb86d61410f8ccad0af27bf792b"></a>记录类型。</p>
    <p id="p1250112591212"><a name="p1250112591212"></a><a name="p1250112591212"></a>取值范围：A、AAAA、MX、CNAME、TXT、NS（仅限公网Zone）、SRV、PTR（仅限内网Zone）、CAA（仅限公网Zone）。</p>
    <p id="a198eb45dfea94fcfa777300551454179"><a name="a198eb45dfea94fcfa777300551454179"></a><a name="a198eb45dfea94fcfa777300551454179"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a>。</p>
    </td>
    </tr>
    <tr id="rc3c113a38d8b40e19629963991179111"><td class="cellrowborder" valign="top" width="18.43%" headers="mcps1.2.4.1.1 "><p id="af8f682bd90344203ba4319cb9329cd89"><a name="af8f682bd90344203ba4319cb9329cd89"></a><a name="af8f682bd90344203ba4319cb9329cd89"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.2 "><p id="abad6db87f732458d8b436c12a3210c88"><a name="abad6db87f732458d8b436c12a3210c88"></a><a name="abad6db87f732458d8b436c12a3210c88"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.519999999999996%" headers="mcps1.2.4.1.3 "><p id="p123031523174010"><a name="p123031523174010"></a><a name="p123031523174010"></a>解析记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="p1030317233408"><a name="p1030317233408"></a><a name="p1030317233408"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    </td>
    </tr>
    <tr id="r37b3fbaa743244edae92887f7a85879b"><td class="cellrowborder" valign="top" width="18.43%" headers="mcps1.2.4.1.1 "><p id="a58ffd09b95b745cea54e9c25ccb21394"><a name="a58ffd09b95b745cea54e9c25ccb21394"></a><a name="a58ffd09b95b745cea54e9c25ccb21394"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.2 "><p id="a2ae8cb48a17a4626b53ac823c85dcb6f"><a name="a2ae8cb48a17a4626b53ac823c85dcb6f"></a><a name="a2ae8cb48a17a4626b53ac823c85dcb6f"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.519999999999996%" headers="mcps1.2.4.1.3 "><p id="aaa856de208d9486988e40aec9b072136"><a name="aaa856de208d9486988e40aec9b072136"></a><a name="aaa856de208d9486988e40aec9b072136"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="r8ce69e869cbe4417ad700242f7a60a1a"><td class="cellrowborder" valign="top" width="18.43%" headers="mcps1.2.4.1.1 "><p id="a3403f8ba9df44877b57d6b5b4864068f"><a name="a3403f8ba9df44877b57d6b5b4864068f"></a><a name="a3403f8ba9df44877b57d6b5b4864068f"></a>create_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.2 "><p id="p187131431990"><a name="p187131431990"></a><a name="p187131431990"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.519999999999996%" headers="mcps1.2.4.1.3 "><p id="ab6b8bf53dcfe4f50bd881bffeb86a75c"><a name="ab6b8bf53dcfe4f50bd881bffeb86a75c"></a><a name="ab6b8bf53dcfe4f50bd881bffeb86a75c"></a>创建时间。</p>
    <p id="a881c9a18b1e24097982dd0f94686438a"><a name="a881c9a18b1e24097982dd0f94686438a"></a><a name="a881c9a18b1e24097982dd0f94686438a"></a>格式：yyyy-MM-dd'T'HH:mm:ss.SSS</p>
    </td>
    </tr>
    <tr id="r38927cc028a6493ea14200a215beb5f1"><td class="cellrowborder" valign="top" width="18.43%" headers="mcps1.2.4.1.1 "><p id="a43961341d5e443e2ae5e866b72ec3639"><a name="a43961341d5e443e2ae5e866b72ec3639"></a><a name="a43961341d5e443e2ae5e866b72ec3639"></a>update_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.2 "><p id="p3597341393"><a name="p3597341393"></a><a name="p3597341393"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.519999999999996%" headers="mcps1.2.4.1.3 "><p id="a3b09a9724a904bdb9d9748d27a14e66c"><a name="a3b09a9724a904bdb9d9748d27a14e66c"></a><a name="a3b09a9724a904bdb9d9748d27a14e66c"></a>更新时间。</p>
    <p id="af325deb1a55e4a66b5ab735f2f65f9af"><a name="af325deb1a55e4a66b5ab735f2f65f9af"></a><a name="af325deb1a55e4a66b5ab735f2f65f9af"></a>格式：yyyy-MM-dd'T'HH:mm:ss.SSS</p>
    </td>
    </tr>
    <tr id="r57ca2c0e85e948dfaf58836f4276aeca"><td class="cellrowborder" valign="top" width="18.43%" headers="mcps1.2.4.1.1 "><p id="ae00da26584744a278669ea88c1fe481c"><a name="ae00da26584744a278669ea88c1fe481c"></a><a name="ae00da26584744a278669ea88c1fe481c"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.2 "><p id="a99a92dbdb2b74fa89c839212003e4864"><a name="a99a92dbdb2b74fa89c839212003e4864"></a><a name="a99a92dbdb2b74fa89c839212003e4864"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.519999999999996%" headers="mcps1.2.4.1.3 "><p id="a45bfe41a9b8144d5828355752733d3b3"><a name="a45bfe41a9b8144d5828355752733d3b3"></a><a name="a45bfe41a9b8144d5828355752733d3b3"></a>资源状态。</p>
    <p id="a60294dc7e1334baba4d2a3444e020149"><a name="a60294dc7e1334baba4d2a3444e020149"></a><a name="a60294dc7e1334baba4d2a3444e020149"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="ra70a82e3577641c48bfff967011a70bb"><td class="cellrowborder" valign="top" width="18.43%" headers="mcps1.2.4.1.1 "><p id="a4cea4ca8281e4ddfb3a451c3228e16c3"><a name="a4cea4ca8281e4ddfb3a451c3228e16c3"></a><a name="a4cea4ca8281e4ddfb3a451c3228e16c3"></a>default</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.2 "><p id="a57ca2db911824c6ab1b680c44335b29e"><a name="a57ca2db911824c6ab1b680c44335b29e"></a><a name="a57ca2db911824c6ab1b680c44335b29e"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.519999999999996%" headers="mcps1.2.4.1.3 "><p id="a7605345fc0f041309ebaa93830fc5e85"><a name="a7605345fc0f041309ebaa93830fc5e85"></a><a name="a7605345fc0f041309ebaa93830fc5e85"></a>标识是否由系统默认生成，系统默认生成的Record Set不能删除。</p>
    </td>
    </tr>
    <tr id="re0ed521efcfb40b3a38e94bf58839201"><td class="cellrowborder" valign="top" width="18.43%" headers="mcps1.2.4.1.1 "><p id="ac9cfd75452ed4da39c94d7a166290d5b"><a name="ac9cfd75452ed4da39c94d7a166290d5b"></a><a name="ac9cfd75452ed4da39c94d7a166290d5b"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.2 "><p id="p11871840396"><a name="p11871840396"></a><a name="p11871840396"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.519999999999996%" headers="mcps1.2.4.1.3 "><p id="p4619625201026"><a name="p4619625201026"></a><a name="p4619625201026"></a>该Record Set所属的项目ID。</p>
    </td>
    </tr>
    <tr id="r0bab22234ef44171aff1b23e500b514a"><td class="cellrowborder" valign="top" width="18.43%" headers="mcps1.2.4.1.1 "><p id="a807f36408ce243a49010e2a04724a3b7"><a name="a807f36408ce243a49010e2a04724a3b7"></a><a name="a807f36408ce243a49010e2a04724a3b7"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.2 "><p id="afdf3844ea44b4f758b42ffdb2e0064ef"><a name="afdf3844ea44b4f758b42ffdb2e0064ef"></a><a name="afdf3844ea44b4f758b42ffdb2e0064ef"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.519999999999996%" headers="mcps1.2.4.1.3 "><p id="a083445bf634e4e0f977c92b1b0bb1863"><a name="a083445bf634e4e0f977c92b1b0bb1863"></a><a name="a083445bf634e4e0f977c92b1b0bb1863"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p14501402474"><a name="p14501402474"></a><a name="p14501402474"></a>详细信息请参见<a href="#table354521744216">表5</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  metadata参数说明

    <a name="table2908319718932"></a>
    <table><thead align="left"><tr id="r1ee98e923a7c4bfcaa89e708d3fca79e"><th class="cellrowborder" valign="top" width="18.33183318331833%" id="mcps1.2.4.1.1"><p id="af493c2fde22f44069c2b5ea0467dfe89"><a name="af493c2fde22f44069c2b5ea0467dfe89"></a><a name="af493c2fde22f44069c2b5ea0467dfe89"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.46194619461946%" id="mcps1.2.4.1.2"><p id="a581940a484df4c8294e51f11391a23c8"><a name="a581940a484df4c8294e51f11391a23c8"></a><a name="a581940a484df4c8294e51f11391a23c8"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.206220622062204%" id="mcps1.2.4.1.3"><p id="a0301bbf5a1234ea3a88a104e1b4cff92"><a name="a0301bbf5a1234ea3a88a104e1b4cff92"></a><a name="a0301bbf5a1234ea3a88a104e1b4cff92"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r7cc02a0ecbd24482bca90faa98114b18"><td class="cellrowborder" valign="top" width="18.33183318331833%" headers="mcps1.2.4.1.1 "><p id="a9234858cb2f447539b4b85a307884322"><a name="a9234858cb2f447539b4b85a307884322"></a><a name="a9234858cb2f447539b4b85a307884322"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46194619461946%" headers="mcps1.2.4.1.2 "><p id="af14a2a2c8f0345f4811bb21dd2a9b667"><a name="af14a2a2c8f0345f4811bb21dd2a9b667"></a><a name="af14a2a2c8f0345f4811bb21dd2a9b667"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.206220622062204%" headers="mcps1.2.4.1.3 "><p id="a39058f9901c84eb9a776ca5cd44ede29"><a name="a39058f9901c84eb9a776ca5cd44ede29"></a><a name="a39058f9901c84eb9a776ca5cd44ede29"></a>满足查询条件的资源总数，不受分页（即limit、offset参数）影响。</p>
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
    <tr id="row175243399495"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
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
            "self": "https://Endpoint/v2/recordsets?limit=1&marker=&name=&status=&zone_id=2c9eb155587194ec01587224c9f90149",
            "next": "https://Endpoint/v2/recordsets?limit=11&marker=2c9eb155587194ec01587224c9f9014a&name=&status=&zone_id=2c9eb155587194ec01587224c9f90149"
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
                    "self": "https://Endpoint/v2/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587194ec01587224c9f9014a"
                },
                "zone_id": "2c9eb155587194ec01587224c9f90149",
                "zone_name": "example.com.",
                "create_at": "2016-11-17T11:56:03.439",
                "update_at": "2016-11-17T12:56:03.827",
                "default": true,
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c"
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
                    "self": "https://Endpoint/v2/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587194ec01587224c9f9014c"
                },
                "zone_id": "2c9eb155587194ec01587224c9f90149",
                "zone_name": "example.com.",
                "create_at": "2016-11-17T11:56:03.439",
                "update_at": "2016-11-17T12:56:03.827",
                "default": true,
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c"
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
                    "self": "https://Endpoint/v2/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587228570158722b6ac30007"
                },
                "zone_id": "2c9eb155587194ec01587224c9f90149",
                "zone_name": "example.com.",
                "create_at": "2016-11-17T12:03:17.827",
                "update_at": "2016-11-17T12:56:03.827",
                "default": false,
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c"
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

