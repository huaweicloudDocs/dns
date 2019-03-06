# 查询批量导入内网Record Set任务状态<a name="ZH-CN_TOPIC_0152545794"></a>

## 功能介绍<a name="zh-cn_topic_0152472909_section2763065016101"></a>

查询批量导入内网Record Set任务状态。

## URI<a name="zh-cn_topic_0152472909_section53701671161015"></a>

-   URI格式

    GET /v2/zones/\{zone\_id\}/import/private/recordsets


## 请求<a name="zh-cn_topic_0152472909_section35049099184932"></a>

-   参数说明

    **表 1**  请求格式参数说明

    <a name="zh-cn_topic_0152472909_table30807893173129"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0152472909_row38661368173129"><th class="cellrowborder" valign="top" width="17.66%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0152472909_p14212988173129"><a name="zh-cn_topic_0152472909_p14212988173129"></a><a name="zh-cn_topic_0152472909_p14212988173129"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0152472909_p23287688173129"><a name="zh-cn_topic_0152472909_p23287688173129"></a><a name="zh-cn_topic_0152472909_p23287688173129"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.669999999999998%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0152472909_p44375381151955"><a name="zh-cn_topic_0152472909_p44375381151955"></a><a name="zh-cn_topic_0152472909_p44375381151955"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.69%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0152472909_p1114682173129"><a name="zh-cn_topic_0152472909_p1114682173129"></a><a name="zh-cn_topic_0152472909_p1114682173129"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0152472909_row59855830152715"><td class="cellrowborder" valign="top" width="17.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0152472909_p16484038152715"><a name="zh-cn_topic_0152472909_p16484038152715"></a><a name="zh-cn_topic_0152472909_p16484038152715"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0152472909_p60138711152715"><a name="zh-cn_topic_0152472909_p60138711152715"></a><a name="zh-cn_topic_0152472909_p60138711152715"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.669999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0152472909_p37636093151955"><a name="zh-cn_topic_0152472909_p37636093151955"></a><a name="zh-cn_topic_0152472909_p37636093151955"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.69%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0152472909_p39397424152715"><a name="zh-cn_topic_0152472909_p39397424152715"></a><a name="zh-cn_topic_0152472909_p39397424152715"></a>导入Record Set的zone id。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    无


## 响应<a name="zh-cn_topic_0152472909_section11315292"></a>

-   要素说明

    <a name="zh-cn_topic_0152472909_zh-cn_topic_0037129969_table21574462"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0152472909_zh-cn_topic_0037129969_row41580444"><th class="cellrowborder" valign="top" width="20.41%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p12572829"><a name="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p12572829"></a><a name="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p12572829"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.47%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p13543581"><a name="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p13543581"></a><a name="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p13543581"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.120000000000005%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p23288300"><a name="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p23288300"></a><a name="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p23288300"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0152472909_zh-cn_topic_0037129969_row7304143"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p54764719"><a name="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p54764719"></a><a name="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p54764719"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p10465156"><a name="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p10465156"></a><a name="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p10465156"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p45797138"><a name="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p45797138"></a><a name="zh-cn_topic_0152472909_zh-cn_topic_0037129969_p45797138"></a>响应码</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0152472909_row689994972815"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0152472909_p689974992813"><a name="zh-cn_topic_0152472909_p689974992813"></a><a name="zh-cn_topic_0152472909_p689974992813"></a>data</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0152472909_p148991049202818"><a name="zh-cn_topic_0152472909_p148991049202818"></a><a name="zh-cn_topic_0152472909_p148991049202818"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0152472909_p108996498281"><a name="zh-cn_topic_0152472909_p108996498281"></a><a name="zh-cn_topic_0152472909_p108996498281"></a>响应数据</p>
    </td>
    </tr>
    </tbody>
    </table>


## 返回值<a name="zh-cn_topic_0152472909_section61705107"></a>

请参考[通用请求返回值](通用请求返回值.md)。

