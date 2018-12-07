# 恢复PTR Record默认值<a name="ZH-CN_TOPIC_0042318616"></a>

## 功能介绍<a name="section8391370"></a>

将弹性IP的PTR记录恢复为默认值。

## URI<a name="section8413469"></a>

PATCH /v2/reverse/floatingips/\{region\}:\{floatingip\_id\}

参数说明请参见[表1](#table48883615)。

**表 1**  URI格式的参数说明

<a name="table48883615"></a>
<table><thead align="left"><tr id="zh-cn_topic_0042318613_row3442661918149"><th class="cellrowborder" valign="top" width="22.64%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0042318613_p3709279118149"><a name="zh-cn_topic_0042318613_p3709279118149"></a><a name="zh-cn_topic_0042318613_p3709279118149"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.37%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0042318613_p5172606218149"><a name="zh-cn_topic_0042318613_p5172606218149"></a><a name="zh-cn_topic_0042318613_p5172606218149"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0042318613_p2906151418149"><a name="zh-cn_topic_0042318613_p2906151418149"></a><a name="zh-cn_topic_0042318613_p2906151418149"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.64%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0042318613_p517246718149"><a name="zh-cn_topic_0042318613_p517246718149"></a><a name="zh-cn_topic_0042318613_p517246718149"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0042318613_row1631668818149"><td class="cellrowborder" valign="top" width="22.64%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0042318613_p4658337018149"><a name="zh-cn_topic_0042318613_p4658337018149"></a><a name="zh-cn_topic_0042318613_p4658337018149"></a>region</p>
</td>
<td class="cellrowborder" valign="top" width="17.37%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0042318613_p1515661618149"><a name="zh-cn_topic_0042318613_p1515661618149"></a><a name="zh-cn_topic_0042318613_p1515661618149"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0042318613_p1972638718149"><a name="zh-cn_topic_0042318613_p1972638718149"></a><a name="zh-cn_topic_0042318613_p1972638718149"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="42.64%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0042318613_p5433349018149"><a name="zh-cn_topic_0042318613_p5433349018149"></a><a name="zh-cn_topic_0042318613_p5433349018149"></a>租户的区域信息。</p>
</td>
</tr>
<tr id="zh-cn_topic_0042318613_row1923936518149"><td class="cellrowborder" valign="top" width="22.64%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0042318613_p1488470218149"><a name="zh-cn_topic_0042318613_p1488470218149"></a><a name="zh-cn_topic_0042318613_p1488470218149"></a>floatingip_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.37%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0042318613_p6481017518149"><a name="zh-cn_topic_0042318613_p6481017518149"></a><a name="zh-cn_topic_0042318613_p6481017518149"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0042318613_p1513281718149"><a name="zh-cn_topic_0042318613_p1513281718149"></a><a name="zh-cn_topic_0042318613_p1513281718149"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="42.64%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0042318613_p1779865118149"><a name="zh-cn_topic_0042318613_p1779865118149"></a><a name="zh-cn_topic_0042318613_p1779865118149"></a>弹性IP的ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section8612359"></a>

-   参数说明

    **表 2**  请求样例的参数说明

    <a name="table239794161830"></a>
    <table><thead align="left"><tr id="row654560711830"><th class="cellrowborder" valign="top" width="22.447755224477554%" id="mcps1.2.5.1.1"><p id="p3415211830"><a name="p3415211830"></a><a name="p3415211830"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.42785721427857%" id="mcps1.2.5.1.2"><p id="p276632601830"><a name="p276632601830"></a><a name="p276632601830"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="p261316001830"><a name="p261316001830"></a><a name="p261316001830"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.77612238776123%" id="mcps1.2.5.1.4"><p id="p362848191830"><a name="p362848191830"></a><a name="p362848191830"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row533892641830"><td class="cellrowborder" valign="top" width="22.447755224477554%" headers="mcps1.2.5.1.1 "><p id="p295631171830"><a name="p295631171830"></a><a name="p295631171830"></a>ptrdname</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.2 "><p id="p458022581830"><a name="p458022581830"></a><a name="p458022581830"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="p189954321830"><a name="p189954321830"></a><a name="p189954321830"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.77612238776123%" headers="mcps1.2.5.1.4 "><p id="p26704373161818"><a name="p26704373161818"></a><a name="p26704373161818"></a>PTR记录对应的域名。</p>
    <p id="p622350301830"><a name="p622350301830"></a><a name="p622350301830"></a>此处值为null。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "ptrdname": null
    }
    ```


## 响应<a name="section10402369"></a>

无

## 返回值<a name="section26512460"></a>

请参考[通用请求返回值](通用请求返回值.md)。

