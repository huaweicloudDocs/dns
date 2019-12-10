# 查询Record Set列表<a name="zh-cn_topic_0037129969"></a>

## 功能介绍<a name="section29105235"></a>

查询租户Record Set资源列表。

## URI<a name="section60620523"></a>

GET /v2/recordsets?zone\_type=\{zone\_type\}&limit=\{limit\}&marker=\{marker\}&offset=\{offset\}&tags=\{tags\}&status=\{status\}&type=\{type\}&name=\{name\}&id=\{id\}&records=\{records\}&sort\_key=\{sort\_key\}&sort\_dir=\{sort\_dir\}

参数说明请参见[表1](#table40248354)。

**表 1**  URI格式的参数说明

<a name="table40248354"></a>
<table><thead align="left"><tr id="row24110047"><th class="cellrowborder" valign="top" width="16.321632163216325%" id="mcps1.2.5.1.1"><p id="p6756797"><a name="p6756797"></a><a name="p6756797"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.121612161216124%" id="mcps1.2.5.1.2"><p id="p10429724"><a name="p10429724"></a><a name="p10429724"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.511751175117514%" id="mcps1.2.5.1.3"><p id="p39501348"><a name="p39501348"></a><a name="p39501348"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50.04500450045004%" id="mcps1.2.5.1.4"><p id="p45492604"><a name="p45492604"></a><a name="p45492604"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row67046586114158"><td class="cellrowborder" valign="top" width="16.321632163216325%" headers="mcps1.2.5.1.1 "><p id="p10129219114159"><a name="p10129219114159"></a><a name="p10129219114159"></a>zone_type</p>
</td>
<td class="cellrowborder" valign="top" width="16.121612161216124%" headers="mcps1.2.5.1.2 "><p id="p15160399114159"><a name="p15160399114159"></a><a name="p15160399114159"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.3 "><p id="p20032767114159"><a name="p20032767114159"></a><a name="p20032767114159"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.04500450045004%" headers="mcps1.2.5.1.4 "><p id="p12041403114159"><a name="p12041403114159"></a><a name="p12041403114159"></a>待查询的Record Set的域名类型。</p>
<p id="p41263770114159"><a name="p41263770114159"></a><a name="p41263770114159"></a>取值范围：public、private</p>
<a name="ul35829612114159"></a><a name="ul35829612114159"></a><ul id="ul35829612114159"><li>如果为空，表示查询公网类型的Record Set。</li><li>如果为public，表示查询公网类型的Record Set。</li><li>如果为private，表示查询内网类型的Record Set。</li></ul>
<p id="p89402038132417"><a name="p89402038132417"></a><a name="p89402038132417"></a>搜索模式默认为模糊搜索。</p>
<p id="p189098471136"><a name="p189098471136"></a><a name="p189098471136"></a>默认值为public。</p>
</td>
</tr>
<tr id="row61022284"><td class="cellrowborder" valign="top" width="16.321632163216325%" headers="mcps1.2.5.1.1 "><p id="p43857981"><a name="p43857981"></a><a name="p43857981"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="16.121612161216124%" headers="mcps1.2.5.1.2 "><p id="p62835574"><a name="p62835574"></a><a name="p62835574"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.3 "><p id="p56516768"><a name="p56516768"></a><a name="p56516768"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.04500450045004%" headers="mcps1.2.5.1.4 "><p id="p14455523"><a name="p14455523"></a><a name="p14455523"></a>分页查询起始的资源ID，为空时为查询第一页。</p>
<p id="p1426623319131"><a name="p1426623319131"></a><a name="p1426623319131"></a>默认值为空。</p>
</td>
</tr>
<tr id="row62990845"><td class="cellrowborder" valign="top" width="16.321632163216325%" headers="mcps1.2.5.1.1 "><p id="p1984791"><a name="p1984791"></a><a name="p1984791"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="16.121612161216124%" headers="mcps1.2.5.1.2 "><p id="p26550365"><a name="p26550365"></a><a name="p26550365"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.3 "><p id="p3095993"><a name="p3095993"></a><a name="p3095993"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.04500450045004%" headers="mcps1.2.5.1.4 "><p id="p230120311413"><a name="p230120311413"></a><a name="p230120311413"></a>每页返回的资源个数。</p>
<p id="p147131447514"><a name="p147131447514"></a><a name="p147131447514"></a>取值范围：0~500</p>
<p id="p1385813431412"><a name="p1385813431412"></a><a name="p1385813431412"></a>取值一般为10，20，50。默认值为500。</p>
</td>
</tr>
<tr id="row78856519552"><td class="cellrowborder" valign="top" width="16.321632163216325%" headers="mcps1.2.5.1.1 "><p id="p5702070419554"><a name="p5702070419554"></a><a name="p5702070419554"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="16.121612161216124%" headers="mcps1.2.5.1.2 "><p id="p5527430219554"><a name="p5527430219554"></a><a name="p5527430219554"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.3 "><p id="p4803348119554"><a name="p4803348119554"></a><a name="p4803348119554"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50.04500450045004%" headers="mcps1.2.5.1.4 "><p id="p35951433204916"><a name="p35951433204916"></a><a name="p35951433204916"></a>分页查询起始偏移量，表示从偏移量的下一个资源开始查询。</p>
<p id="p18898143914915"><a name="p18898143914915"></a><a name="p18898143914915"></a>取值范围：0~2147483647</p>
<p id="p13209172234718"><a name="p13209172234718"></a><a name="p13209172234718"></a>默认值为0。</p>
<p id="p167712216335"><a name="p167712216335"></a><a name="p167712216335"></a>当前设置marker不为空时，以marker为分页起始标识。</p>
</td>
</tr>
<tr id="row55044453115726"><td class="cellrowborder" valign="top" width="16.321632163216325%" headers="mcps1.2.5.1.1 "><p id="p216770371221"><a name="p216770371221"></a><a name="p216770371221"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="16.121612161216124%" headers="mcps1.2.5.1.2 "><p id="p110096061221"><a name="p110096061221"></a><a name="p110096061221"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.3 "><p id="p193628991221"><a name="p193628991221"></a><a name="p193628991221"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.04500450045004%" headers="mcps1.2.5.1.4 "><p id="p248910051221"><a name="p248910051221"></a><a name="p248910051221"></a>资源标签。</p>
<p id="p226924561221"><a name="p226924561221"></a><a name="p226924561221"></a>取值格式：key1,value1|key2,value2</p>
<p id="p40552875114139"><a name="p40552875114139"></a><a name="p40552875114139"></a>多个标签之间用"|"分开，每个标签的键值用英文逗号","相隔。</p>
<p id="p29055151221"><a name="p29055151221"></a><a name="p29055151221"></a>多个标签之间为“与”的关系。</p>
<p id="p59717447115129"><a name="p59717447115129"></a><a name="p59717447115129"></a>关于资源标签，请参见<a href="添加资源标签.md">添加资源标签</a>。</p>
<p id="p1770514714203"><a name="p1770514714203"></a><a name="p1770514714203"></a>搜索模式为精确搜索。如果资源标签值value是以*开头时，则按照*后面的值全模糊匹配。</p>
<p id="p71284149127"><a name="p71284149127"></a><a name="p71284149127"></a>默认值为空。</p>
</td>
</tr>
<tr id="row91871931125514"><td class="cellrowborder" valign="top" width="16.321632163216325%" headers="mcps1.2.5.1.1 "><p id="p77524811122"><a name="p77524811122"></a><a name="p77524811122"></a></p>
<p id="p15187431105515"><a name="p15187431105515"></a><a name="p15187431105515"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="16.121612161216124%" headers="mcps1.2.5.1.2 "><p id="p21877311559"><a name="p21877311559"></a><a name="p21877311559"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.3 "><p id="p18187143110551"><a name="p18187143110551"></a><a name="p18187143110551"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.04500450045004%" headers="mcps1.2.5.1.4 "><p id="p181873314559"><a name="p181873314559"></a><a name="p181873314559"></a>待查询的Record Set的状态。</p>
<p id="p447517111159"><a name="p447517111159"></a><a name="p447517111159"></a>取值范围：ACTIVE、ERROR、DISABLE、FREEZE、PENDING_CREATE、PENDING_UPDATE、PENDING_DELETE</p>
<p id="p1641444019533"><a name="p1641444019533"></a><a name="p1641444019533"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
<p id="p1289715373203"><a name="p1289715373203"></a><a name="p1289715373203"></a>搜索模式默认为模糊搜索。</p>
<p id="p1135030171215"><a name="p1135030171215"></a><a name="p1135030171215"></a>默认值为空。</p>
</td>
</tr>
<tr id="row1799821219113"><td class="cellrowborder" valign="top" width="16.321632163216325%" headers="mcps1.2.5.1.1 "><p id="p4998111210116"><a name="p4998111210116"></a><a name="p4998111210116"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="16.121612161216124%" headers="mcps1.2.5.1.2 "><p id="p89981512101120"><a name="p89981512101120"></a><a name="p89981512101120"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.3 "><p id="p399821215119"><a name="p399821215119"></a><a name="p399821215119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.04500450045004%" headers="mcps1.2.5.1.4 "><p id="p109982012141111"><a name="p109982012141111"></a><a name="p109982012141111"></a>待查询的Record Set的记录集类型。</p>
<p id="p20817123416132"><a name="p20817123416132"></a><a name="p20817123416132"></a>取值范围：A、CNAME、MX、AAAA、TXT、SRV、NS、CAA，PTR（仅限内网Zone）</p>
<p id="p111997895417"><a name="p111997895417"></a><a name="p111997895417"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a></p>
<p id="p13289122841911"><a name="p13289122841911"></a><a name="p13289122841911"></a>搜索模式固定为精确搜索。</p>
<p id="p8193193917127"><a name="p8193193917127"></a><a name="p8193193917127"></a>默认值为空。</p>
</td>
</tr>
<tr id="row11927135213161"><td class="cellrowborder" valign="top" width="16.321632163216325%" headers="mcps1.2.5.1.1 "><p id="p189276527168"><a name="p189276527168"></a><a name="p189276527168"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16.121612161216124%" headers="mcps1.2.5.1.2 "><p id="p19927752151617"><a name="p19927752151617"></a><a name="p19927752151617"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.3 "><p id="p1492719522167"><a name="p1492719522167"></a><a name="p1492719522167"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.04500450045004%" headers="mcps1.2.5.1.4 "><p id="p11927252121613"><a name="p11927252121613"></a><a name="p11927252121613"></a>待查询的Record Set的域名中包含此name。</p>
<p id="p16251111519186"><a name="p16251111519186"></a><a name="p16251111519186"></a>搜索模式默认为模糊搜索。</p>
<p id="p1242174471218"><a name="p1242174471218"></a><a name="p1242174471218"></a>默认值为空。</p>
</td>
</tr>
<tr id="row33603617197"><td class="cellrowborder" valign="top" width="16.321632163216325%" headers="mcps1.2.5.1.1 "><p id="p13604691913"><a name="p13604691913"></a><a name="p13604691913"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.121612161216124%" headers="mcps1.2.5.1.2 "><p id="p15360960192"><a name="p15360960192"></a><a name="p15360960192"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.3 "><p id="p4360869195"><a name="p4360869195"></a><a name="p4360869195"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.04500450045004%" headers="mcps1.2.5.1.4 "><p id="p173609610193"><a name="p173609610193"></a><a name="p173609610193"></a>待查询的Record Set的id包含此id。</p>
<p id="p20802163115183"><a name="p20802163115183"></a><a name="p20802163115183"></a>搜索模式默认为模糊搜索。</p>
<p id="p19284124741213"><a name="p19284124741213"></a><a name="p19284124741213"></a>默认值为空。</p>
</td>
</tr>
<tr id="row191263112211"><td class="cellrowborder" valign="top" width="16.321632163216325%" headers="mcps1.2.5.1.1 "><p id="p112614115211"><a name="p112614115211"></a><a name="p112614115211"></a>records</p>
</td>
<td class="cellrowborder" valign="top" width="16.121612161216124%" headers="mcps1.2.5.1.2 "><p id="p81261211182110"><a name="p81261211182110"></a><a name="p81261211182110"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.3 "><p id="p131261311192119"><a name="p131261311192119"></a><a name="p131261311192119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.04500450045004%" headers="mcps1.2.5.1.4 "><p id="p260972615213"><a name="p260972615213"></a><a name="p260972615213"></a>待查询的Record Set的值中包含此records。</p>
<p id="p64731727196"><a name="p64731727196"></a><a name="p64731727196"></a>搜索模式默认为模糊搜索。</p>
<p id="p6571155011120"><a name="p6571155011120"></a><a name="p6571155011120"></a>默认值为空。</p>
</td>
</tr>
<tr id="row6672923143613"><td class="cellrowborder" valign="top" width="16.321632163216325%" headers="mcps1.2.5.1.1 "><p id="p15674182317363"><a name="p15674182317363"></a><a name="p15674182317363"></a>sort_key</p>
</td>
<td class="cellrowborder" valign="top" width="16.121612161216124%" headers="mcps1.2.5.1.2 "><p id="p206741223103614"><a name="p206741223103614"></a><a name="p206741223103614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.3 "><p id="p7674132316360"><a name="p7674132316360"></a><a name="p7674132316360"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.04500450045004%" headers="mcps1.2.5.1.4 "><p id="p4674182316366"><a name="p4674182316366"></a><a name="p4674182316366"></a>查询结果中Record Set列表的排序字段。</p>
<p id="p161032135113"><a name="p161032135113"></a><a name="p161032135113"></a>取值范围：</p>
<a name="ul1181955993116"></a><a name="ul1181955993116"></a><ul id="ul1181955993116"><li>name：域名</li><li>type：记录集类型</li></ul>
<p id="p980118577128"><a name="p980118577128"></a><a name="p980118577128"></a>默认值为空，表示不排序。</p>
</td>
</tr>
<tr id="row11889126183816"><td class="cellrowborder" valign="top" width="16.321632163216325%" headers="mcps1.2.5.1.1 "><p id="p208891026103817"><a name="p208891026103817"></a><a name="p208891026103817"></a>sort_dir</p>
</td>
<td class="cellrowborder" valign="top" width="16.121612161216124%" headers="mcps1.2.5.1.2 "><p id="p4889162653813"><a name="p4889162653813"></a><a name="p4889162653813"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.511751175117514%" headers="mcps1.2.5.1.3 "><p id="p128891626133813"><a name="p128891626133813"></a><a name="p128891626133813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.04500450045004%" headers="mcps1.2.5.1.4 "><p id="p116071347131216"><a name="p116071347131216"></a><a name="p116071347131216"></a>查询结果中Record Set列表的排序方式。</p>
<p id="p749316343213"><a name="p749316343213"></a><a name="p749316343213"></a>取值范围：</p>
<a name="ul18204217325"></a><a name="ul18204217325"></a><ul id="ul18204217325"><li>desc：降序排序</li><li>asc：升序排序</li></ul>
<p id="p3562616138"><a name="p3562616138"></a><a name="p3562616138"></a>默认值为空，表示不排序。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section8713795"></a>

-   请求参数

    无

-   请求样例

    查询域名类型为公网，记录集类型为A，且域名包含“www.example.com”的域名的记录集列表。

    ```
    GET https://{DNS_Endpoint}/v2/recordsets?zone_type=&type=A&name=www.example.com
    ```


## 响应<a name="section11315292"></a>

-   要素说明

    **表 2**  响应样例的要素说明

    <a name="table21574462"></a>
    <table><thead align="left"><tr id="row41580444"><th class="cellrowborder" valign="top" width="17.71%" id="mcps1.2.4.1.1"><p id="p12572829"><a name="p12572829"></a><a name="p12572829"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p13543581"><a name="p13543581"></a><a name="p13543581"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.29%" id="mcps1.2.4.1.3"><p id="p23288300"><a name="p23288300"></a><a name="p23288300"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row986574513439"><td class="cellrowborder" valign="top" width="17.71%" headers="mcps1.2.4.1.1 "><p id="p977735394312"><a name="p977735394312"></a><a name="p977735394312"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1577785318438"><a name="p1577785318438"></a><a name="p1577785318438"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p1277713536436"><a name="p1277713536436"></a><a name="p1277713536436"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p197771536439"><a name="p197771536439"></a><a name="p197771536439"></a>详细信息请参见<a href="#table354521744216">表5</a>。</p>
    </td>
    </tr>
    <tr id="row7304143"><td class="cellrowborder" valign="top" width="17.71%" headers="mcps1.2.4.1.1 "><p id="p54764719"><a name="p54764719"></a><a name="p54764719"></a>recordsets</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1162515611711"><a name="p1162515611711"></a><a name="p1162515611711"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p45797138"><a name="p45797138"></a><a name="p45797138"></a>recordset列表对象，详细信息请参见<a href="#table18580737">表3</a>。</p>
    </td>
    </tr>
    <tr id="row2133747418458"><td class="cellrowborder" valign="top" width="17.71%" headers="mcps1.2.4.1.1 "><p id="p5781953918458"><a name="p5781953918458"></a><a name="p5781953918458"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5469790918458"><a name="p5469790918458"></a><a name="p5469790918458"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p5673028518536"><a name="p5673028518536"></a><a name="p5673028518536"></a>返回满足过滤条件的资源总数，详细信息请参见<a href="#table9971756154520">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  recordsets字段说明

    <a name="table18580737"></a>
    <table><thead align="left"><tr id="rba3ac5c9022d433a9f831e45adb3139d"><th class="cellrowborder" valign="top" width="18.13%" id="mcps1.2.4.1.1"><p id="af45b6f861fca4148bdabcd3f04b3c585"><a name="af45b6f861fca4148bdabcd3f04b3c585"></a><a name="af45b6f861fca4148bdabcd3f04b3c585"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.67%" id="mcps1.2.4.1.2"><p id="a7dd3d03763104b729e040e9492bc2ff8"><a name="a7dd3d03763104b729e040e9492bc2ff8"></a><a name="a7dd3d03763104b729e040e9492bc2ff8"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.2%" id="mcps1.2.4.1.3"><p id="ab5a394c2e4bf4013b8d26cdf12e57c24"><a name="ab5a394c2e4bf4013b8d26cdf12e57c24"></a><a name="ab5a394c2e4bf4013b8d26cdf12e57c24"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r969f83cacc0d47e19b400db44bcefe5d"><td class="cellrowborder" valign="top" width="18.13%" headers="mcps1.2.4.1.1 "><p id="af7379915cb7e45518ad6389deb156c16"><a name="af7379915cb7e45518ad6389deb156c16"></a><a name="af7379915cb7e45518ad6389deb156c16"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="aed3fb97ef2c44649a4df091614a5fdd3"><a name="aed3fb97ef2c44649a4df091614a5fdd3"></a><a name="aed3fb97ef2c44649a4df091614a5fdd3"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="a7cf188e9e96542f4920ff0531e8a7bf3"><a name="a7cf188e9e96542f4920ff0531e8a7bf3"></a><a name="a7cf188e9e96542f4920ff0531e8a7bf3"></a>Record Set的ID。</p>
    </td>
    </tr>
    <tr id="r3486bde187164f8d8778fd87d3c378f0"><td class="cellrowborder" valign="top" width="18.13%" headers="mcps1.2.4.1.1 "><p id="af845ec9aa4c54290a3c8253710222cbc"><a name="af845ec9aa4c54290a3c8253710222cbc"></a><a name="af845ec9aa4c54290a3c8253710222cbc"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="a184f428a9cd94ffc909dcb75a7f20ffd"><a name="a184f428a9cd94ffc909dcb75a7f20ffd"></a><a name="a184f428a9cd94ffc909dcb75a7f20ffd"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="a107054ce4de94723890caea30f5757d3"><a name="a107054ce4de94723890caea30f5757d3"></a><a name="a107054ce4de94723890caea30f5757d3"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="rddc62f3e40f94c23bde096ec169557a4"><td class="cellrowborder" valign="top" width="18.13%" headers="mcps1.2.4.1.1 "><p id="adf295748fce44c51ab15716d2fca7e7e"><a name="adf295748fce44c51ab15716d2fca7e7e"></a><a name="adf295748fce44c51ab15716d2fca7e7e"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="ac76f924adf39422283aa1be57fe006f0"><a name="ac76f924adf39422283aa1be57fe006f0"></a><a name="ac76f924adf39422283aa1be57fe006f0"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="a5b0ee15a497b4ab7a5dbb737c73626a2"><a name="a5b0ee15a497b4ab7a5dbb737c73626a2"></a><a name="a5b0ee15a497b4ab7a5dbb737c73626a2"></a>Record Set的描述信息。</p>
    </td>
    </tr>
    <tr id="re1cf9f7cd8b143b194cd280e116a4b9c"><td class="cellrowborder" valign="top" width="18.13%" headers="mcps1.2.4.1.1 "><p id="a584f07267f8348e292f92fb24c3f2fee"><a name="a584f07267f8348e292f92fb24c3f2fee"></a><a name="a584f07267f8348e292f92fb24c3f2fee"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="ad1b9905e26094d0d88e276952e41441d"><a name="ad1b9905e26094d0d88e276952e41441d"></a><a name="ad1b9905e26094d0d88e276952e41441d"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="ad42f99ad578645c4b50dbf985a7162ab"><a name="ad42f99ad578645c4b50dbf985a7162ab"></a><a name="ad42f99ad578645c4b50dbf985a7162ab"></a>托管该记录的zone_id。</p>
    </td>
    </tr>
    <tr id="r3a794727d8344df49d5fbb7c99d30130"><td class="cellrowborder" valign="top" width="18.13%" headers="mcps1.2.4.1.1 "><p id="af604e2cdbefc46659353a86fd567eef0"><a name="af604e2cdbefc46659353a86fd567eef0"></a><a name="af604e2cdbefc46659353a86fd567eef0"></a>zone_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="adc9bb6da8c5e47959baf489929313e42"><a name="adc9bb6da8c5e47959baf489929313e42"></a><a name="adc9bb6da8c5e47959baf489929313e42"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="a7356cfcfe3d949c8b76883578a681052"><a name="a7356cfcfe3d949c8b76883578a681052"></a><a name="a7356cfcfe3d949c8b76883578a681052"></a>托管该记录的zone_name。</p>
    </td>
    </tr>
    <tr id="r398a51c6191240b9bdd29358f3410b73"><td class="cellrowborder" valign="top" width="18.13%" headers="mcps1.2.4.1.1 "><p id="a5bffae1635bd486cbf5ef03cdee9c0cd"><a name="a5bffae1635bd486cbf5ef03cdee9c0cd"></a><a name="a5bffae1635bd486cbf5ef03cdee9c0cd"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="a4d34d1f420ec42079710c4d92e0b7616"><a name="a4d34d1f420ec42079710c4d92e0b7616"></a><a name="a4d34d1f420ec42079710c4d92e0b7616"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="ad1150aaf4f1a44e997e3e03abe8c776e"><a name="ad1150aaf4f1a44e997e3e03abe8c776e"></a><a name="ad1150aaf4f1a44e997e3e03abe8c776e"></a>记录类型。</p>
    <p id="p1484155154215"><a name="p1484155154215"></a><a name="p1484155154215"></a>取值范围：A,AAAA,MX,CNAME,TXT, NS（仅限公网Zone）,SRV,PTR（仅限内网Zone）,CAA（仅限公网Zone）。</p>
    <p id="p7402204505815"><a name="p7402204505815"></a><a name="p7402204505815"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a>。</p>
    </td>
    </tr>
    <tr id="r514c4f05b7164f9f9a757f7bd0b7e552"><td class="cellrowborder" valign="top" width="18.13%" headers="mcps1.2.4.1.1 "><p id="acc30ded7ad904dc19929667281bdf470"><a name="acc30ded7ad904dc19929667281bdf470"></a><a name="acc30ded7ad904dc19929667281bdf470"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="adca3e1dc109149ffbd6e40b7eb5ef0c8"><a name="adca3e1dc109149ffbd6e40b7eb5ef0c8"></a><a name="adca3e1dc109149ffbd6e40b7eb5ef0c8"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="p123031523174010"><a name="p123031523174010"></a><a name="p123031523174010"></a>解析记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="p1030317233408"><a name="p1030317233408"></a><a name="p1030317233408"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    </td>
    </tr>
    <tr id="r7c6e7235e2784b7fabcc18251ddafcdc"><td class="cellrowborder" valign="top" width="18.13%" headers="mcps1.2.4.1.1 "><p id="a9f6e2cd5e50e4aa5847081725319268d"><a name="a9f6e2cd5e50e4aa5847081725319268d"></a><a name="a9f6e2cd5e50e4aa5847081725319268d"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="a691054f831a04fc6a8a0b5f8dacf3ab2"><a name="a691054f831a04fc6a8a0b5f8dacf3ab2"></a><a name="a691054f831a04fc6a8a0b5f8dacf3ab2"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="a8ad57aedc72349a29b1ee975b2518257"><a name="a8ad57aedc72349a29b1ee975b2518257"></a><a name="a8ad57aedc72349a29b1ee975b2518257"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="rf1e2aa6701db4f2a9599b86ee5c744e3"><td class="cellrowborder" valign="top" width="18.13%" headers="mcps1.2.4.1.1 "><p id="a18066d6aebd441efad61d00896e13f08"><a name="a18066d6aebd441efad61d00896e13f08"></a><a name="a18066d6aebd441efad61d00896e13f08"></a>create_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="ab7a29ae554744d05875a8e818d1deec0"><a name="ab7a29ae554744d05875a8e818d1deec0"></a><a name="ab7a29ae554744d05875a8e818d1deec0"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="a77d8f72a4bdd45879c196c0160196f50"><a name="a77d8f72a4bdd45879c196c0160196f50"></a><a name="a77d8f72a4bdd45879c196c0160196f50"></a>创建时间。</p>
    <p id="p1731444152613"><a name="p1731444152613"></a><a name="p1731444152613"></a>格式：yyyy-MM-dd'T'HH:mm:ss.SSS</p>
    </td>
    </tr>
    <tr id="r442ce54f5a794788a7ccb195a4b044b1"><td class="cellrowborder" valign="top" width="18.13%" headers="mcps1.2.4.1.1 "><p id="a88e27c6c0c4c42819998a3fdbe2013a6"><a name="a88e27c6c0c4c42819998a3fdbe2013a6"></a><a name="a88e27c6c0c4c42819998a3fdbe2013a6"></a>update_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="p15406328285"><a name="p15406328285"></a><a name="p15406328285"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="aa7cad34bafbc4911a8e4ee943de3d5c1"><a name="aa7cad34bafbc4911a8e4ee943de3d5c1"></a><a name="aa7cad34bafbc4911a8e4ee943de3d5c1"></a>更新时间。</p>
    <p id="p12611114912613"><a name="p12611114912613"></a><a name="p12611114912613"></a>格式：yyyy-MM-dd'T'HH:mm:ss.SSS</p>
    </td>
    </tr>
    <tr id="ra1bb5c494baa45c093a0ed3ea3019fd3"><td class="cellrowborder" valign="top" width="18.13%" headers="mcps1.2.4.1.1 "><p id="aac1eb9d8c2344f97a7a0936bd02ef17b"><a name="aac1eb9d8c2344f97a7a0936bd02ef17b"></a><a name="aac1eb9d8c2344f97a7a0936bd02ef17b"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="a84dffb1a82884ef08a2aadb59bf7b646"><a name="a84dffb1a82884ef08a2aadb59bf7b646"></a><a name="a84dffb1a82884ef08a2aadb59bf7b646"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="a7a8d323b3b5740a88990f8f0a57b2d91"><a name="a7a8d323b3b5740a88990f8f0a57b2d91"></a><a name="a7a8d323b3b5740a88990f8f0a57b2d91"></a>资源状态。</p>
    <p id="p1140919441254"><a name="p1140919441254"></a><a name="p1140919441254"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="r1423508fa22543d8a613944e3903b99f"><td class="cellrowborder" valign="top" width="18.13%" headers="mcps1.2.4.1.1 "><p id="af26a0208c4c64ddd946c9b311972c864"><a name="af26a0208c4c64ddd946c9b311972c864"></a><a name="af26a0208c4c64ddd946c9b311972c864"></a>default</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="a509867184c0e4465ab4619e9170ede0d"><a name="a509867184c0e4465ab4619e9170ede0d"></a><a name="a509867184c0e4465ab4619e9170ede0d"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="ae7a240dfdb36438b988ac09b4f91b32f"><a name="ae7a240dfdb36438b988ac09b4f91b32f"></a><a name="ae7a240dfdb36438b988ac09b4f91b32f"></a>标识是否由系统默认生成，系统默认生成的Record Set不能删除。</p>
    </td>
    </tr>
    <tr id="raf503e75a0204706bd483ee97ddbe730"><td class="cellrowborder" valign="top" width="18.13%" headers="mcps1.2.4.1.1 "><p id="a1c514643bb3f49c888508a07acb384cf"><a name="a1c514643bb3f49c888508a07acb384cf"></a><a name="a1c514643bb3f49c888508a07acb384cf"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="ade8bb3864367491084f4f4fe78e58a33"><a name="ade8bb3864367491084f4f4fe78e58a33"></a><a name="ade8bb3864367491084f4f4fe78e58a33"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="p4619625201026"><a name="p4619625201026"></a><a name="p4619625201026"></a>该Record Set所属的项目ID。</p>
    </td>
    </tr>
    <tr id="rd3a029c667c546e295b038e8f38b71f6"><td class="cellrowborder" valign="top" width="18.13%" headers="mcps1.2.4.1.1 "><p id="a8779f70c5dc4414c8df0c2950001a653"><a name="a8779f70c5dc4414c8df0c2950001a653"></a><a name="a8779f70c5dc4414c8df0c2950001a653"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="a51104ec0822b4bf4bf9018680539141a"><a name="a51104ec0822b4bf4bf9018680539141a"></a><a name="a51104ec0822b4bf4bf9018680539141a"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="aa2a07c69de424ee5bd26b246f46c26c1"><a name="aa2a07c69de424ee5bd26b246f46c26c1"></a><a name="aa2a07c69de424ee5bd26b246f46c26c1"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p1226974804620"><a name="p1226974804620"></a><a name="p1226974804620"></a>详细信息请参见<a href="#table354521744216">表5</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  metadata参数说明

    <a name="table9971756154520"></a>
    <table><thead align="left"><tr id="r1ee98e923a7c4bfcaa89e708d3fca79e"><th class="cellrowborder" valign="top" width="18.23182318231823%" id="mcps1.2.4.1.1"><p id="af493c2fde22f44069c2b5ea0467dfe89"><a name="af493c2fde22f44069c2b5ea0467dfe89"></a><a name="af493c2fde22f44069c2b5ea0467dfe89"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.77197719771977%" id="mcps1.2.4.1.2"><p id="a581940a484df4c8294e51f11391a23c8"><a name="a581940a484df4c8294e51f11391a23c8"></a><a name="a581940a484df4c8294e51f11391a23c8"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="61.996199619962%" id="mcps1.2.4.1.3"><p id="a0301bbf5a1234ea3a88a104e1b4cff92"><a name="a0301bbf5a1234ea3a88a104e1b4cff92"></a><a name="a0301bbf5a1234ea3a88a104e1b4cff92"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r7cc02a0ecbd24482bca90faa98114b18"><td class="cellrowborder" valign="top" width="18.23182318231823%" headers="mcps1.2.4.1.1 "><p id="a9234858cb2f447539b4b85a307884322"><a name="a9234858cb2f447539b4b85a307884322"></a><a name="a9234858cb2f447539b4b85a307884322"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77197719771977%" headers="mcps1.2.4.1.2 "><p id="af14a2a2c8f0345f4811bb21dd2a9b667"><a name="af14a2a2c8f0345f4811bb21dd2a9b667"></a><a name="af14a2a2c8f0345f4811bb21dd2a9b667"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.996199619962%" headers="mcps1.2.4.1.3 "><p id="a39058f9901c84eb9a776ca5cd44ede29"><a name="a39058f9901c84eb9a776ca5cd44ede29"></a><a name="a39058f9901c84eb9a776ca5cd44ede29"></a>满足查询条件的资源总数，不受分页（即limit、offset参数）影响。</p>
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
    <tr id="row37670275497"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
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
            "self": "https://Endpoint/v2/recordsets",
            "next": "https://Endpoint/v2/recordsets?id=&limit=11&marker=2c9eb155587194ec01587224c9f9014a"
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
                "update_at": "2016-11-17T11:56:03.827",
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
                "update_at": "2016-11-17T11:56:03.827",
                "default": true,
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c"
            },
            {
                "id": "2c9eb155587228570158722996ca0002",
                "name": "example.org.",
                "type": "SOA",
                "ttl": 300,
                "records": [
                    "ns1.hotrot.de. xx.example.org. (1 7200 900 1209600 300)"
                ],
                "status": "ACTIVE",
                "links": {
                    "self": "https://Endpoint/v2/zones/2c9eb155587228570158722996c50001/recordsets/2c9eb155587228570158722996ca0002"
                },
                "zone_id": "2c9eb155587228570158722996c50001",
                "zone_name": "example.org.",
                "create_at": "2016-11-17T12:01:17.996",
                "update_at": "2016-11-17T12:56:03.827",
                "default": true,
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c"
            },
            {
                "id": "2c9eb155587228570158722996ca0004",
                "name": "example.org.",
                "type": "NS",
                "ttl": 172800,
                "records": [
                    "ns2.hotrot.de.",
                    "ns1.hotrot.de."
                ],
                "status": "ACTIVE",
                "links": {
                    "self": "https://Endpoint/v2/zones/2c9eb155587228570158722996c50001/recordsets/2c9eb155587228570158722996ca0004"
                },
                "zone_id": "2c9eb155587228570158722996c50001",
                "zone_name": "example.org.",
                "create_at": "2016-11-17T12:01:17.996",
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
                "status": "ACTIVE",
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
            "total_count": 5
        }
    }
    
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

