# 查询公网Zone的名称服务器<a name="ZH-CN_TOPIC_0057343056"></a>

## 功能介绍<a name="section55898385"></a>

查询单个公网Zone的名称服务器。

## URI<a name="section33323423"></a>

GET /v2/zones/\{zone\_id\}/nameservers

参数说明请参见[表1](#table14024165)。

**表 1**  URI格式的参数说明

<a name="table14024165"></a>
<table><thead align="left"><tr id="row26592044"><th class="cellrowborder" valign="top" width="15.459999999999999%" id="mcps1.2.5.1.1"><p id="p6471942"><a name="p6471942"></a><a name="p6471942"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.459999999999999%" id="mcps1.2.5.1.2"><p id="p54465313"><a name="p54465313"></a><a name="p54465313"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.53%" id="mcps1.2.5.1.3"><p id="p49614245"><a name="p49614245"></a><a name="p49614245"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.55%" id="mcps1.2.5.1.4"><p id="p59330872"><a name="p59330872"></a><a name="p59330872"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row41071365"><td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.5.1.1 "><p id="p38446258"><a name="p38446258"></a><a name="p38446258"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.5.1.2 "><p id="p27139175"><a name="p27139175"></a><a name="p27139175"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.2.5.1.3 "><p id="p50789581"><a name="p50789581"></a><a name="p50789581"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="51.55%" headers="mcps1.2.5.1.4 "><p id="p20315403"><a name="p20315403"></a><a name="p20315403"></a>待查询zone的ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section31475357"></a>

无

## 响应<a name="section14842765"></a>

-   要素说明

    **表 2**  响应样例的要素说明

    <a name="table2534644119347"></a>
    <table><thead align="left"><tr id="row2134485619347"><th class="cellrowborder" valign="top" width="18.47%" id="mcps1.2.4.1.1"><p id="p5121175619347"><a name="p5121175619347"></a><a name="p5121175619347"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.59%" id="mcps1.2.4.1.2"><p id="p5451156519347"><a name="p5451156519347"></a><a name="p5451156519347"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="59.940000000000005%" id="mcps1.2.4.1.3"><p id="p5336061019347"><a name="p5336061019347"></a><a name="p5336061019347"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2724213119347"><td class="cellrowborder" valign="top" width="18.47%" headers="mcps1.2.4.1.1 "><p id="p5912903419347"><a name="p5912903419347"></a><a name="p5912903419347"></a>nameservers</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.59%" headers="mcps1.2.4.1.2 "><p id="p2472241219347"><a name="p2472241219347"></a><a name="p2472241219347"></a><em id="i26985596193639"><a name="i26985596193639"></a><a name="i26985596193639"></a>列表数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="59.940000000000005%" headers="mcps1.2.4.1.3 "><p id="p64387025171923"><a name="p64387025171923"></a><a name="p64387025171923"></a>name server列表对象。</p>
    <p id="p60737358161124"><a name="p60737358161124"></a><a name="p60737358161124"></a>nameservers参数说明，请参见<a href="#table3847447219326">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  nameservers参数说明

    <a name="table3847447219326"></a>
    <table><thead align="left"><tr id="row3833649519326"><th class="cellrowborder" valign="top" width="18.47%" id="mcps1.2.4.1.1"><p id="p3493722219342"><a name="p3493722219342"></a><a name="p3493722219342"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.33%" id="mcps1.2.4.1.2"><p id="p1134272819342"><a name="p1134272819342"></a><a name="p1134272819342"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.2%" id="mcps1.2.4.1.3"><p id="p4634576219342"><a name="p4634576219342"></a><a name="p4634576219342"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3753895719326"><td class="cellrowborder" valign="top" width="18.47%" headers="mcps1.2.4.1.1 "><p id="p19222756195728"><a name="p19222756195728"></a><a name="p19222756195728"></a>hostname</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p13539398195728"><a name="p13539398195728"></a><a name="p13539398195728"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="p22949440195728"><a name="p22949440195728"></a><a name="p22949440195728"></a>主机名。</p>
    </td>
    </tr>
    <tr id="row4963379019326"><td class="cellrowborder" valign="top" width="18.47%" headers="mcps1.2.4.1.1 "><p id="p20035160195728"><a name="p20035160195728"></a><a name="p20035160195728"></a>priority</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p12235287195728"><a name="p12235287195728"></a><a name="p12235287195728"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="p51534186195728"><a name="p51534186195728"></a><a name="p51534186195728"></a>优先级。</p>
    <p id="p63758461163042"><a name="p63758461163042"></a><a name="p63758461163042"></a>示例：</p>
    <p id="p19928749162855"><a name="p19928749162855"></a><a name="p19928749162855"></a>如果priority的值为“1”，表示会第一个采用该域名服务器进行解析。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "nameservers": [
            {
                "hostname": "ns1.example.com.", 
                "priority": 1 
            }, 
            {
                "hostname": "ns2.example.com.", 
                "priority": 2
            }
        ]
    }
    
    ```


## 返回值<a name="section66476022"></a>

请参考[通用请求返回值](通用请求返回值.md)。

