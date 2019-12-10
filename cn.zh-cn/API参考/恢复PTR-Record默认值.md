# 恢复PTR Record默认值<a name="zh-cn_topic_0042318616"></a>

## 功能介绍<a name="section8391370"></a>

将弹性IP的PTR记录恢复为默认值。

## URI<a name="section8413469"></a>

PATCH /v2/reverse/floatingips/\{region\}:\{floatingip\_id\}

参数说明请参见[表1](#table48883615)。

**表 1**  URI格式的参数说明

<a name="table48883615"></a>
<table><thead align="left"><tr id="rf5eb1b4b32f8403bb0acf9d017b51ee5"><th class="cellrowborder" valign="top" width="18.11%" id="mcps1.2.5.1.1"><p id="a3c7e1e08fe294e3e82e1797588253df5"><a name="a3c7e1e08fe294e3e82e1797588253df5"></a><a name="a3c7e1e08fe294e3e82e1797588253df5"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.91%" id="mcps1.2.5.1.2"><p id="adc5414917a3c400cb8857a02b29eb94d"><a name="adc5414917a3c400cb8857a02b29eb94d"></a><a name="adc5414917a3c400cb8857a02b29eb94d"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.83%" id="mcps1.2.5.1.3"><p id="a9ce61a6198d44964bdc496d82601e141"><a name="a9ce61a6198d44964bdc496d82601e141"></a><a name="a9ce61a6198d44964bdc496d82601e141"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50.14999999999999%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0042318613_p517246718149"><a name="zh-cn_topic_0042318613_p517246718149"></a><a name="zh-cn_topic_0042318613_p517246718149"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="rfa1eb070d71448a9b2fbaa5917068657"><td class="cellrowborder" valign="top" width="18.11%" headers="mcps1.2.5.1.1 "><p id="ae661ce94166a4825a0aad48ed9e3a0e3"><a name="ae661ce94166a4825a0aad48ed9e3a0e3"></a><a name="ae661ce94166a4825a0aad48ed9e3a0e3"></a>region</p>
</td>
<td class="cellrowborder" valign="top" width="17.91%" headers="mcps1.2.5.1.2 "><p id="ac4b80f38e0ef4382be487f39931804d3"><a name="ac4b80f38e0ef4382be487f39931804d3"></a><a name="ac4b80f38e0ef4382be487f39931804d3"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.83%" headers="mcps1.2.5.1.3 "><p id="a0a1bf1099829467e967689705fc84fe5"><a name="a0a1bf1099829467e967689705fc84fe5"></a><a name="a0a1bf1099829467e967689705fc84fe5"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.14999999999999%" headers="mcps1.2.5.1.4 "><p id="a939d47bc868d44c290326fb1df4c5e00"><a name="a939d47bc868d44c290326fb1df4c5e00"></a><a name="a939d47bc868d44c290326fb1df4c5e00"></a>租户的区域信息。</p>
<p id="p5433349018149"><a name="p5433349018149"></a><a name="p5433349018149"></a>详细内容请参见<a href="终端节点.md">终端节点</a>。</p>
</td>
</tr>
<tr id="r0588e91c222b4483b97fe5b2e56f79bb"><td class="cellrowborder" valign="top" width="18.11%" headers="mcps1.2.5.1.1 "><p id="ac3563e9e05cc422ab54a9d288aa5810c"><a name="ac3563e9e05cc422ab54a9d288aa5810c"></a><a name="ac3563e9e05cc422ab54a9d288aa5810c"></a>floatingip_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.91%" headers="mcps1.2.5.1.2 "><p id="af475fd33d3fc4310b7f5a1f14e1fa9c9"><a name="af475fd33d3fc4310b7f5a1f14e1fa9c9"></a><a name="af475fd33d3fc4310b7f5a1f14e1fa9c9"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.83%" headers="mcps1.2.5.1.3 "><p id="a2fe0b089a6a14db1a241b4d93dc9fd5a"><a name="a2fe0b089a6a14db1a241b4d93dc9fd5a"></a><a name="a2fe0b089a6a14db1a241b4d93dc9fd5a"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.14999999999999%" headers="mcps1.2.5.1.4 "><p id="ad2fce4accef8431b86dcaca0bd572a60"><a name="ad2fce4accef8431b86dcaca0bd572a60"></a><a name="ad2fce4accef8431b86dcaca0bd572a60"></a>弹性IP的ID。</p>
<p id="p5553155134916"><a name="p5553155134916"></a><a name="p5553155134916"></a>可以通过网络控制台的弹性公网IP页面获取或者通过<a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090598.html" target="_blank" rel="noopener noreferrer">查询弹性公网IP列表</a>获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section8612359"></a>

-   参数说明

    **表 2**  请求样例的参数说明

    <a name="table239794161830"></a>
    <table><thead align="left"><tr id="row654560711830"><th class="cellrowborder" valign="top" width="17.008299170082992%" id="mcps1.2.5.1.1"><p id="p3415211830"><a name="p3415211830"></a><a name="p3415211830"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.098190180981902%" id="mcps1.2.5.1.2"><p id="p276632601830"><a name="p276632601830"></a><a name="p276632601830"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.72852714728527%" id="mcps1.2.5.1.3"><p id="p261316001830"><a name="p261316001830"></a><a name="p261316001830"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="50.16498350164984%" id="mcps1.2.5.1.4"><p id="p362848191830"><a name="p362848191830"></a><a name="p362848191830"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row533892641830"><td class="cellrowborder" valign="top" width="17.008299170082992%" headers="mcps1.2.5.1.1 "><p id="p295631171830"><a name="p295631171830"></a><a name="p295631171830"></a>ptrdname</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.098190180981902%" headers="mcps1.2.5.1.2 "><p id="p458022581830"><a name="p458022581830"></a><a name="p458022581830"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.72852714728527%" headers="mcps1.2.5.1.3 "><p id="p189954321830"><a name="p189954321830"></a><a name="p189954321830"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.16498350164984%" headers="mcps1.2.5.1.4 "><p id="p26704373161818"><a name="p26704373161818"></a><a name="p26704373161818"></a>PTR记录对应的域名。</p>
    <p id="p622350301830"><a name="p622350301830"></a><a name="p622350301830"></a>此处值为null。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    恢复ID为“_region\_id_:c5504932-bf23-4171-b655-b87a6bc59334”的弹性IP的PTR为默认值。

    ```
    PATCH https://{DNS_Endpoint}/v2/reverse/floatingips/region_id:c5504932-bf23-4171-b655-b87a6bc59334
    ```

    ```
    {
        "ptrdname": null
    }
    ```


## 响应<a name="section10402369"></a>

无

## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

