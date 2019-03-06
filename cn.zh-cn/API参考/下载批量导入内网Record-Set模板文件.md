# 下载批量导入内网Record Set模板文件<a name="ZH-CN_TOPIC_0152545796"></a>

## 功能介绍<a name="section2763065016101"></a>

下载批量导入Record Set的模板。

## URI<a name="section53701671161015"></a>

GET /v2/templates/import/private/recordset?locale=\{locale\}

参数说明请参见[表1](#table30807893173129)。

**表 1**  URI格式的参数说明

<a name="table30807893173129"></a>
<table><thead align="left"><tr id="row38661368173129"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p14212988173129"><a name="p14212988173129"></a><a name="p14212988173129"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p23287688173129"><a name="p23287688173129"></a><a name="p23287688173129"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p1114682173129"><a name="p1114682173129"></a><a name="p1114682173129"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row6301875173129"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p5124116173129"><a name="p5124116173129"></a><a name="p5124116173129"></a>locale</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p166665209417"><a name="p166665209417"></a><a name="p166665209417"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p807379194116"><a name="p807379194116"></a><a name="p807379194116"></a>导入模板所属语言。</p>
<p id="p56820233173129"><a name="p56820233173129"></a><a name="p56820233173129"></a>取值范围：zh-cn（中文），en-us（英文）</p>
<p id="p6265006894134"><a name="p6265006894134"></a><a name="p6265006894134"></a>默认为zh-cn。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="zh-cn_topic_0152498197_section35049099184932"></a>

-   参数说明

    无

-   请求样例

    无


## 响应<a name="zh-cn_topic_0152498197_section11315292"></a>

-   要素说明

    <a name="zh-cn_topic_0152498197_zh-cn_topic_0037129969_table21574462"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0152498197_zh-cn_topic_0037129969_row41580444"><th class="cellrowborder" valign="top" width="20.41%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p12572829"><a name="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p12572829"></a><a name="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p12572829"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.47%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p13543581"><a name="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p13543581"></a><a name="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p13543581"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.120000000000005%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p23288300"><a name="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p23288300"></a><a name="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p23288300"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0152498197_zh-cn_topic_0037129969_row7304143"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p54764719"><a name="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p54764719"></a><a name="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p54764719"></a>FileRepresentation</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p10465156"><a name="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p10465156"></a><a name="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p10465156"></a>File</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p45797138"><a name="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p45797138"></a><a name="zh-cn_topic_0152498197_zh-cn_topic_0037129969_p45797138"></a>文件模板。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 返回值<a name="zh-cn_topic_0152498197_section61705107"></a>

请参考[通用请求返回值](通用请求返回值.md)。

