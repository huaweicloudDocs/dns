# 查询批量导入Record Set任务<a name="ZH-CN_TOPIC_0130149200"></a>

## 功能介绍<a name="section29105235"></a>

查询批量导入Record Set的任务信息。

## URI<a name="section60620523"></a>

GET /v2/zones/\{zone\_id\}/import/recordsets

参数说明请参见[表1](#table40248354)。

**表 1**  URI格式的参数说明

<a name="table40248354"></a>
<table><thead align="left"><tr id="row24110047"><th class="cellrowborder" valign="top" width="24.92%" id="mcps1.2.4.1.1"><p id="p6756797"><a name="p6756797"></a><a name="p6756797"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="21.89%" id="mcps1.2.4.1.2"><p id="p10429724"><a name="p10429724"></a><a name="p10429724"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="53.190000000000005%" id="mcps1.2.4.1.3"><p id="p45492604"><a name="p45492604"></a><a name="p45492604"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row67046586114158"><td class="cellrowborder" valign="top" width="24.92%" headers="mcps1.2.4.1.1 "><p id="p4583482295510"><a name="p4583482295510"></a><a name="p4583482295510"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.2.4.1.2 "><p id="p2163312295510"><a name="p2163312295510"></a><a name="p2163312295510"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="53.190000000000005%" headers="mcps1.2.4.1.3 "><p id="p6128908295528"><a name="p6128908295528"></a><a name="p6128908295528"></a>所属zone的ID。</p>
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
    <tbody><tr id="row7304143"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.1 "><p id="p54764719"><a name="p54764719"></a><a name="p54764719"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.2.4.1.2 "><p id="p5168558495612"><a name="p5168558495612"></a><a name="p5168558495612"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.2.4.1.3 "><p id="p6626197095624"><a name="p6626197095624"></a><a name="p6626197095624"></a>状态码</p>
    </td>
    </tr>
    <tr id="row2133747418458"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.1 "><p id="p5781953918458"><a name="p5781953918458"></a><a name="p5781953918458"></a>data</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.2.4.1.2 "><p id="p5469790918458"><a name="p5469790918458"></a><a name="p5469790918458"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.2.4.1.3 "><p id="p5673028518536"><a name="p5673028518536"></a><a name="p5673028518536"></a>批量导入结果</p>
    </td>
    </tr>
    </tbody>
    </table>

    其中，[表2](#table21574462)的data字段说明，请参见[表3](#table18580737)。

    **表 3**  data字段说明

    <a name="table18580737"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row52466955175323"><th class="cellrowborder" valign="top" width="27.889999999999997%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2769858175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2769858175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p2769858175323"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p46296309175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p46296309175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p46296309175323"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.3%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p62697904175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p62697904175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p62697904175323"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row47909891175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64112397175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64112397175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64112397175323"></a>task_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1660870175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1660870175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1660870175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1249204175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1249204175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1249204175323"></a>任务ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row6942422175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64097412175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64097412175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p64097412175323"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p44990515175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p44990515175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p44990515175323"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p3915545095742"><a name="p3915545095742"></a><a name="p3915545095742"></a>任务状态。</p>
    <p id="p5117746995747"><a name="p5117746995747"></a><a name="p5117746995747"></a>取值范围：PENDING, DONE</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row61442071175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51194416175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51194416175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p51194416175323"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63301991175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63301991175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p63301991175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43966660175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43966660175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43966660175323"></a>所属zone的ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row2176746175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p11805366175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p11805366175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p11805366175323"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1051908175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1051908175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p1051908175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p10043845175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p10043845175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p10043845175323"></a>所属zone的类型。</p>
    </td>
    </tr>
    <tr id="row85240571019"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p193600321019"><a name="p193600321019"></a><a name="p193600321019"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p246587881019"><a name="p246587881019"></a><a name="p246587881019"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p512048121019"><a name="p512048121019"></a><a name="p512048121019"></a>创建时间。</p>
    </td>
    </tr>
    <tr id="row5744492010112"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p2252695810112"><a name="p2252695810112"></a><a name="p2252695810112"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p1274431610112"><a name="p1274431610112"></a><a name="p1274431610112"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p2565671510112"><a name="p2565671510112"></a><a name="p2565671510112"></a>更新时间。</p>
    </td>
    </tr>
    <tr id="row653970501024"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p626696941024"><a name="p626696941024"></a><a name="p626696941024"></a>language</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p430804831024"><a name="p430804831024"></a><a name="p430804831024"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p669671211024"><a name="p669671211024"></a><a name="p669671211024"></a>导入时所使用的模板语言。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row38132372175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37461920175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37461920175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p37461920175323"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27536075175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27536075175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p27536075175323"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p5720905195922"><a name="p5720905195922"></a><a name="p5720905195922"></a>导入的总记录数。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row20796819175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4811553175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4811553175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p4811553175323"></a>success_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47559731175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47559731175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47559731175323"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p569929461007"><a name="p569929461007"></a><a name="p569929461007"></a>导入成功的记录数。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row13978060175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43388342175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43388342175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p43388342175323"></a>error_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p29596719175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p29596719175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p29596719175323"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p30492925175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p30492925175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p30492925175323"></a>导入失败的记录数。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_row23148559175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36524189175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36524189175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p36524189175323"></a>error_items</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47080972175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47080972175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p47080972175323"></a><em id="i1309797110321"><a name="i1309797110321"></a><a name="i1309797110321"></a>列表数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p15737135175323"><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p15737135175323"></a><a name="zh-cn_topic_0037129968_zh-cn_topic_0037134404_p15737135175323"></a>导入失败的记录明细。</p>
    </td>
    </tr>
    </tbody>
    </table>

    其中，[表3](#table18580737)的error\_items字段说明，请参见[表4](#table9971756154520)。

    **表 4**  error\_items参数说明

    <a name="table9971756154520"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0037134402_row58979189175457"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0037134402_p46156243175457"><a name="zh-cn_topic_0037134402_p46156243175457"></a><a name="zh-cn_topic_0037134402_p46156243175457"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0037134402_p47668234175457"><a name="zh-cn_topic_0037134402_p47668234175457"></a><a name="zh-cn_topic_0037134402_p47668234175457"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0037134402_p35921708175457"><a name="zh-cn_topic_0037134402_p35921708175457"></a><a name="zh-cn_topic_0037134402_p35921708175457"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0037134402_row54859922175457"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134402_p14468674175457"><a name="zh-cn_topic_0037134402_p14468674175457"></a><a name="zh-cn_topic_0037134402_p14468674175457"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134402_p31111955175457"><a name="zh-cn_topic_0037134402_p31111955175457"></a><a name="zh-cn_topic_0037134402_p31111955175457"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p6308186310615"><a name="p6308186310615"></a><a name="p6308186310615"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="row264107011054"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p482421911054"><a name="p482421911054"></a><a name="p482421911054"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p153034241054"><a name="p153034241054"></a><a name="p153034241054"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p316178701054"><a name="p316178701054"></a><a name="p316178701054"></a>Record Set的类型。</p>
    </td>
    </tr>
    <tr id="row351137031056"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p482014261056"><a name="p482014261056"></a><a name="p482014261056"></a>line</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p120013951056"><a name="p120013951056"></a><a name="p120013951056"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p325889331056"><a name="p325889331056"></a><a name="p325889331056"></a>Record Set所属线路。</p>
    </td>
    </tr>
    <tr id="row578224491058"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p121123811058"><a name="p121123811058"></a><a name="p121123811058"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p415788181058"><a name="p415788181058"></a><a name="p415788181058"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p124410831058"><a name="p124410831058"></a><a name="p124410831058"></a>Record Set的TTL。</p>
    </td>
    </tr>
    <tr id="row1335802210510"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p528222610510"><a name="p528222610510"></a><a name="p528222610510"></a>weight</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p2520717510510"><a name="p2520717510510"></a><a name="p2520717510510"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p2851528010510"><a name="p2851528010510"></a><a name="p2851528010510"></a>Record Set的权重。</p>
    <p id="p3854865710138"><a name="p3854865710138"></a><a name="p3854865710138"></a>系统预留字段。当支持权重时，该字段正常显示，否则不显示。</p>
    </td>
    </tr>
    <tr id="row11785410512"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p5978200910512"><a name="p5978200910512"></a><a name="p5978200910512"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p1050457010512"><a name="p1050457010512"></a><a name="p1050457010512"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p4556384310512"><a name="p4556384310512"></a><a name="p4556384310512"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="row3977948110513"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p6442468810513"><a name="p6442468810513"></a><a name="p6442468810513"></a>error_code</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p5101721110513"><a name="p5101721110513"></a><a name="p5101721110513"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p3875343110513"><a name="p3875343110513"></a><a name="p3875343110513"></a>错误码。</p>
    </td>
    </tr>
    <tr id="row4928252010515"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p3404070410515"><a name="p3404070410515"></a><a name="p3404070410515"></a>error_message</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p583362210515"><a name="p583362210515"></a><a name="p583362210515"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p276141010515"><a name="p276141010515"></a><a name="p276141010515"></a>错误信息。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
      "code": 200,
      "data": {
        "task_id": "4011afa265b412380165b415b1400001",
        "status": "DONE",
        "created_at": "2018-09-07T12:50:45.181",
        "updated_at": "2018-09-07T12:50:46.344",
        "zone_id": "4011afa165b1f0e00165b1f8d2a80380",
        "zone_type": "public",
        "language": "zh-cn",
        "total_count": 1,
        "success_count": 0,
        "error_count": 1,
        "error_items": [
          {
            "name": "test.import.",
            "type": "A",
            "line": "default_view",
            "ttl": "300",
            "value": [
              "192.168.1.1",
              "192.168.222.111"
            ],
            "error_code": "DNS.0806",
            "error_message": "This line is not be supported in this DNS version."
          }
        ]
      }
    }
    ```


## 返回值<a name="section34728767"></a>

请参考[通用请求返回值](通用请求返回值.md)。

