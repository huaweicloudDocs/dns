# 查询内网Zone<a name="ZH-CN_TOPIC_0057311028"></a>

## 功能介绍<a name="section55898385"></a>

查询单个内网Zone。

## URI<a name="section33323423"></a>

GET /v2/zones/\{zone\_id\}

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

    <a name="table66395488123415"></a>
    <table><thead align="left"><tr id="row29441359123415"><th class="cellrowborder" valign="top" width="18.38%" id="mcps1.2.4.1.1"><p id="p35939865123415"><a name="p35939865123415"></a><a name="p35939865123415"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.33%" id="mcps1.2.4.1.2"><p id="p25447972123415"><a name="p25447972123415"></a><a name="p25447972123415"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.29%" id="mcps1.2.4.1.3"><p id="p48019864123415"><a name="p48019864123415"></a><a name="p48019864123415"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row64403739123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p49320408123415"><a name="p49320408123415"></a><a name="p49320408123415"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p35530101123415"><a name="p35530101123415"></a><a name="p35530101123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p59365914123415"><a name="p59365914123415"></a><a name="p59365914123415"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="row64531184123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p59643381123415"><a name="p59643381123415"></a><a name="p59643381123415"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p66384534123415"><a name="p66384534123415"></a><a name="p66384534123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p8438205123415"><a name="p8438205123415"></a><a name="p8438205123415"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="row8834981123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p44544845123415"><a name="p44544845123415"></a><a name="p44544845123415"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p51362669123415"><a name="p51362669123415"></a><a name="p51362669123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p66735534123415"><a name="p66735534123415"></a><a name="p66735534123415"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="row63748898123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p63387127123415"><a name="p63387127123415"></a><a name="p63387127123415"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p34083648123415"><a name="p34083648123415"></a><a name="p34083648123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p9312102123415"><a name="p9312102123415"></a><a name="p9312102123415"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="row16700055123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p10527186123415"><a name="p10527186123415"></a><a name="p10527186123415"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p47395742123415"><a name="p47395742123415"></a><a name="p47395742123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p13849890123415"><a name="p13849890123415"></a><a name="p13849890123415"></a>zone类型，公网或者内网。</p>
    </td>
    </tr>
    <tr id="row57540153123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p30240837123415"><a name="p30240837123415"></a><a name="p30240837123415"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p33588766123415"><a name="p33588766123415"></a><a name="p33588766123415"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p36335531123415"><a name="p36335531123415"></a><a name="p36335531123415"></a>该zone下SOA记录中的ttl值。</p>
    </td>
    </tr>
    <tr id="row58584329123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p47710208123415"><a name="p47710208123415"></a><a name="p47710208123415"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p39321631123415"><a name="p39321631123415"></a><a name="p39321631123415"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p30935567123415"><a name="p30935567123415"></a><a name="p30935567123415"></a>该zone下SOA记录中用于标识变更的序列值。</p>
    </td>
    </tr>
    <tr id="row9984653123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p3450553123415"><a name="p3450553123415"></a><a name="p3450553123415"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p11059337123415"><a name="p11059337123415"></a><a name="p11059337123415"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p23391077123415"><a name="p23391077123415"></a><a name="p23391077123415"></a>资源状态。</p>
    <p id="p9193108123415"><a name="p9193108123415"></a><a name="p9193108123415"></a>取值范围：PENDING_CREATE, ACTIVE, PENDING_DELETE, ERROR。</p>
    </td>
    </tr>
    <tr id="row15629110123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p57998436123415"><a name="p57998436123415"></a><a name="p57998436123415"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p252886123415"><a name="p252886123415"></a><a name="p252886123415"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p20483829123415"><a name="p20483829123415"></a><a name="p20483829123415"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="row50136736123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p34543853123415"><a name="p34543853123415"></a><a name="p34543853123415"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p46588698123415"><a name="p46588698123415"></a><a name="p46588698123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p15588175123415"><a name="p15588175123415"></a><a name="p15588175123415"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="row6075853123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p22382050123415"><a name="p22382050123415"></a><a name="p22382050123415"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p1006739123415"><a name="p1006739123415"></a><a name="p1006739123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p14437066123415"><a name="p14437066123415"></a><a name="p14437066123415"></a>zone所属的租户ID。</p>
    </td>
    </tr>
    <tr id="row62824730123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p55638354123415"><a name="p55638354123415"></a><a name="p55638354123415"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p10412802123415"><a name="p10412802123415"></a><a name="p10412802123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p38130643123415"><a name="p38130643123415"></a><a name="p38130643123415"></a>创建时间。</p>
    </td>
    </tr>
    <tr id="row7631471123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p14169428123415"><a name="p14169428123415"></a><a name="p14169428123415"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p6873005123415"><a name="p6873005123415"></a><a name="p6873005123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p19842531123415"><a name="p19842531123415"></a><a name="p19842531123415"></a>更新时间。</p>
    </td>
    </tr>
    <tr id="row44365052123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p36799431123415"><a name="p36799431123415"></a><a name="p36799431123415"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p27963939123415"><a name="p27963939123415"></a><a name="p27963939123415"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p5501274116741"><a name="p5501274116741"></a><a name="p5501274116741"></a>指向当前资源或者其他资源的链接。</p>
    <p id="p50486583123415"><a name="p50486583123415"></a><a name="p50486583123415"></a>当查询需要分页时，需要包含一个next链接指向下一页。</p>
    </td>
    </tr>
    <tr id="row51726070123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p29062162123415"><a name="p29062162123415"></a><a name="p29062162123415"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p5224955123415"><a name="p5224955123415"></a><a name="p5224955123415"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p20568216123415"><a name="p20568216123415"></a><a name="p20568216123415"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    </td>
    </tr>
    <tr id="row50896222123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p28953317123415"><a name="p28953317123415"></a><a name="p28953317123415"></a>routers</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p63517332123415"><a name="p63517332123415"></a><a name="p63517332123415"></a>List&lt;Router&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p44630292123415"><a name="p44630292123415"></a><a name="p44630292123415"></a>与该zone关联的Router(VPC)列表。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "id": "ff8080825b8fc86c015b94bc6f8712c3",
        "name": "example.com.",
        "description": "This is an example zone.",
        "email": "xx@example.com",
        "ttl": 300,
        "serial": 0,
        "masters": [],
        "status": "ACTIVE",
        "links": {
            "self": "https://Endpoint/v2/zones/ff8080825b8fc86c015b94bc6f8712c3"
        },
        "pool_id": "ff8080825ab738f4015ab7513298010e",
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
        "zone_type": "private",
        "created_at": "2017-04-22T08:17:08.997",
        "updated_at": "2017-04-22T08:17:09.997",
        "record_num": 2,
        "routers": [
            {
                "status": "ACTIVE",
                "router_id": "19664294-0bf6-4271-ad3a-94b8c79c6558",
                "router_region": "xx"
            },
            {
                "status": "ACTIVE",
                "router_id": "f0791650-db8c-4a20-8a44-a06c6e24b15b",
                "router_region": "xx"
            }
        ]
    }
    
    ```


## 返回值<a name="section66476022"></a>

请参考[通用请求返回值](通用请求返回值.md)。

