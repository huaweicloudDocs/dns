# 内网Zone解关联VPC<a name="ZH-CN_TOPIC_0057331452"></a>

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
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.2.5.1.3 "><p id="p50789581"><a name="p50789581"></a><a name="p50789581"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="51.55%" headers="mcps1.2.5.1.4 "><p id="p20315403"><a name="p20315403"></a><a name="p20315403"></a>待解关联zone的ID。</p>
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
    <td class="cellrowborder" valign="top" width="17.599999999999998%" headers="mcps1.2.5.1.3 "><p id="p159862761815"><a name="p159862761815"></a><a name="p159862761815"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.53%" headers="mcps1.2.5.1.4 "><p id="p198200141815"><a name="p198200141815"></a><a name="p198200141815"></a>需要解关联的Router(VPC)，详细信息请参见<a href="#ZH-CN_TOPIC_0057331452__table441624051815">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  Router对象参数说明

    <a name="table441624051815"></a>
    <table><thead align="left"><tr id="row9315751815"><th class="cellrowborder" valign="top" width="18.09%" id="mcps1.2.5.1.1"><p id="p83487181815"><a name="p83487181815"></a><a name="p83487181815"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="12.72%" id="mcps1.2.5.1.2"><p id="p51575781815"><a name="p51575781815"></a><a name="p51575781815"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.71%" id="mcps1.2.5.1.3"><p id="p151107071815"><a name="p151107071815"></a><a name="p151107071815"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.480000000000004%" id="mcps1.2.5.1.4"><p id="p160077601815"><a name="p160077601815"></a><a name="p160077601815"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row215602021815"><td class="cellrowborder" valign="top" width="18.09%" headers="mcps1.2.5.1.1 "><p id="p15459281815"><a name="p15459281815"></a><a name="p15459281815"></a>router_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.72%" headers="mcps1.2.5.1.2 "><p id="p581113471815"><a name="p581113471815"></a><a name="p581113471815"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.71%" headers="mcps1.2.5.1.3 "><p id="p93986421815"><a name="p93986421815"></a><a name="p93986421815"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.480000000000004%" headers="mcps1.2.5.1.4 "><p id="p230925261815"><a name="p230925261815"></a><a name="p230925261815"></a>Router(VPC)的ID。</p>
    </td>
    </tr>
    <tr id="row65061421815"><td class="cellrowborder" valign="top" width="18.09%" headers="mcps1.2.5.1.1 "><p id="p572354551815"><a name="p572354551815"></a><a name="p572354551815"></a>router_region</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.72%" headers="mcps1.2.5.1.2 "><p id="p55602731815"><a name="p55602731815"></a><a name="p55602731815"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.71%" headers="mcps1.2.5.1.3 "><p id="p477289551815"><a name="p477289551815"></a><a name="p477289551815"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.480000000000004%" headers="mcps1.2.5.1.4 "><p id="p408401661815"><a name="p408401661815"></a><a name="p408401661815"></a>Router(VPC)所在的region。</p>
    <p id="p50046718172120"><a name="p50046718172120"></a><a name="p50046718172120"></a>如果为空，默认为token中project所在的region。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

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
    <td class="cellrowborder" valign="top" width="22.02%" headers="mcps1.2.4.1.2 "><p id="p2380847318844"><a name="p2380847318844"></a><a name="p2380847318844"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.35%" headers="mcps1.2.4.1.3 "><p id="p4943817618844"><a name="p4943817618844"></a><a name="p4943817618844"></a>Router(VPC)的ID。</p>
    </td>
    </tr>
    <tr id="row4229040718844"><td class="cellrowborder" valign="top" width="21.63%" headers="mcps1.2.4.1.1 "><p id="p297095218844"><a name="p297095218844"></a><a name="p297095218844"></a>router_region</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.02%" headers="mcps1.2.4.1.2 "><p id="p3932056118844"><a name="p3932056118844"></a><a name="p3932056118844"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.35%" headers="mcps1.2.4.1.3 "><p id="p3084890718844"><a name="p3084890718844"></a><a name="p3084890718844"></a>Router(VPC)所在的region。</p>
    </td>
    </tr>
    <tr id="row920471418844"><td class="cellrowborder" valign="top" width="21.63%" headers="mcps1.2.4.1.1 "><p id="p738436818844"><a name="p738436818844"></a><a name="p738436818844"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.02%" headers="mcps1.2.4.1.2 "><p id="p6126290618844"><a name="p6126290618844"></a><a name="p6126290618844"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.35%" headers="mcps1.2.4.1.3 "><p id="p940787516628"><a name="p940787516628"></a><a name="p940787516628"></a>任务处理状态。</p>
    <p id="p6334833618844"><a name="p6334833618844"></a><a name="p6334833618844"></a>包括PENDING_CREATE、PENDING_DELETE、ACTIVE, ERROR。</p>
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


## 返回值<a name="section1917896317411"></a>

请参考[通用请求返回值](通用请求返回值.md)。

