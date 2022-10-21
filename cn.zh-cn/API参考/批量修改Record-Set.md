# 批量修改Record Set<a name="dns_api_64009"></a>

## 功能介绍<a name="zh-cn_topic_0136957256_section2763065016101"></a>

批量修改RecordSet。属于原子性操作，请求Record Set将全部完成修改，或不做任何修改。

仅公网Zone支持。

## URI<a name="zh-cn_topic_0136957256_zh-cn_topic_0037129969_section60620523"></a>

-   URI格式

    PUT /v2.1/zones/\{zone\_id\}/recordsets

-   参数说明

    **表 1**  URI格式的参数说明

    <a name="zh-cn_topic_0136957256_table30807893173129"></a>
    <table><thead align="left"><tr id="dns_api_64007_zh-cn_topic_0093127233_row38661368173129"><th class="cellrowborder" valign="top" width="17.66%" id="mcps1.2.5.1.1"><p id="dns_api_64007_zh-cn_topic_0093127233_p14212988173129"><a name="dns_api_64007_zh-cn_topic_0093127233_p14212988173129"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p14212988173129"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.2"><p id="dns_api_64007_zh-cn_topic_0093127233_p23287688173129"><a name="dns_api_64007_zh-cn_topic_0093127233_p23287688173129"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p23287688173129"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.3"><p id="dns_api_64007_zh-cn_topic_0093127233_p44375381151955"><a name="dns_api_64007_zh-cn_topic_0093127233_p44375381151955"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p44375381151955"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="50.38%" id="mcps1.2.5.1.4"><p id="dns_api_64007_zh-cn_topic_0093127233_p1114682173129"><a name="dns_api_64007_zh-cn_topic_0093127233_p1114682173129"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p1114682173129"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="dns_api_64007_zh-cn_topic_0093127233_row59855830152715"><td class="cellrowborder" valign="top" width="17.66%" headers="mcps1.2.5.1.1 "><p id="dns_api_64007_zh-cn_topic_0093127233_p16484038152715"><a name="dns_api_64007_zh-cn_topic_0093127233_p16484038152715"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p16484038152715"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="dns_api_64007_zh-cn_topic_0093127233_p60138711152715"><a name="dns_api_64007_zh-cn_topic_0093127233_p60138711152715"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p60138711152715"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.3 "><p id="dns_api_64007_zh-cn_topic_0093127233_p37636093151955"><a name="dns_api_64007_zh-cn_topic_0093127233_p37636093151955"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p37636093151955"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.38%" headers="mcps1.2.5.1.4 "><p id="dns_api_64007_zh-cn_topic_0093127233_p39397424152715"><a name="dns_api_64007_zh-cn_topic_0093127233_p39397424152715"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p39397424152715"></a>所属Zone ID。</p>
    <p id="dns_api_64007_p2171125516411"><a name="dns_api_64007_p2171125516411"></a><a name="dns_api_64007_p2171125516411"></a>公网Zone ID可以通过<a href="查询公网Zone列表.md">查询公网Zone列表</a>获取。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="zh-cn_topic_0136957256_zh-cn_topic_0037129969_section8713795"></a>

-   参数说明

    **表 2**  请求样例的参数说明

    <a name="zh-cn_topic_0136957256_table22319179103010"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0136957256_row7527145103010"><th class="cellrowborder" valign="top" width="22.45%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0136957256_p5719038103010"><a name="zh-cn_topic_0136957256_p5719038103010"></a><a name="zh-cn_topic_0136957256_p5719038103010"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.59%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0136957256_p60588956103010"><a name="zh-cn_topic_0136957256_p60588956103010"></a><a name="zh-cn_topic_0136957256_p60588956103010"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.59%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0136957256_p8758378103010"><a name="zh-cn_topic_0136957256_p8758378103010"></a><a name="zh-cn_topic_0136957256_p8758378103010"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.37%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0136957256_p38339984103010"><a name="zh-cn_topic_0136957256_p38339984103010"></a><a name="zh-cn_topic_0136957256_p38339984103010"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0136957256_row18530999103010"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0136957256_p24615942103010"><a name="zh-cn_topic_0136957256_p24615942103010"></a><a name="zh-cn_topic_0136957256_p24615942103010"></a>recordsets</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.59%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0136957256_p47734310103010"><a name="zh-cn_topic_0136957256_p47734310103010"></a><a name="zh-cn_topic_0136957256_p47734310103010"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.59%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0136957256_p41273919103010"><a name="zh-cn_topic_0136957256_p41273919103010"></a><a name="zh-cn_topic_0136957256_p41273919103010"></a>Array of object</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p45797138"><a name="p45797138"></a><a name="p45797138"></a>recordset列表对象，详细信息请参见<a href="#zh-cn_topic_0136957256_zh-cn_topic_0037134404_table9470531173211">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  recordsets参数说明

    <a name="zh-cn_topic_0136957256_zh-cn_topic_0037134404_table9470531173211"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0136957256_row56563138212436"><th class="cellrowborder" valign="top" width="24.89%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0136957256_p18211479212436"><a name="zh-cn_topic_0136957256_p18211479212436"></a><a name="zh-cn_topic_0136957256_p18211479212436"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.149999999999999%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0136957256_p65843680212436"><a name="zh-cn_topic_0136957256_p65843680212436"></a><a name="zh-cn_topic_0136957256_p65843680212436"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.59%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0136957256_p31737862212436"><a name="zh-cn_topic_0136957256_p31737862212436"></a><a name="zh-cn_topic_0136957256_p31737862212436"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.37%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0136957256_p20630000212436"><a name="zh-cn_topic_0136957256_p20630000212436"></a><a name="zh-cn_topic_0136957256_p20630000212436"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0136957256_row44558375102626"><td class="cellrowborder" valign="top" width="24.89%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0136957256_p41560275102626"><a name="zh-cn_topic_0136957256_p41560275102626"></a><a name="zh-cn_topic_0136957256_p41560275102626"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.149999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0136957256_p10939087102626"><a name="zh-cn_topic_0136957256_p10939087102626"></a><a name="zh-cn_topic_0136957256_p10939087102626"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.59%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0136957256_p13650880102626"><a name="zh-cn_topic_0136957256_p13650880102626"></a><a name="zh-cn_topic_0136957256_p13650880102626"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0136957256_p31979534102626"><a name="zh-cn_topic_0136957256_p31979534102626"></a><a name="zh-cn_topic_0136957256_p31979534102626"></a>RecordSet资源ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0136957256_row4988353103238"><td class="cellrowborder" valign="top" width="24.89%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0136957256_p1403466103238"><a name="zh-cn_topic_0136957256_p1403466103238"></a><a name="zh-cn_topic_0136957256_p1403466103238"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.149999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0136957256_p46571891103238"><a name="zh-cn_topic_0136957256_p46571891103238"></a><a name="zh-cn_topic_0136957256_p46571891103238"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.59%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0136957256_p14226788103238"><a name="zh-cn_topic_0136957256_p14226788103238"></a><a name="zh-cn_topic_0136957256_p14226788103238"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0136957256_p11519174103238"><a name="zh-cn_topic_0136957256_p11519174103238"></a><a name="zh-cn_topic_0136957256_p11519174103238"></a>RecordSet资源描述。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0136957256_row503639010339"><td class="cellrowborder" valign="top" width="24.89%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0136957256_p24655236103318"><a name="zh-cn_topic_0136957256_p24655236103318"></a><a name="zh-cn_topic_0136957256_p24655236103318"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.149999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0136957256_p50917085103318"><a name="zh-cn_topic_0136957256_p50917085103318"></a><a name="zh-cn_topic_0136957256_p50917085103318"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.59%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0136957256_p30643219103318"><a name="zh-cn_topic_0136957256_p30643219103318"></a><a name="zh-cn_topic_0136957256_p30643219103318"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p575713445225"><a name="p575713445225"></a><a name="p575713445225"></a>Record Set的有效缓存时间，以秒为单位。</p>
    <p id="p175784417226"><a name="p175784417226"></a><a name="p175784417226"></a>取值范围：300-2147483647。</p>
    <p id="p1075754442219"><a name="p1075754442219"></a><a name="p1075754442219"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0136957256_row48786871103348"><td class="cellrowborder" valign="top" width="24.89%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0136957256_p59687896103357"><a name="zh-cn_topic_0136957256_p59687896103357"></a><a name="zh-cn_topic_0136957256_p59687896103357"></a>weight</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.149999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0136957256_p2881387103357"><a name="zh-cn_topic_0136957256_p2881387103357"></a><a name="zh-cn_topic_0136957256_p2881387103357"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.59%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0136957256_p32065766103357"><a name="zh-cn_topic_0136957256_p32065766103357"></a><a name="zh-cn_topic_0136957256_p32065766103357"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p313140112313"><a name="p313140112313"></a><a name="p313140112313"></a>解析记录的权重，默认为null。</p>
    <a name="ul3131201239"></a><a name="ul3131201239"></a><ul id="ul3131201239"><li>当weight=null时，表示该解析记录不设置权重。</li><li>当weight=0，表示备用域名解析记录。</li><li>当weight&gt;0，表示主用域名解析记录。</li></ul>
    <p id="p813150102316"><a name="p813150102316"></a><a name="p813150102316"></a>取值范围：0~100</p>
    <p id="p11318015231"><a name="p11318015231"></a><a name="p11318015231"></a>在相同域名、类型、线路下的解析记录，规则如下：</p>
    <a name="ul71310013233"></a><a name="ul71310013233"></a><ul id="ul71310013233"><li>全部设置权重，或全部不设置权重。</li><li>当不设置权重时，只能创建一个解析记录。</li><li>当设置权重时，最多能创建20个解析记录。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0136957256_row34777092102626"><td class="cellrowborder" valign="top" width="24.89%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0136957256_p50324954102626"><a name="zh-cn_topic_0136957256_p50324954102626"></a><a name="zh-cn_topic_0136957256_p50324954102626"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.149999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0136957256_p49789511102626"><a name="zh-cn_topic_0136957256_p49789511102626"></a><a name="zh-cn_topic_0136957256_p49789511102626"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.59%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0136957256_p6418580102626"><a name="zh-cn_topic_0136957256_p6418580102626"></a><a name="zh-cn_topic_0136957256_p6418580102626"></a>List&lt;string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0136957256_p11222164102626"><a name="zh-cn_topic_0136957256_p11222164102626"></a><a name="zh-cn_topic_0136957256_p11222164102626"></a>解析记录值。</p>
    <p id="p2611319234"><a name="p2611319234"></a><a name="p2611319234"></a>不同Type对应的Value值规则不同。</p>
    <p id="p176111332310"><a name="p176111332310"></a><a name="p176111332310"></a>如Type为AAAA类型，Value是域名对应的IPv6地址列表。</p>
    <p id="p165138237"><a name="p165138237"></a><a name="p165138237"></a>具体参见《云解析服务用户指南》中“<a href="https://support.huaweicloud.com/usermanual-dns/dns_usermanual_0601.html" target="_blank" rel="noopener noreferrer">管理记录集</a>”章节的说明及请求样例。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "recordsets": [
            {
                "id": "2c9eb155587194ec01587224c9f9014a",
                "description": "This is an type A record set.",
                "ttl": 3600,
                "weight": 10,
                "records": [
                    "192.168.10.1",
                    "192.168.10.2"
                ]
            },
            {
                "id": "2c9eb155587194ec01587224c9f9014c",
                "description": "This is an type AAAA record set.",
                "ttl": 300,
                "weight": 5,
                "records": [
                    "fe80:0:0:0:202:b3ff:fe1e:8329",
                    "ff03:0db8:85a3:0:0:8a2e:0370:7334"
                ]
            }
        ]
    }
    ```


## 响应<a name="zh-cn_topic_0136957256_section40090803161031"></a>

-   参数说明

    **表 4**  响应样例的要素说明

    <a name="dns_api_64007_zh-cn_topic_0093127233_table21574462"></a>
    <table><thead align="left"><tr id="dns_api_64007_zh-cn_topic_0093127233_row41580444"><th class="cellrowborder" valign="top" width="20.41%" id="mcps1.2.4.1.1"><p id="dns_api_64007_zh-cn_topic_0093127233_p12572829"><a name="dns_api_64007_zh-cn_topic_0093127233_p12572829"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p12572829"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.47%" id="mcps1.2.4.1.2"><p id="dns_api_64007_zh-cn_topic_0093127233_p13543581"><a name="dns_api_64007_zh-cn_topic_0093127233_p13543581"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p13543581"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.120000000000005%" id="mcps1.2.4.1.3"><p id="dns_api_64007_zh-cn_topic_0093127233_p23288300"><a name="dns_api_64007_zh-cn_topic_0093127233_p23288300"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p23288300"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="dns_api_64007_zh-cn_topic_0093127233_row7304143"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0093127233_p54764719"><a name="dns_api_64007_zh-cn_topic_0093127233_p54764719"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p54764719"></a>recordsets</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0093127233_p10465156"><a name="dns_api_64007_zh-cn_topic_0093127233_p10465156"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p10465156"></a><em id="dns_api_64007_zh-cn_topic_0093127233_i44918310194055"><a name="dns_api_64007_zh-cn_topic_0093127233_i44918310194055"></a><a name="dns_api_64007_zh-cn_topic_0093127233_i44918310194055"></a>列表数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0093127233_p45797138"><a name="dns_api_64007_zh-cn_topic_0093127233_p45797138"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p45797138"></a>recordset列表对象。</p>
    <p id="dns_api_64007_p18829223105414"><a name="dns_api_64007_p18829223105414"></a><a name="dns_api_64007_p18829223105414"></a>recordsets字段说明，请参见<a href="#dns_api_64007_zh-cn_topic_0093127233_table7669703175323">表5</a></p>
    </td>
    </tr>
    <tr id="dns_api_64007_zh-cn_topic_0093127233_row2133747418458"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0093127233_p5781953918458"><a name="dns_api_64007_zh-cn_topic_0093127233_p5781953918458"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p5781953918458"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0093127233_p5469790918458"><a name="dns_api_64007_zh-cn_topic_0093127233_p5469790918458"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p5469790918458"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_p105219307549"><a name="dns_api_64007_p105219307549"></a><a name="dns_api_64007_p105219307549"></a>资源总数。</p>
    <p id="dns_api_64007_zh-cn_topic_0093127233_p5673028518536"><a name="dns_api_64007_zh-cn_topic_0093127233_p5673028518536"></a><a name="dns_api_64007_zh-cn_topic_0093127233_p5673028518536"></a>metadata字段说明请参见<a href="#dns_api_64007_zh-cn_topic_0093127233_table9971756154520">表6</a>。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_row11738171517255"><td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_zh-cn_topic_0037139748_p288749251572"><a name="dns_api_64007_zh-cn_topic_0037139748_p288749251572"></a><a name="dns_api_64007_zh-cn_topic_0037139748_p288749251572"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_zh-cn_topic_0037139748_p571676251572"><a name="dns_api_64007_zh-cn_topic_0037139748_p571676251572"></a><a name="dns_api_64007_zh-cn_topic_0037139748_p571676251572"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.120000000000005%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_zh-cn_topic_0037139748_p660161572"><a name="dns_api_64007_zh-cn_topic_0037139748_p660161572"></a><a name="dns_api_64007_zh-cn_topic_0037139748_p660161572"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="dns_api_64007_p14741433184311"><a name="dns_api_64007_p14741433184311"></a><a name="dns_api_64007_p14741433184311"></a>详细信息请参见<a href="#dns_api_64007_zh-cn_topic_0093127233_table11888161342410">表7</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  recordsets参数说明

    <a name="dns_api_64007_zh-cn_topic_0093127233_table7669703175323"></a>
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

    **表 6**  metadata参数说明

    <a name="dns_api_64007_zh-cn_topic_0093127233_table9971756154520"></a>
    <table><thead align="left"><tr id="dns_api_64007_dns_api_65003_r1ee98e923a7c4bfcaa89e708d3fca79e"><th class="cellrowborder" valign="top" width="18.43184318431843%" id="mcps1.2.4.1.1"><p id="dns_api_64007_dns_api_65003_af493c2fde22f44069c2b5ea0467dfe89"><a name="dns_api_64007_dns_api_65003_af493c2fde22f44069c2b5ea0467dfe89"></a><a name="dns_api_64007_dns_api_65003_af493c2fde22f44069c2b5ea0467dfe89"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.571957195719573%" id="mcps1.2.4.1.2"><p id="dns_api_64007_dns_api_65003_a581940a484df4c8294e51f11391a23c8"><a name="dns_api_64007_dns_api_65003_a581940a484df4c8294e51f11391a23c8"></a><a name="dns_api_64007_dns_api_65003_a581940a484df4c8294e51f11391a23c8"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="61.996199619962%" id="mcps1.2.4.1.3"><p id="dns_api_64007_dns_api_65003_a0301bbf5a1234ea3a88a104e1b4cff92"><a name="dns_api_64007_dns_api_65003_a0301bbf5a1234ea3a88a104e1b4cff92"></a><a name="dns_api_64007_dns_api_65003_a0301bbf5a1234ea3a88a104e1b4cff92"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="dns_api_64007_dns_api_65003_r7cc02a0ecbd24482bca90faa98114b18"><td class="cellrowborder" valign="top" width="18.43184318431843%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_dns_api_65003_a9234858cb2f447539b4b85a307884322"><a name="dns_api_64007_dns_api_65003_a9234858cb2f447539b4b85a307884322"></a><a name="dns_api_64007_dns_api_65003_a9234858cb2f447539b4b85a307884322"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.571957195719573%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_dns_api_65003_af14a2a2c8f0345f4811bb21dd2a9b667"><a name="dns_api_64007_dns_api_65003_af14a2a2c8f0345f4811bb21dd2a9b667"></a><a name="dns_api_64007_dns_api_65003_af14a2a2c8f0345f4811bb21dd2a9b667"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="61.996199619962%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_dns_api_65003_a39058f9901c84eb9a776ca5cd44ede29"><a name="dns_api_64007_dns_api_65003_a39058f9901c84eb9a776ca5cd44ede29"></a><a name="dns_api_64007_dns_api_65003_a39058f9901c84eb9a776ca5cd44ede29"></a>满足查询条件的资源总数，不受分页（即limit、offset参数）影响。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 7**  links对象参数说明

    <a name="dns_api_64007_zh-cn_topic_0093127233_table11888161342410"></a>
    <table><thead align="left"><tr id="dns_api_64007_dns_api_80006_row917304253418"><th class="cellrowborder" valign="top" width="18%" id="mcps1.2.4.1.1"><p id="dns_api_64007_dns_api_80006_p101731742153416"><a name="dns_api_64007_dns_api_80006_p101731742153416"></a><a name="dns_api_64007_dns_api_80006_p101731742153416"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.25%" id="mcps1.2.4.1.2"><p id="dns_api_64007_dns_api_80006_p0174542163418"><a name="dns_api_64007_dns_api_80006_p0174542163418"></a><a name="dns_api_64007_dns_api_80006_p0174542163418"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.74999999999999%" id="mcps1.2.4.1.3"><p id="dns_api_64007_dns_api_80006_p7174194243414"><a name="dns_api_64007_dns_api_80006_p7174194243414"></a><a name="dns_api_64007_dns_api_80006_p7174194243414"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="dns_api_64007_dns_api_80006_row1390694871216"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_dns_api_80006_p8907184881217"><a name="dns_api_64007_dns_api_80006_p8907184881217"></a><a name="dns_api_64007_dns_api_80006_p8907184881217"></a>self</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.25%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_dns_api_80006_p9907184891219"><a name="dns_api_64007_dns_api_80006_p9907184891219"></a><a name="dns_api_64007_dns_api_80006_p9907184891219"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.74999999999999%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_dns_api_80006_p1890754813127"><a name="dns_api_64007_dns_api_80006_p1890754813127"></a><a name="dns_api_64007_dns_api_80006_p1890754813127"></a>当前资源的链接。</p>
    </td>
    </tr>
    <tr id="dns_api_64007_dns_api_80006_row15778204719370"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="dns_api_64007_dns_api_80006_p136561245153620"><a name="dns_api_64007_dns_api_80006_p136561245153620"></a><a name="dns_api_64007_dns_api_80006_p136561245153620"></a>next</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.25%" headers="mcps1.2.4.1.2 "><p id="dns_api_64007_dns_api_80006_p19656144517367"><a name="dns_api_64007_dns_api_80006_p19656144517367"></a><a name="dns_api_64007_dns_api_80006_p19656144517367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.74999999999999%" headers="mcps1.2.4.1.3 "><p id="dns_api_64007_dns_api_80006_p76567451365"><a name="dns_api_64007_dns_api_80006_p76567451365"></a><a name="dns_api_64007_dns_api_80006_p76567451365"></a>下一页资源的链接。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "links": {
            "self": "https://Endpoint/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets/batch/lines"
        },
        "recordsets": [
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
                    "self": "https://
    Endpoint/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587228570158722b6ac30007"
                },
                "zone_id": "2c9eb155587194ec01587224c9f90149",
                "zone_name": "example.com.",
                "created_at": "2016-11-17T12:03:17.827",
                "updated_at": null,
                "health_check_id": "e55c6f3dc4e34c8e86353b664ae0e89f",
                "default": false,
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
                "line": "default_view",
                "weight": 0
            },
            {
                "id": "2c9eb155587228570158722b6ac30008",
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
                    "self": "https://Endpoint/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587228570158722b6ac30008"
                },
                "zone_id": "2c9eb155587194ec01587224c9f90149",
                "zone_name": "example.com.",
                "created_at": "2016-11-17T12:03:17.827",
                "updated_at": null,
                "health_check_id": "e55c6f3dc4e34c8e86353b664ae0e89c",
                "default": false,
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
                "line": "Abroad",
                "weight": 0
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

