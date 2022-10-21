# 批量删除单个Zone下的Record Set<a name="dns_api_64008"></a>

## 功能介绍<a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_section29105235"></a>

批量删除某个Zone下的Record Set资源，当删除的资源不存在时，则默认删除成功。

响应结果中只包含本次实际删除的资源。

## URI<a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_section60620523"></a>

-   URI格式

    DELETE /v2.1/zones/\{zone\_id\}/recordsets

-   参数说明

    **表 1**  URI格式的参数说明

    <a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_table40248354"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_row24110047"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p6756797"><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p6756797"></a><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p6756797"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p10429724"><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p10429724"></a><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p10429724"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.14141414141414%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p39501348"><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p39501348"></a><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p39501348"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p45492604"><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p45492604"></a><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p45492604"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_row67046586114158"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0117871072_p855371017254"><a name="zh-cn_topic_0117871072_p855371017254"></a><a name="zh-cn_topic_0117871072_p855371017254"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0117871072_p2176187717254"><a name="zh-cn_topic_0117871072_p2176187717254"></a><a name="zh-cn_topic_0117871072_p2176187717254"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0117871072_p1788163317254"><a name="zh-cn_topic_0117871072_p1788163317254"></a><a name="zh-cn_topic_0117871072_p1788163317254"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0117871072_p3912620217254"><a name="zh-cn_topic_0117871072_p3912620217254"></a><a name="zh-cn_topic_0117871072_p3912620217254"></a>所属Zone id。</p>
    <p id="p2171125516411"><a name="p2171125516411"></a><a name="p2171125516411"></a>公网Zone ID可以通过<a href="查询公网Zone列表.md">查询公网Zone列表</a>获取。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_section8713795"></a>

-   参数说明

    **表 2**  请求样例的参数说明

    <a name="zh-cn_topic_0117871072_zh-cn_topic_0037134404_table9470531173211"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0117871072_row56563138212436"><th class="cellrowborder" valign="top" width="22.43%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0117871072_p18211479212436"><a name="zh-cn_topic_0117871072_p18211479212436"></a><a name="zh-cn_topic_0117871072_p18211479212436"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.61%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0117871072_p65843680212436"><a name="zh-cn_topic_0117871072_p65843680212436"></a><a name="zh-cn_topic_0117871072_p65843680212436"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.59%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0117871072_p31737862212436"><a name="zh-cn_topic_0117871072_p31737862212436"></a><a name="zh-cn_topic_0117871072_p31737862212436"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.37%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0117871072_p20630000212436"><a name="zh-cn_topic_0117871072_p20630000212436"></a><a name="zh-cn_topic_0117871072_p20630000212436"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0117871072_row46539514114141"><td class="cellrowborder" valign="top" width="22.43%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0117871072_p43765688114141"><a name="zh-cn_topic_0117871072_p43765688114141"></a><a name="zh-cn_topic_0117871072_p43765688114141"></a>recordset_ids</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.61%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0117871072_p55359806114141"><a name="zh-cn_topic_0117871072_p55359806114141"></a><a name="zh-cn_topic_0117871072_p55359806114141"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.59%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0117871072_p54959301114141"><a name="zh-cn_topic_0117871072_p54959301114141"></a><a name="zh-cn_topic_0117871072_p54959301114141"></a>List&lt;string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0117871072_p87350939633"><a name="zh-cn_topic_0117871072_p87350939633"></a><a name="zh-cn_topic_0117871072_p87350939633"></a>Record Set ID列表。</p>
    <p id="zh-cn_topic_0117871072_p2930291216428"><a name="zh-cn_topic_0117871072_p2930291216428"></a><a name="zh-cn_topic_0117871072_p2930291216428"></a>最多支持100个。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "recordset_ids": [
           "2c9eb155587194ec01587224c9f9014a",
           "2c9eb155587194ec01587224c9f9014c"
        ]
    }
    ```


## 响应<a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_section11315292"></a>

-   要素说明

    **表 3**  响应样例的要素说明

    <a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_table21574462"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_row41580444"><th class="cellrowborder" valign="top" width="20.41%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p12572829"><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p12572829"></a><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p12572829"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.47%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p13543581"><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p13543581"></a><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p13543581"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.120000000000005%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p23288300"><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p23288300"></a><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p23288300"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_row7304143"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p54764719"><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p54764719"></a><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p54764719"></a>recordsets</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p10465156"><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p10465156"></a><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p10465156"></a>列表数据结构</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p45797138"><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p45797138"></a><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p45797138"></a>recordset列表对象。recordsets字段说明，请参见<a href="#table39323385618">表4</a></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_row2133747418458"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p5781953918458"><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p5781953918458"></a><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p5781953918458"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p5469790918458"><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p5469790918458"></a><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p5469790918458"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p5673028518536"><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p5673028518536"></a><a name="zh-cn_topic_0117871072_zh-cn_topic_0037129969_p5673028518536"></a>返回满足过滤条件的资源总数。metadata字段说明请参见<a href="#zh-cn_topic_0093127233_table9971756154520">表5</a>。</p>
    </td>
    </tr>
    <tr id="row868068113814"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p288749251572"><a name="zh-cn_topic_0037139748_p288749251572"></a><a name="zh-cn_topic_0037139748_p288749251572"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p571676251572"><a name="zh-cn_topic_0037139748_p571676251572"></a><a name="zh-cn_topic_0037139748_p571676251572"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p660161572"><a name="zh-cn_topic_0037139748_p660161572"></a><a name="zh-cn_topic_0037139748_p660161572"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p14741433184311"><a name="p14741433184311"></a><a name="p14741433184311"></a>详细信息请参见<a href="#zh-cn_topic_0093127233_table11888161342410">表6</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  recordsets参数说明

    <a name="table39323385618"></a>
    <table><thead align="left"><tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row52466955175323"><th class="cellrowborder" valign="top" width="27.889999999999997%" id="mcps1.2.4.1.1"><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p2769858175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p2769858175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p2769858175323"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.2.4.1.2"><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p46296309175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p46296309175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p46296309175323"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.3%" id="mcps1.2.4.1.3"><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p62697904175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p62697904175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p62697904175323"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row47909891175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p64112397175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p64112397175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p64112397175323"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p1660870175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p1660870175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p1660870175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p1249204175323"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p1249204175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p1249204175323"></a>Record Set的ID。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row6942422175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p64097412175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p64097412175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p64097412175323"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p44990515175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p44990515175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p44990515175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p32019574175323"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p32019574175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p32019574175323"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row61442071175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p51194416175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p51194416175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p51194416175323"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p63301991175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p63301991175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p63301991175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p43966660175323"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p43966660175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p43966660175323"></a>Record Set的描述信息。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row2176746175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p11805366175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p11805366175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p11805366175323"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p1051908175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p1051908175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p1051908175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p10043845175323"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p10043845175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p10043845175323"></a>托管该记录的zone_id。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row61212722175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p8318586175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p8318586175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p8318586175323"></a>zone_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p31287919175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p31287919175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p31287919175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p16372315175323"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p16372315175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p16372315175323"></a>托管该记录的zone_name。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row38132372175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p37461920175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p37461920175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p37461920175323"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p27536075175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p27536075175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p27536075175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p24813356175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p24813356175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p24813356175323"></a>记录类型。</p>
    <p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p52445812175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p52445812175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p52445812175323"></a>取值范围：A，AAAA，MX，CNAME，TXT，NS（仅限公网Zone），SRV，CAA（仅限公网Zone）。</p>
    <p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p15442435577"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p15442435577"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p15442435577"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a>。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row20796819175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p4811553175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p4811553175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p4811553175323"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p47559731175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p47559731175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p47559731175323"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p123031523174010"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p123031523174010"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p123031523174010"></a>解析记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p1030317233408"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p1030317233408"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p1030317233408"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row13978060175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p43388342175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p43388342175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p43388342175323"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p29596719175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p29596719175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p29596719175323"></a>List&lt;string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p30492925175323"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p30492925175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p30492925175323"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row23148559175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p36524189175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p36524189175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p36524189175323"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p47080972175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p47080972175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p47080972175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p15737135175323"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p15737135175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p15737135175323"></a>创建时间。</p>
    <p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p91253279589"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p91253279589"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p91253279589"></a>格式：yyyy-MM-dd'T'HH:mm:ss.SSS</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row33465792175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p42570937175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p42570937175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p42570937175323"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p27449776175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p27449776175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p27449776175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p63703533175323"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p63703533175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p63703533175323"></a>更新时间。</p>
    <p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p1291282918585"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p1291282918585"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p1291282918585"></a>格式：yyyy-MM-dd'T'HH:mm:ss.SSS</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row17850883175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p36228271175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p36228271175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p36228271175323"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p6480061175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p6480061175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p6480061175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p65781854175323"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p65781854175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p65781854175323"></a>资源状态。</p>
    <p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p17497161105814"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p17497161105814"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p17497161105814"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row61184424175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p49633411175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p49633411175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p49633411175323"></a>default</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p56048766175323"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p56048766175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p56048766175323"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p37768157175323"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p37768157175323"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p37768157175323"></a>标识是否由系统默认生成，系统默认生成的Record Set不能删除。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row15199048201026"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p23163408201026"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p23163408201026"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p23163408201026"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p40653752201026"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p40653752201026"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p40653752201026"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p4619625201026"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p4619625201026"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p4619625201026"></a>该Record Set所属的项目ID。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row3965248419366"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p2132803819366"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p2132803819366"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p2132803819366"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p1127763319366"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p1127763319366"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p1127763319366"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p4107308719366"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p4107308719366"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p4107308719366"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p8605123216466"><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p8605123216466"></a><a name="dns_api_64007_zh-cn_topic_0120180015_dns_api_64001_p8605123216466"></a>详细信息请参见<a href="数据结构.md#table0172144213344">表1</a>。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row15869402143342"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p13813035143342"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p13813035143342"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p13813035143342"></a>line</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p45114021143342"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p45114021143342"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p45114021143342"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p30357067143342"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p30357067143342"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p30357067143342"></a>解析线路ID。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row5250267143345"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p46748947143345"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p46748947143345"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p46748947143345"></a>weight</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p28568349143345"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p28568349143345"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p28568349143345"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p32334952143345"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p32334952143345"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p32334952143345"></a>解析记录的权重。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row2642850715221"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p6033434615221"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p6033434615221"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p6033434615221"></a>health_check_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p5524385315221"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p5524385315221"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p5524385315221"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p4556711715221"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p4556711715221"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p4556711715221"></a>健康检查ID。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_row67748315437"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p1777583174312"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p1777583174312"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p1777583174312"></a>alias_target</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p477512344313"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p477512344313"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p477512344313"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p7775113154320"><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p7775113154320"></a><a name="dns_api_64007_zh-cn_topic_0120180015_zh-cn_topic_0082840627_p7775113154320"></a>别名记录。详细信息请参见<a href="数据结构.md#table11888161342410">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  metadata参数说明

    <a name="zh-cn_topic_0093127233_table9971756154520"></a>
    <table><thead align="left"><tr id="dns_api_65003_r1ee98e923a7c4bfcaa89e708d3fca79e"><th class="cellrowborder" valign="top" width="18.43184318431843%" id="mcps1.2.4.1.1"><p id="dns_api_65003_af493c2fde22f44069c2b5ea0467dfe89"><a name="dns_api_65003_af493c2fde22f44069c2b5ea0467dfe89"></a><a name="dns_api_65003_af493c2fde22f44069c2b5ea0467dfe89"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.571957195719573%" id="mcps1.2.4.1.2"><p id="dns_api_65003_a581940a484df4c8294e51f11391a23c8"><a name="dns_api_65003_a581940a484df4c8294e51f11391a23c8"></a><a name="dns_api_65003_a581940a484df4c8294e51f11391a23c8"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="61.996199619962%" id="mcps1.2.4.1.3"><p id="dns_api_65003_a0301bbf5a1234ea3a88a104e1b4cff92"><a name="dns_api_65003_a0301bbf5a1234ea3a88a104e1b4cff92"></a><a name="dns_api_65003_a0301bbf5a1234ea3a88a104e1b4cff92"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="dns_api_65003_r7cc02a0ecbd24482bca90faa98114b18"><td class="cellrowborder" valign="top" width="18.43184318431843%" headers="mcps1.2.4.1.1 "><p id="dns_api_65003_a9234858cb2f447539b4b85a307884322"><a name="dns_api_65003_a9234858cb2f447539b4b85a307884322"></a><a name="dns_api_65003_a9234858cb2f447539b4b85a307884322"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.571957195719573%" headers="mcps1.2.4.1.2 "><p id="dns_api_65003_af14a2a2c8f0345f4811bb21dd2a9b667"><a name="dns_api_65003_af14a2a2c8f0345f4811bb21dd2a9b667"></a><a name="dns_api_65003_af14a2a2c8f0345f4811bb21dd2a9b667"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.996199619962%" headers="mcps1.2.4.1.3 "><p id="dns_api_65003_a39058f9901c84eb9a776ca5cd44ede29"><a name="dns_api_65003_a39058f9901c84eb9a776ca5cd44ede29"></a><a name="dns_api_65003_a39058f9901c84eb9a776ca5cd44ede29"></a>满足查询条件的资源总数，不受分页（即limit、offset参数）影响。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  links对象参数说明

    <a name="zh-cn_topic_0093127233_table11888161342410"></a>
    <table><thead align="left"><tr id="dns_api_80006_row917304253418"><th class="cellrowborder" valign="top" width="18%" id="mcps1.2.4.1.1"><p id="dns_api_80006_p101731742153416"><a name="dns_api_80006_p101731742153416"></a><a name="dns_api_80006_p101731742153416"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.25%" id="mcps1.2.4.1.2"><p id="dns_api_80006_p0174542163418"><a name="dns_api_80006_p0174542163418"></a><a name="dns_api_80006_p0174542163418"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.74999999999999%" id="mcps1.2.4.1.3"><p id="dns_api_80006_p7174194243414"><a name="dns_api_80006_p7174194243414"></a><a name="dns_api_80006_p7174194243414"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="dns_api_80006_row1390694871216"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="dns_api_80006_p8907184881217"><a name="dns_api_80006_p8907184881217"></a><a name="dns_api_80006_p8907184881217"></a>self</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.25%" headers="mcps1.2.4.1.2 "><p id="dns_api_80006_p9907184891219"><a name="dns_api_80006_p9907184891219"></a><a name="dns_api_80006_p9907184891219"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.74999999999999%" headers="mcps1.2.4.1.3 "><p id="dns_api_80006_p1890754813127"><a name="dns_api_80006_p1890754813127"></a><a name="dns_api_80006_p1890754813127"></a>当前资源的链接。</p>
    </td>
    </tr>
    <tr id="dns_api_80006_row15778204719370"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="dns_api_80006_p136561245153620"><a name="dns_api_80006_p136561245153620"></a><a name="dns_api_80006_p136561245153620"></a>next</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.25%" headers="mcps1.2.4.1.2 "><p id="dns_api_80006_p19656144517367"><a name="dns_api_80006_p19656144517367"></a><a name="dns_api_80006_p19656144517367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.74999999999999%" headers="mcps1.2.4.1.3 "><p id="dns_api_80006_p76567451365"><a name="dns_api_80006_p76567451365"></a><a name="dns_api_80006_p76567451365"></a>下一页资源的链接。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "links": {
            "self": "https://Endpoint/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets"
        },
        "recordsets": [
            {
                "id": "2c9eb155587194ec01587224c9f9014a",
                "name": "example.com.",
                "type": "A",
                "ttl": 300,
                "records": [
                    "1.1.1.1"
                ],
                "status": "PENDING_DELETE",
                "links": {
                    "self": "https://Endpoint/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587194ec01587224c9f9014a"
                },
                "zone_id": "2c9eb155587194ec01587224c9f90149",
                "zone_name": "example.com.",
                "created_at": "2016-11-17T11:56:03.439",
                "updated_at": "2016-11-17T11:56:06.439",
                "default": false,
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
                "line": "default_view",
                "weight": null,
                "set_id": null
            },
            {
                "id": "2c9eb155587194ec01587224c9f9014c",
                "name": "1.example.com.",
                "type": "A",
                "ttl": 172800,
                "records": [
                    "2.2.2.2"
                ],
                "status": "PENDING_DELETE",
                "links": {
                    "self": "https://Endpoint/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587194ec01587224c9f9014c"
                },
                "zone_id": "2c9eb155587194ec01587224c9f90149",
                "zone_name": "example.com.",
                "created_at": "2016-11-17T11:56:03.439",
                "updated_at": "2016-11-17T11:56:06.439",
                "default": false,
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
                "line": "default_view",
                "weight": null,
                "set_id": null
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

