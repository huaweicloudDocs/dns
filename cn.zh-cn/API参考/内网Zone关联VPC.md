# 内网Zone关联VPC<a name="ZH-CN_TOPIC_0057329431"></a>

## 功能介绍<a name="section3569153217343"></a>

在内网Zone上关联VPC。

## URI<a name="section6163262617350"></a>

POST /v2/zones/\{zone\_id\}/associaterouter

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
<td class="cellrowborder" valign="top" width="51.55%" headers="mcps1.2.5.1.4 "><p id="p20315403"><a name="p20315403"></a><a name="p20315403"></a>待关联zone的ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section4207148117353"></a>

-   参数说明

    **表 2**  请求样例的参数说明

    <a name="table3720408817742"></a>
    <table><thead align="left"><tr id="row6225671717742"><th class="cellrowborder" valign="top" width="17.91%" id="mcps1.2.5.1.1"><p id="p5153686617742"><a name="p5153686617742"></a><a name="p5153686617742"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.959999999999999%" id="mcps1.2.5.1.2"><p id="p473035017742"><a name="p473035017742"></a><a name="p473035017742"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.04%" id="mcps1.2.5.1.3"><p id="p386753717742"><a name="p386753717742"></a><a name="p386753717742"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.09%" id="mcps1.2.5.1.4"><p id="p5956810717742"><a name="p5956810717742"></a><a name="p5956810717742"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1329410717742"><td class="cellrowborder" valign="top" width="17.91%" headers="mcps1.2.5.1.1 "><p id="p2681781817157"><a name="p2681781817157"></a><a name="p2681781817157"></a>router</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.5.1.2 "><p id="p6603174617742"><a name="p6603174617742"></a><a name="p6603174617742"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.04%" headers="mcps1.2.5.1.3 "><p id="p9188475171518"><a name="p9188475171518"></a><a name="p9188475171518"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.09%" headers="mcps1.2.5.1.4 "><p id="p36712148171536"><a name="p36712148171536"></a><a name="p36712148171536"></a>需要关联的Router(VPC)，详细信息请参见<a href="#ZH-CN_TOPIC_0057329431__table4448008117179">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  Router对象参数说明

    <a name="table4448008117179"></a>
    <table><thead align="left"><tr id="row6132935617179"><th class="cellrowborder" valign="top" width="18.088191180881914%" id="mcps1.2.5.1.1"><p id="p36588677171719"><a name="p36588677171719"></a><a name="p36588677171719"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.728427157284273%" id="mcps1.2.5.1.2"><p id="p10892865171719"><a name="p10892865171719"></a><a name="p10892865171719"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.14828517148285%" id="mcps1.2.5.1.3"><p id="p9906869171719"><a name="p9906869171719"></a><a name="p9906869171719"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.035096490350966%" id="mcps1.2.5.1.4"><p id="p64258954171719"><a name="p64258954171719"></a><a name="p64258954171719"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row266872817179"><td class="cellrowborder" valign="top" width="18.088191180881914%" headers="mcps1.2.5.1.1 "><p id="p25118582171719"><a name="p25118582171719"></a><a name="p25118582171719"></a>router_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.728427157284273%" headers="mcps1.2.5.1.2 "><p id="p21339228171719"><a name="p21339228171719"></a><a name="p21339228171719"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.14828517148285%" headers="mcps1.2.5.1.3 "><p id="p50755907171719"><a name="p50755907171719"></a><a name="p50755907171719"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.035096490350966%" headers="mcps1.2.5.1.4 "><p id="p17587794171719"><a name="p17587794171719"></a><a name="p17587794171719"></a>Router(VPC)的ID。</p>
    </td>
    </tr>
    <tr id="row6657832817179"><td class="cellrowborder" valign="top" width="18.088191180881914%" headers="mcps1.2.5.1.1 "><p id="p3709384171719"><a name="p3709384171719"></a><a name="p3709384171719"></a>router_region</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.728427157284273%" headers="mcps1.2.5.1.2 "><p id="p32024676171719"><a name="p32024676171719"></a><a name="p32024676171719"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.14828517148285%" headers="mcps1.2.5.1.3 "><p id="p43861924171719"><a name="p43861924171719"></a><a name="p43861924171719"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.035096490350966%" headers="mcps1.2.5.1.4 "><p id="p63154928171719"><a name="p63154928171719"></a><a name="p63154928171719"></a>Router(VPC)所在的region。</p>
    <p id="p31477322172059"><a name="p31477322172059"></a><a name="p31477322172059"></a>如果为空，默认为token中project所在的region。</p>
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

    <a name="table4512106017551"></a>
    <table><thead align="left"><tr id="row2225931917551"><th class="cellrowborder" valign="top" width="21.63%" id="mcps1.2.4.1.1"><p id="p5817443517551"><a name="p5817443517551"></a><a name="p5817443517551"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.02%" id="mcps1.2.4.1.2"><p id="p3436442517551"><a name="p3436442517551"></a><a name="p3436442517551"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.35%" id="mcps1.2.4.1.3"><p id="p3205505917551"><a name="p3205505917551"></a><a name="p3205505917551"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row4632297717551"><td class="cellrowborder" valign="top" width="21.63%" headers="mcps1.2.4.1.1 "><p id="p6117366017551"><a name="p6117366017551"></a><a name="p6117366017551"></a>router_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.02%" headers="mcps1.2.4.1.2 "><p id="p4937778317551"><a name="p4937778317551"></a><a name="p4937778317551"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.35%" headers="mcps1.2.4.1.3 "><p id="p4017744717551"><a name="p4017744717551"></a><a name="p4017744717551"></a>Router(VPC)的ID。</p>
    </td>
    </tr>
    <tr id="row2605270417551"><td class="cellrowborder" valign="top" width="21.63%" headers="mcps1.2.4.1.1 "><p id="p2989427417551"><a name="p2989427417551"></a><a name="p2989427417551"></a>router_region</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.02%" headers="mcps1.2.4.1.2 "><p id="p4423327117551"><a name="p4423327117551"></a><a name="p4423327117551"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.35%" headers="mcps1.2.4.1.3 "><p id="p2612521117551"><a name="p2612521117551"></a><a name="p2612521117551"></a>Router(VPC)所在的region。</p>
    </td>
    </tr>
    <tr id="row16652885175519"><td class="cellrowborder" valign="top" width="21.63%" headers="mcps1.2.4.1.1 "><p id="p38120631175524"><a name="p38120631175524"></a><a name="p38120631175524"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.02%" headers="mcps1.2.4.1.2 "><p id="p57184665175519"><a name="p57184665175519"></a><a name="p57184665175519"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.35%" headers="mcps1.2.4.1.3 "><p id="p1635999216648"><a name="p1635999216648"></a><a name="p1635999216648"></a>任务处理状态。</p>
    <p id="p24990280175620"><a name="p24990280175620"></a><a name="p24990280175620"></a>包括PENDING_CREATE、PENDING_DELETE、ACTIVE、ERROR。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "status": "PENDING_CREATE",
        "router_id": "f0791650-db8c-4a20-8a44-a06c6e24b15b",
        "router_region": "xx"
    }
    
    ```


## 返回值<a name="section1917896317411"></a>

请参考[通用请求返回值](通用请求返回值.md)。

