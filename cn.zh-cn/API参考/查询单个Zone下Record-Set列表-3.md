# 查询单个Zone下Record Set列表<a name="ZH-CN_TOPIC_0082840630"></a>

## 功能介绍<a name="section8391370"></a>

查询单个Zone下Record Set列表。

## URI<a name="section8413469"></a>

GET /v2.1/zones/\{zone\_id\}/recordsets?limit=\{limit\}&marker=\{marker\}&line=\{line\_name\}&sort\_key=\{sort\_key\}&sort\_dir=\{sort\_dir\}

参数说明请参见[表1](#table48883615)。

**表 1**  URI格式的参数说明

<a name="table48883615"></a>
<table><thead align="left"><tr id="row57562809"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.5.1.1"><p id="p32075938"><a name="p32075938"></a><a name="p32075938"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.5.1.2"><p id="p48014184"><a name="p48014184"></a><a name="p48014184"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14141414141414%" id="mcps1.2.5.1.3"><p id="p63943666"><a name="p63943666"></a><a name="p63943666"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.2.5.1.4"><p id="p12054440"><a name="p12054440"></a><a name="p12054440"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row36885620"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p34945211"><a name="p34945211"></a><a name="p34945211"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p11989863"><a name="p11989863"></a><a name="p11989863"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p31654880"><a name="p31654880"></a><a name="p31654880"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p13908493"><a name="p13908493"></a><a name="p13908493"></a>所属zone id。仅支持公网zone。</p>
</td>
</tr>
<tr id="row58067579"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p5853458"><a name="p5853458"></a><a name="p5853458"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p4368081"><a name="p4368081"></a><a name="p4368081"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p18270305"><a name="p18270305"></a><a name="p18270305"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p3499754"><a name="p3499754"></a><a name="p3499754"></a>分页查询起始的资源ID，为空时为查询第一页。</p>
</td>
</tr>
<tr id="row31497787"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p1183915"><a name="p1183915"></a><a name="p1183915"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p28788263"><a name="p28788263"></a><a name="p28788263"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p50147992"><a name="p50147992"></a><a name="p50147992"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="ul2143191219534"></a><a name="ul2143191219534"></a><ul id="ul2143191219534"><li>取值范围：0～500<p id="p13936864195316"><a name="p13936864195316"></a><a name="p13936864195316"></a>取值一般为10，20，50</p>
</li><li>功能说明：每页返回的个数。</li></ul>
</td>
</tr>
<tr id="row15709056145520"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p55549708145520"><a name="p55549708145520"></a><a name="p55549708145520"></a>line</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p3232537145520"><a name="p3232537145520"></a><a name="p3232537145520"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p60508934145520"><a name="p60508934145520"></a><a name="p60508934145520"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p2276603145520"><a name="p2276603145520"></a><a name="p2276603145520"></a>解析线路。请参见<a href="解析线路类型.md">解析线路类型</a>。</p>
</td>
</tr>
<tr id="row9685158173314"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p15674182317363"><a name="p15674182317363"></a><a name="p15674182317363"></a>sort_key</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p206741223103614"><a name="p206741223103614"></a><a name="p206741223103614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p7674132316360"><a name="p7674132316360"></a><a name="p7674132316360"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p4674182316366"><a name="p4674182316366"></a><a name="p4674182316366"></a>查询结果中Record Set列表的排序字段。</p>
<p id="p161032135113"><a name="p161032135113"></a><a name="p161032135113"></a>取值范围：</p>
<a name="ul0957431182915"></a><a name="ul0957431182915"></a><ul id="ul0957431182915"><li>name：域名</li><li>type：记录集类型</li></ul>
</td>
</tr>
<tr id="row5685558123311"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p208891026103817"><a name="p208891026103817"></a><a name="p208891026103817"></a>sort_dir</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p4889162653813"><a name="p4889162653813"></a><a name="p4889162653813"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p128891626133813"><a name="p128891626133813"></a><a name="p128891626133813"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p116071347131216"><a name="p116071347131216"></a><a name="p116071347131216"></a>查询结果中Record Set列表的排序方式。</p>
<p id="p1791903818290"><a name="p1791903818290"></a><a name="p1791903818290"></a>取值范围：</p>
<a name="ul4952114912919"></a><a name="ul4952114912919"></a><ul id="ul4952114912919"><li>desc：降序排序</li><li>asc：升序排序</li></ul>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section8612359"></a>

无

## 响应<a name="section10402369"></a>

-   要素说明

    **表 2**  响应样例的要素说明

    <a name="table53402119"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0037129969_row41580444"><th class="cellrowborder" valign="top" width="20.41%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0037129969_p12572829"><a name="zh-cn_topic_0037129969_p12572829"></a><a name="zh-cn_topic_0037129969_p12572829"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.47%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0037129969_p13543581"><a name="zh-cn_topic_0037129969_p13543581"></a><a name="zh-cn_topic_0037129969_p13543581"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.120000000000005%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0037129969_p23288300"><a name="zh-cn_topic_0037129969_p23288300"></a><a name="zh-cn_topic_0037129969_p23288300"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0037129969_row7304143"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129969_p54764719"><a name="zh-cn_topic_0037129969_p54764719"></a><a name="zh-cn_topic_0037129969_p54764719"></a>recordsets</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129969_p10465156"><a name="zh-cn_topic_0037129969_p10465156"></a><a name="zh-cn_topic_0037129969_p10465156"></a><em id="zh-cn_topic_0037129969_i44918310194055"><a name="zh-cn_topic_0037129969_i44918310194055"></a><a name="zh-cn_topic_0037129969_i44918310194055"></a>列表数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129969_p45797138"><a name="zh-cn_topic_0037129969_p45797138"></a><a name="zh-cn_topic_0037129969_p45797138"></a>recordset列表对象</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129969_row2133747418458"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129969_p5781953918458"><a name="zh-cn_topic_0037129969_p5781953918458"></a><a name="zh-cn_topic_0037129969_p5781953918458"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129969_p5469790918458"><a name="zh-cn_topic_0037129969_p5469790918458"></a><a name="zh-cn_topic_0037129969_p5469790918458"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129969_p5673028518536"><a name="zh-cn_topic_0037129969_p5673028518536"></a><a name="zh-cn_topic_0037129969_p5673028518536"></a>返回满足过滤条件的资源总数</p>
    </td>
    </tr>
    </tbody>
    </table>

    其中，[表2](#table53402119)中的recordsets字段说明，请参见[表3](#table7192645154740)；metadata字段说明请参见[表4](#table2908319718932)。

    **表 3**  recordsets字段说明

    <a name="table7192645154740"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row52466955175323"><th class="cellrowborder" valign="top" width="27.889999999999997%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2769858175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2769858175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2769858175323"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p46296309175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p46296309175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p46296309175323"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.3%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p62697904175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p62697904175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p62697904175323"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row47909891175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64112397175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64112397175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64112397175323"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1660870175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1660870175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1660870175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1249204175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1249204175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1249204175323"></a>Record Set的ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row6942422175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64097412175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64097412175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64097412175323"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p44990515175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p44990515175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p44990515175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p32019574175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p32019574175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p32019574175323"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row61442071175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51194416175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51194416175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51194416175323"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63301991175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63301991175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63301991175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43966660175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43966660175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43966660175323"></a>Record Set的描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row2176746175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p11805366175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p11805366175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p11805366175323"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1051908175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1051908175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1051908175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p10043845175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p10043845175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p10043845175323"></a>托管该记录的zone_id。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row61212722175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p8318586175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p8318586175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p8318586175323"></a>zone_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p31287919175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p31287919175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p31287919175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p16372315175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p16372315175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p16372315175323"></a>托管该记录的zone_name。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row38132372175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37461920175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37461920175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37461920175323"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27536075175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27536075175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27536075175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p24813356175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p24813356175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p24813356175323"></a>记录类型。</p>
    <p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p52445812175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p52445812175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p52445812175323"></a>取值范围：A，AAAA，MX，CNAME，TXT，NS（仅限公网Zone），SRV，CAA（仅限公网Zone）。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row20796819175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4811553175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4811553175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4811553175323"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47559731175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47559731175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47559731175323"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p22097398175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p22097398175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p22097398175323"></a>域名的缓存时间，单位为秒，缓存时间越长更新生效越慢。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row13978060175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43388342175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43388342175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43388342175323"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p29596719175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p29596719175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p29596719175323"></a>List&lt;string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p30492925175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p30492925175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p30492925175323"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row23148559175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36524189175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36524189175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36524189175323"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47080972175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47080972175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47080972175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p15737135175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p15737135175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p15737135175323"></a>创建时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row33465792175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p42570937175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p42570937175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p42570937175323"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27449776175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27449776175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27449776175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63703533175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63703533175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63703533175323"></a>更新时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row17850883175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36228271175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36228271175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36228271175323"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p6480061175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p6480061175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p6480061175323"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p65781854175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p65781854175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p65781854175323"></a>资源状态。</p>
    <p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51374523175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51374523175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51374523175323"></a>取值范围：PENDING_CREATE，ACTIVE，PENDING_UPDATE，PENDING_DELETE，ERROR，FREEZE，DISABLE。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row61184424175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p49633411175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p49633411175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p49633411175323"></a>default</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p56048766175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p56048766175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p56048766175323"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37768157175323"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37768157175323"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37768157175323"></a>标识是否由系统默认生成，系统默认生成的Record Set不能删除。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row15199048201026"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p23163408201026"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p23163408201026"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p23163408201026"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p40653752201026"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p40653752201026"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p40653752201026"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4619625201026"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4619625201026"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4619625201026"></a>该Record Set所属的租户ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_row3965248419366"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2132803819366"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2132803819366"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2132803819366"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1127763319366"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1127763319366"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1127763319366"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4107308719366"><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4107308719366"></a><a name="zh-cn_topic_0082840629_zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4107308719366"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_row9356682144842"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_p22615737144842"><a name="zh-cn_topic_0082840629_p22615737144842"></a><a name="zh-cn_topic_0082840629_p22615737144842"></a>line</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_p19935422144842"><a name="zh-cn_topic_0082840629_p19935422144842"></a><a name="zh-cn_topic_0082840629_p19935422144842"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_p4156471144842"><a name="zh-cn_topic_0082840629_p4156471144842"></a><a name="zh-cn_topic_0082840629_p4156471144842"></a>解析线路。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_row53235414144842"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_p45908350113426"><a name="zh-cn_topic_0082840629_p45908350113426"></a><a name="zh-cn_topic_0082840629_p45908350113426"></a>weight</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_p27588875113426"><a name="zh-cn_topic_0082840629_p27588875113426"></a><a name="zh-cn_topic_0082840629_p27588875113426"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_p20106421113426"><a name="zh-cn_topic_0082840629_p20106421113426"></a><a name="zh-cn_topic_0082840629_p20106421113426"></a>解析记录的权重。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840629_row65752664152411"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840629_p24365529152411"><a name="zh-cn_topic_0082840629_p24365529152411"></a><a name="zh-cn_topic_0082840629_p24365529152411"></a>health_check_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840629_p27450827152411"><a name="zh-cn_topic_0082840629_p27450827152411"></a><a name="zh-cn_topic_0082840629_p27450827152411"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840629_p67036304152425"><a name="zh-cn_topic_0082840629_p67036304152425"></a><a name="zh-cn_topic_0082840629_p67036304152425"></a>健康检查ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  metadata参数说明

    <a name="table2908319718932"></a>
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
            "self": "https://Endpoint/v2.1/recordsets?limit=11&marker=&name=&status=&zone_id=2c9eb155587194ec01587224c9f90149"
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
                "zone_id": "2c9eb155587194ec01587224c9f90149",
                "zone_name": "example.com.",
                "created_at": "2016-11-17T11:56:03.439",
                "updated_at": "2016-11-17T11:56:06.439",
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
                "zone_id": "2c9eb155587194ec01587224c9f90149",
                "zone_name": "example.com.",
                "created_at": "2016-11-17T11:56:03.439",
                "updated_at": "2016-11-17T11:56:06.439",
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
                "zone_id": "2c9eb155587194ec01587224c9f90149",
                "zone_name": "example.com.",
                "created_at": "2016-11-17T12:03:17.827",
                "updated_at": "2016-11-17T12:56:06.439",
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


## 返回值<a name="section26512460"></a>

请参考[通用请求返回值](通用请求返回值.md)。

