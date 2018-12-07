# 查询Record Set列表<a name="ZH-CN_TOPIC_0037129969"></a>

## 功能介绍<a name="section29105235"></a>

查询租户Record Set资源列表。

## URI<a name="section60620523"></a>

GET /v2/recordsets?zone\_type=\{zone\_type\}&limit=\{limit\}&marker=\{marker\}&offset=\{offset\}&tags=\{tags\}&status=\{status\}&type=\{type\}&name=\{name\}&id=\{id\}&records=\{records\}&sort\_key=\{sort\_key\}&sort\_dir=\{sort\_dir\}

参数说明请参见[表1](#table40248354)。

**表 1**  URI格式的参数说明

<a name="table40248354"></a>
<table><thead align="left"><tr id="row24110047"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.5.1.1"><p id="p6756797"><a name="p6756797"></a><a name="p6756797"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.5.1.2"><p id="p10429724"><a name="p10429724"></a><a name="p10429724"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14141414141414%" id="mcps1.2.5.1.3"><p id="p39501348"><a name="p39501348"></a><a name="p39501348"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.2.5.1.4"><p id="p45492604"><a name="p45492604"></a><a name="p45492604"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row67046586114158"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p10129219114159"><a name="p10129219114159"></a><a name="p10129219114159"></a>zone_type</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p15160399114159"><a name="p15160399114159"></a><a name="p15160399114159"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p20032767114159"><a name="p20032767114159"></a><a name="p20032767114159"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p12041403114159"><a name="p12041403114159"></a><a name="p12041403114159"></a>待查询的Record Set的域名类型。</p>
<p id="p41263770114159"><a name="p41263770114159"></a><a name="p41263770114159"></a>取值范围：public、private</p>
<a name="ul35829612114159"></a><a name="ul35829612114159"></a><ul id="ul35829612114159"><li>如果为空，表示查询公网类型的Record Set。</li><li>如果为public，表示查询公网类型的Record Set。</li><li>如果为private，表示查询内网类型的Record Set。</li></ul>
</td>
</tr>
<tr id="row61022284"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p43857981"><a name="p43857981"></a><a name="p43857981"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p62835574"><a name="p62835574"></a><a name="p62835574"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p56516768"><a name="p56516768"></a><a name="p56516768"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p14455523"><a name="p14455523"></a><a name="p14455523"></a>分页查询起始的资源ID，为空时为查询第一页。</p>
</td>
</tr>
<tr id="row62990845"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p1984791"><a name="p1984791"></a><a name="p1984791"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p26550365"><a name="p26550365"></a><a name="p26550365"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p3095993"><a name="p3095993"></a><a name="p3095993"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="ul18169499193915"></a><a name="ul18169499193915"></a><ul id="ul18169499193915"><li>取值范围：0~500<p id="p61821521193933"><a name="p61821521193933"></a><a name="p61821521193933"></a>取值一般为10，20，50</p>
</li><li>功能说明：每页返回的资源个数。</li></ul>
</td>
</tr>
<tr id="row78856519552"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p5702070419554"><a name="p5702070419554"></a><a name="p5702070419554"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p5527430219554"><a name="p5527430219554"></a><a name="p5527430219554"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p4803348119554"><a name="p4803348119554"></a><a name="p4803348119554"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="ul6550672819554"></a><a name="ul6550672819554"></a><ul id="ul6550672819554"><li>取值范围：0~2147483647</li><li>分页查询起始页码，起始值为0。当前设置marker不为空时，以marker为分页起始标识。</li></ul>
</td>
</tr>
<tr id="row55044453115726"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p216770371221"><a name="p216770371221"></a><a name="p216770371221"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p110096061221"><a name="p110096061221"></a><a name="p110096061221"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p193628991221"><a name="p193628991221"></a><a name="p193628991221"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p248910051221"><a name="p248910051221"></a><a name="p248910051221"></a>资源标签。</p>
<p id="p226924561221"><a name="p226924561221"></a><a name="p226924561221"></a>取值格式：key1,value1|key2,value2</p>
<p id="p40552875114139"><a name="p40552875114139"></a><a name="p40552875114139"></a>多个标签之间用"|"分开，每个标签的键值用英文逗号","相隔。</p>
<p id="p29055151221"><a name="p29055151221"></a><a name="p29055151221"></a>多个标签之间为“与”的关系。</p>
<p id="p59717447115129"><a name="p59717447115129"></a><a name="p59717447115129"></a>关于资源标签，请参见<a href="添加资源标签.md">添加资源标签</a>。</p>
</td>
</tr>
<tr id="row91871931125514"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p15187431105515"><a name="p15187431105515"></a><a name="p15187431105515"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p21877311559"><a name="p21877311559"></a><a name="p21877311559"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p18187143110551"><a name="p18187143110551"></a><a name="p18187143110551"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p181873314559"><a name="p181873314559"></a><a name="p181873314559"></a>待查询的Record Set的状态。</p>
<p id="p447517111159"><a name="p447517111159"></a><a name="p447517111159"></a>取值范围：ACTIVE、ERROR、DISABLE、FREEZE、PENDING_CREATE、PENDING_UPDATE、PENDING_DELETE</p>
<a name="ul2690931193818"></a><a name="ul2690931193818"></a><ul id="ul2690931193818"><li>如果为空，表示查询所有状态的Record Set</li><li>如果为ACTIVE，表示查询正常状态的Record Set</li><li>如果为ERROR，表示查询失败状态的Record Set</li><li>如果为DISABLE，表示查询已暂停状态的Record Set</li><li>如果为FREEZE，表示查询已冻结状态的Record Set</li><li>如果为PENDING_CREATE，表示查询创建中状态的Record Set</li><li>如果为PENDING_UPDATE，表示查询更新中状态的Record Set</li><li>如果为PENDING_DELETE，表示查询删除中状态的Record Set</li></ul>
</td>
</tr>
<tr id="row1799821219113"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p4998111210116"><a name="p4998111210116"></a><a name="p4998111210116"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p89981512101120"><a name="p89981512101120"></a><a name="p89981512101120"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p399821215119"><a name="p399821215119"></a><a name="p399821215119"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p109982012141111"><a name="p109982012141111"></a><a name="p109982012141111"></a>待查询的Record Set的记录集类型。</p>
<p id="p20817123416132"><a name="p20817123416132"></a><a name="p20817123416132"></a>取值范围：A、CNAME、MX、AAAA、TXT、SRV、NS、CAA</p>
<a name="ul439464583815"></a><a name="ul439464583815"></a><ul id="ul439464583815"><li>如果为空，表示查询所有类型的Record Set</li><li>如果为A，表示查询A类型的Record Set</li><li>如果为CNAME，表示查询CNAME类型的Record Set</li><li>如果为MX，表示查询MX类型的Record Set</li><li>如果为AAAA，表示查询AAAA类型的Record Set</li><li>如果为TXT，表示查询TXT类型的Record Set</li><li>如果为SRV，表示查询SRV类型的Record Set</li><li>如果为NS，表示查询NS类型的Record Set</li><li>如果为CAA，表示查询CAA类型的Record Set</li></ul>
</td>
</tr>
<tr id="row11927135213161"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p189276527168"><a name="p189276527168"></a><a name="p189276527168"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p19927752151617"><a name="p19927752151617"></a><a name="p19927752151617"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p1492719522167"><a name="p1492719522167"></a><a name="p1492719522167"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p11927252121613"><a name="p11927252121613"></a><a name="p11927252121613"></a>待查询的Record Set的域名中包含此name。</p>
</td>
</tr>
<tr id="row33603617197"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p13604691913"><a name="p13604691913"></a><a name="p13604691913"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p15360960192"><a name="p15360960192"></a><a name="p15360960192"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p4360869195"><a name="p4360869195"></a><a name="p4360869195"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p173609610193"><a name="p173609610193"></a><a name="p173609610193"></a>待查询的Record Set的id包含此id。</p>
</td>
</tr>
<tr id="row191263112211"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p112614115211"><a name="p112614115211"></a><a name="p112614115211"></a>records</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p81261211182110"><a name="p81261211182110"></a><a name="p81261211182110"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p131261311192119"><a name="p131261311192119"></a><a name="p131261311192119"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p260972615213"><a name="p260972615213"></a><a name="p260972615213"></a>待查询的Record Set的值中包含此records。</p>
</td>
</tr>
<tr id="row6672923143613"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p15674182317363"><a name="p15674182317363"></a><a name="p15674182317363"></a>sort_key</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p206741223103614"><a name="p206741223103614"></a><a name="p206741223103614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p7674132316360"><a name="p7674132316360"></a><a name="p7674132316360"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p4674182316366"><a name="p4674182316366"></a><a name="p4674182316366"></a>查询结果中Record Set列表的排序字段。</p>
<p id="p161032135113"><a name="p161032135113"></a><a name="p161032135113"></a>取值范围：</p>
<a name="ul1181955993116"></a><a name="ul1181955993116"></a><ul id="ul1181955993116"><li>name：域名</li><li>type：记录集类型</li></ul>
</td>
</tr>
<tr id="row11889126183816"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p208891026103817"><a name="p208891026103817"></a><a name="p208891026103817"></a>sort_dir</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p4889162653813"><a name="p4889162653813"></a><a name="p4889162653813"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p128891626133813"><a name="p128891626133813"></a><a name="p128891626133813"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p116071347131216"><a name="p116071347131216"></a><a name="p116071347131216"></a>查询结果中Record Set列表的排序方式。</p>
<p id="p749316343213"><a name="p749316343213"></a><a name="p749316343213"></a>取值范围：</p>
<a name="ul18204217325"></a><a name="ul18204217325"></a><ul id="ul18204217325"><li>desc：降序排序</li><li>asc：升序排序</li></ul>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section8713795"></a>

无

## 响应<a name="section11315292"></a>

-   要素说明

    **表 2**  响应样例的要素说明

    <a name="table21574462"></a>
    <table><thead align="left"><tr id="row41580444"><th class="cellrowborder" valign="top" width="20.41%" id="mcps1.2.4.1.1"><p id="p12572829"><a name="p12572829"></a><a name="p12572829"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.47%" id="mcps1.2.4.1.2"><p id="p13543581"><a name="p13543581"></a><a name="p13543581"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.120000000000005%" id="mcps1.2.4.1.3"><p id="p23288300"><a name="p23288300"></a><a name="p23288300"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row7304143"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.1 "><p id="p54764719"><a name="p54764719"></a><a name="p54764719"></a>recordsets</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.2.4.1.2 "><p id="p10465156"><a name="p10465156"></a><a name="p10465156"></a><em id="i44918310194055"><a name="i44918310194055"></a><a name="i44918310194055"></a>列表数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.2.4.1.3 "><p id="p45797138"><a name="p45797138"></a><a name="p45797138"></a>recordset列表对象</p>
    </td>
    </tr>
    <tr id="row2133747418458"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.1 "><p id="p5781953918458"><a name="p5781953918458"></a><a name="p5781953918458"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.2.4.1.2 "><p id="p5469790918458"><a name="p5469790918458"></a><a name="p5469790918458"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.2.4.1.3 "><p id="p5673028518536"><a name="p5673028518536"></a><a name="p5673028518536"></a>返回满足过滤条件的资源总数</p>
    </td>
    </tr>
    </tbody>
    </table>

    其中，[表2](#table21574462)中的recordsets字段说明，请参见[表3](#table18580737)；metadata字段说明请参见[表4](#table9971756154520)。 

    **表 3**  recordsets字段说明

    <a name="table18580737"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row52466955175323"><th class="cellrowborder" valign="top" width="27.889999999999997%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2769858175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2769858175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2769858175323"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p46296309175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p46296309175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p46296309175323"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.3%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p62697904175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p62697904175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p62697904175323"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row47909891175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64112397175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64112397175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64112397175323"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1660870175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1660870175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1660870175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1249204175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1249204175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1249204175323"></a>Record Set的ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row6942422175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64097412175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64097412175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64097412175323"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p44990515175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p44990515175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p44990515175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p32019574175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p32019574175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p32019574175323"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row61442071175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51194416175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51194416175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51194416175323"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63301991175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63301991175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63301991175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43966660175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43966660175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43966660175323"></a>Record Set的描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row2176746175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p11805366175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p11805366175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p11805366175323"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1051908175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1051908175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1051908175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p10043845175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p10043845175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p10043845175323"></a>托管该记录的zone_id。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row61212722175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p8318586175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p8318586175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p8318586175323"></a>zone_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p31287919175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p31287919175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p31287919175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p16372315175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p16372315175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p16372315175323"></a>托管该记录的zone_name。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row38132372175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37461920175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37461920175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37461920175323"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27536075175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27536075175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27536075175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p24813356175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p24813356175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p24813356175323"></a>记录类型。</p>
    <p id="p1484155154215"><a name="p1484155154215"></a><a name="p1484155154215"></a>取值范围：A,AAAA,MX,CNAME,TXT, NS（仅限公网Zone）,SRV,PTR（仅限内网Zone）,CAA（仅限公网Zone）。</p>
    <p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p52445812175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p52445812175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p52445812175323"></a></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row20796819175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4811553175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4811553175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4811553175323"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47559731175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47559731175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47559731175323"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p22097398175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p22097398175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p22097398175323"></a>域名的缓存时间，单位为秒，缓存时间越长更新生效越慢。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row13978060175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43388342175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43388342175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43388342175323"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p29596719175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p29596719175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p29596719175323"></a>List&lt;string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p30492925175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p30492925175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p30492925175323"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row23148559175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36524189175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36524189175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36524189175323"></a>create_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47080972175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47080972175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47080972175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p15737135175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p15737135175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p15737135175323"></a>创建时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row33465792175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p42570937175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p42570937175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p42570937175323"></a>update_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27449776175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27449776175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27449776175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63703533175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63703533175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63703533175323"></a>更新时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row17850883175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36228271175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36228271175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36228271175323"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p6480061175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p6480061175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p6480061175323"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p65781854175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p65781854175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p65781854175323"></a>资源状态。</p>
    <p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51374523175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51374523175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51374523175323"></a>取值范围：PENDING_CREATE，ACTIVE，PENDING_UPDATE，PENDING_DELETE，ERROR。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row61184424175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p49633411175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p49633411175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p49633411175323"></a>default</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p56048766175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p56048766175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p56048766175323"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37768157175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37768157175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37768157175323"></a>标识是否由系统默认生成，系统默认生成的Record Set不能删除。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row15199048201026"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p23163408201026"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p23163408201026"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p23163408201026"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p40653752201026"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p40653752201026"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p40653752201026"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4619625201026"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4619625201026"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4619625201026"></a>该Record Set所属的租户ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row3965248419366"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2132803819366"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2132803819366"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2132803819366"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1127763319366"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1127763319366"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1127763319366"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4107308719366"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4107308719366"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4107308719366"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  metadata参数说明

    <a name="table9971756154520"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0037134402_row58979189175457"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0037134402_p46156243175457"><a name="zh-cn_topic_0037134402_p46156243175457"></a><a name="zh-cn_topic_0037134402_p46156243175457"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0037134402_p47668234175457"><a name="zh-cn_topic_0037134402_p47668234175457"></a><a name="zh-cn_topic_0037134402_p47668234175457"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0037134402_p35921708175457"><a name="zh-cn_topic_0037134402_p35921708175457"></a><a name="zh-cn_topic_0037134402_p35921708175457"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0037134402_row54859922175457"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134402_p14468674175457"><a name="zh-cn_topic_0037134402_p14468674175457"></a><a name="zh-cn_topic_0037134402_p14468674175457"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134402_p31111955175457"><a name="zh-cn_topic_0037134402_p31111955175457"></a><a name="zh-cn_topic_0037134402_p31111955175457"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134402_p37040428175457"><a name="zh-cn_topic_0037134402_p37040428175457"></a><a name="zh-cn_topic_0037134402_p37040428175457"></a>资源总数</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "links": {
            "self": "https://Endpoint/v2/recordsets"
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


## 返回值<a name="section34728767"></a>

请参考[通用请求返回值](通用请求返回值.md)。

