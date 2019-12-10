# 内网Zone解关联VPC<a name="zh-cn_topic_0057331452"></a>

## 功能介绍<a name="section3569153217343"></a>

在Private Zone上解关联VPC。

当Private Zone仅关联一个VPC时，不能进行解关联操作。

## URI<a name="section6163262617350"></a>

POST /v2/zones/\{zone\_id\}/disassociaterouter

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
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.2.5.1.3 "><p id="p50789581"><a name="p50789581"></a><a name="p50789581"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.55%" headers="mcps1.2.5.1.4 "><p id="p20315403"><a name="p20315403"></a><a name="p20315403"></a>待解关联zone的ID。</p>
<p id="p1669018482183"><a name="p1669018482183"></a><a name="p1669018482183"></a>可以通过<a href="查询内网Zone列表.md">查询内网Zone列表</a>获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section4207148117353"></a>

-   参数说明

    **表 2**  请求样例的参数说明

    <a name="table72706611815"></a>
    <table><thead align="left"><tr id="row255897031815"><th class="cellrowborder" valign="top" width="15.47%" id="mcps1.2.5.1.1"><p id="p595000771815"><a name="p595000771815"></a><a name="p595000771815"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.4%" id="mcps1.2.5.1.2"><p id="p547769391815"><a name="p547769391815"></a><a name="p547769391815"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.599999999999998%" id="mcps1.2.5.1.3"><p id="p77471141815"><a name="p77471141815"></a><a name="p77471141815"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.53%" id="mcps1.2.5.1.4"><p id="p235365301815"><a name="p235365301815"></a><a name="p235365301815"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row274107621815"><td class="cellrowborder" valign="top" width="15.47%" headers="mcps1.2.5.1.1 "><p id="p56792261815"><a name="p56792261815"></a><a name="p56792261815"></a>router</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.4%" headers="mcps1.2.5.1.2 "><p id="p573641711815"><a name="p573641711815"></a><a name="p573641711815"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.599999999999998%" headers="mcps1.2.5.1.3 "><p id="p159862761815"><a name="p159862761815"></a><a name="p159862761815"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.53%" headers="mcps1.2.5.1.4 "><p id="p198200141815"><a name="p198200141815"></a><a name="p198200141815"></a>需要解关联的Router(VPC)，详细信息请参见<a href="#table4448008117179">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  router对象参数说明

    <a name="table4448008117179"></a>
    <table><thead align="left"><tr id="row6132935617179"><th class="cellrowborder" valign="top" width="16.27%" id="mcps1.2.5.1.1"><p id="p36588677171719"><a name="p36588677171719"></a><a name="p36588677171719"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.95%" id="mcps1.2.5.1.2"><p id="p06011644121012"><a name="p06011644121012"></a><a name="p06011644121012"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.380000000000003%" id="mcps1.2.5.1.3"><p id="p9906869171719"><a name="p9906869171719"></a><a name="p9906869171719"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.4%" id="mcps1.2.5.1.4"><p id="p64258954171719"><a name="p64258954171719"></a><a name="p64258954171719"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row266872817179"><td class="cellrowborder" valign="top" width="16.27%" headers="mcps1.2.5.1.1 "><p id="p25118582171719"><a name="p25118582171719"></a><a name="p25118582171719"></a>router_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.95%" headers="mcps1.2.5.1.2 "><p id="p11602144151017"><a name="p11602144151017"></a><a name="p11602144151017"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.380000000000003%" headers="mcps1.2.5.1.3 "><p id="p50755907171719"><a name="p50755907171719"></a><a name="p50755907171719"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.4%" headers="mcps1.2.5.1.4 "><p id="p17587794171719"><a name="p17587794171719"></a><a name="p17587794171719"></a>Router(VPC)所属VPC的ID。</p>
    <p id="p143411822947"><a name="p143411822947"></a><a name="p143411822947"></a>该参数的值可以通过如下两种方式获取：</p>
    <a name="ul1938314911411"></a><a name="ul1938314911411"></a><ul id="ul1938314911411"><li>通过虚拟私有云的管理控制台，在VPC的详情页面中获取VPC的ID。</li><li>通过<a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090625.html" target="_blank" rel="noopener noreferrer">查询VPC列表</a>获取VPC ID。</li></ul>
    </td>
    </tr>
    <tr id="row6657832817179"><td class="cellrowborder" valign="top" width="16.27%" headers="mcps1.2.5.1.1 "><p id="p3709384171719"><a name="p3709384171719"></a><a name="p3709384171719"></a>router_region</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.95%" headers="mcps1.2.5.1.2 "><p id="p8602134413102"><a name="p8602134413102"></a><a name="p8602134413102"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.380000000000003%" headers="mcps1.2.5.1.3 "><p id="p43861924171719"><a name="p43861924171719"></a><a name="p43861924171719"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.4%" headers="mcps1.2.5.1.4 "><p id="p63154928171719"><a name="p63154928171719"></a><a name="p63154928171719"></a>Router(VPC)所在的region。</p>
    <p id="p38645142171939"><a name="p38645142171939"></a><a name="p38645142171939"></a>如果为空，默认为token中project所在的region。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    为Zone ID为“ff8080825b8fc86c015b94bc6f8712c3”的域名解关联VPC。

    ```
    POST https://{DNS_Endpoint}/v2/zones/ff8080825b8fc86c015b94bc6f8712c3/disassociaterouter
    ```

    ```
    {
        "router": {
            "router_id": "f0791650-db8c-4a20-8a44-a06c6e24b15b",
            "router_region": "xx"
        }
    }
    ```


## 响应<a name="section2142173017358"></a>

-   要素说明

    **表 4**  响应样例的要素说明

    <a name="table3895302218844"></a>
    <table><thead align="left"><tr id="row4896688518844"><th class="cellrowborder" valign="top" width="21.63%" id="mcps1.2.4.1.1"><p id="p689472918844"><a name="p689472918844"></a><a name="p689472918844"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.02%" id="mcps1.2.4.1.2"><p id="p2160217018844"><a name="p2160217018844"></a><a name="p2160217018844"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.35%" id="mcps1.2.4.1.3"><p id="p494531118844"><a name="p494531118844"></a><a name="p494531118844"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row6502588818844"><td class="cellrowborder" valign="top" width="21.63%" headers="mcps1.2.4.1.1 "><p id="p3260560718844"><a name="p3260560718844"></a><a name="p3260560718844"></a>router_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.02%" headers="mcps1.2.4.1.2 "><p id="p2380847318844"><a name="p2380847318844"></a><a name="p2380847318844"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.35%" headers="mcps1.2.4.1.3 "><p id="p4943817618844"><a name="p4943817618844"></a><a name="p4943817618844"></a>Router(VPC)的ID。</p>
    </td>
    </tr>
    <tr id="row4229040718844"><td class="cellrowborder" valign="top" width="21.63%" headers="mcps1.2.4.1.1 "><p id="p297095218844"><a name="p297095218844"></a><a name="p297095218844"></a>router_region</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.02%" headers="mcps1.2.4.1.2 "><p id="p3932056118844"><a name="p3932056118844"></a><a name="p3932056118844"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.35%" headers="mcps1.2.4.1.3 "><p id="p3084890718844"><a name="p3084890718844"></a><a name="p3084890718844"></a>Router(VPC)所在的region。</p>
    </td>
    </tr>
    <tr id="row920471418844"><td class="cellrowborder" valign="top" width="21.63%" headers="mcps1.2.4.1.1 "><p id="p738436818844"><a name="p738436818844"></a><a name="p738436818844"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.02%" headers="mcps1.2.4.1.2 "><p id="p6126290618844"><a name="p6126290618844"></a><a name="p6126290618844"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.35%" headers="mcps1.2.4.1.3 "><p id="p940787516628"><a name="p940787516628"></a><a name="p940787516628"></a>资源状态。</p>
    <p id="p998065791017"><a name="p998065791017"></a><a name="p998065791017"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "status": "PENDING_DELETE",
        "router_id": "f0791650-db8c-4a20-8a44-a06c6e24b15b",
        "router_region": "xx"
    }
    
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

