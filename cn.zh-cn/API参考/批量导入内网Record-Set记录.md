# 批量导入内网Record Set记录<a name="ZH-CN_TOPIC_0152545793"></a>

## 功能介绍<a name="zh-cn_topic_0152472908_section2763065016101"></a>

批量导入内网Record Set记录。

## URI<a name="zh-cn_topic_0152472908_section53701671161015"></a>

POST /v2/zones/\{zone\_id\}/import/private/recordsets

## 请求<a name="zh-cn_topic_0152472908_section35049099184932"></a>

-   参数说明

    **表 1**  请求格式参数说明

    <a name="zh-cn_topic_0152472908_table30807893173129"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0152472908_row38661368173129"><th class="cellrowborder" valign="top" width="17.66%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0152472908_p14212988173129"><a name="zh-cn_topic_0152472908_p14212988173129"></a><a name="zh-cn_topic_0152472908_p14212988173129"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0152472908_p23287688173129"><a name="zh-cn_topic_0152472908_p23287688173129"></a><a name="zh-cn_topic_0152472908_p23287688173129"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.669999999999998%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0152472908_p44375381151955"><a name="zh-cn_topic_0152472908_p44375381151955"></a><a name="zh-cn_topic_0152472908_p44375381151955"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.69%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0152472908_p1114682173129"><a name="zh-cn_topic_0152472908_p1114682173129"></a><a name="zh-cn_topic_0152472908_p1114682173129"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0152472908_row59855830152715"><td class="cellrowborder" valign="top" width="17.66%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0152472908_p16484038152715"><a name="zh-cn_topic_0152472908_p16484038152715"></a><a name="zh-cn_topic_0152472908_p16484038152715"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0152472908_p60138711152715"><a name="zh-cn_topic_0152472908_p60138711152715"></a><a name="zh-cn_topic_0152472908_p60138711152715"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.669999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0152472908_p37636093151955"><a name="zh-cn_topic_0152472908_p37636093151955"></a><a name="zh-cn_topic_0152472908_p37636093151955"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.69%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0152472908_p39397424152715"><a name="zh-cn_topic_0152472908_p39397424152715"></a><a name="zh-cn_topic_0152472908_p39397424152715"></a>zone id</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    无


## 响应<a name="zh-cn_topic_0152472908_section11315292"></a>

-   要素说明
-   响应样例的要素说明

    <a name="zh-cn_topic_0152472908_zh-cn_topic_0037129969_table21574462"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0152472908_zh-cn_topic_0037129969_row41580444"><th class="cellrowborder" valign="top" width="20.41%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p12572829"><a name="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p12572829"></a><a name="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p12572829"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.47%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p13543581"><a name="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p13543581"></a><a name="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p13543581"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.120000000000005%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p23288300"><a name="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p23288300"></a><a name="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p23288300"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0152472908_zh-cn_topic_0037129969_row7304143"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p54764719"><a name="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p54764719"></a><a name="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p54764719"></a>task_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p10465156"><a name="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p10465156"></a><a name="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p10465156"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p45797138"><a name="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p45797138"></a><a name="zh-cn_topic_0152472908_zh-cn_topic_0037129969_p45797138"></a>任务id</p>
    </td>
    </tr>
    </tbody>
    </table>


## 返回值<a name="zh-cn_topic_0152472908_section61705107"></a>

请参考[通用请求返回值](通用请求返回值.md)。

