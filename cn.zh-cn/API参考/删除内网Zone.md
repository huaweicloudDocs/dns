# 删除内网Zone<a name="ZH-CN_TOPIC_0057311030"></a>

## 功能介绍<a name="section2763065016101"></a>

删除单个内网Zone。

## URI<a name="section53701671161015"></a>

DELETE /v2/zones/\{zone\_id\}

参数说明请参见[表1](#table56746773172616)。

**表 1**  URI格式的参数说明

<a name="table56746773172616"></a>
<table><thead align="left"><tr id="row12848229172616"><th class="cellrowborder" valign="top" width="15.459999999999999%" id="mcps1.2.5.1.1"><p id="p44975878172616"><a name="p44975878172616"></a><a name="p44975878172616"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.459999999999999%" id="mcps1.2.5.1.2"><p id="p46443918172616"><a name="p46443918172616"></a><a name="p46443918172616"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.53%" id="mcps1.2.5.1.3"><p id="p1368350172616"><a name="p1368350172616"></a><a name="p1368350172616"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.55%" id="mcps1.2.5.1.4"><p id="p24157908172616"><a name="p24157908172616"></a><a name="p24157908172616"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row39993297172616"><td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.5.1.1 "><p id="p43071797172616"><a name="p43071797172616"></a><a name="p43071797172616"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.5.1.2 "><p id="p26647585172616"><a name="p26647585172616"></a><a name="p26647585172616"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.2.5.1.3 "><p id="p21075379172616"><a name="p21075379172616"></a><a name="p21075379172616"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="51.55%" headers="mcps1.2.5.1.4 "><p id="p4976396172616"><a name="p4976396172616"></a><a name="p4976396172616"></a>待删除zone的ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section44958995161021"></a>

无

## 响应<a name="section40090803161031"></a>

-   要素说明

    **表 2**  响应样例的要素说明

    <a name="table28510837181412"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0057311028_row29441359123415"><th class="cellrowborder" valign="top" width="18.38%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0057311028_p35939865123415"><a name="zh-cn_topic_0057311028_p35939865123415"></a><a name="zh-cn_topic_0057311028_p35939865123415"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.33%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0057311028_p25447972123415"><a name="zh-cn_topic_0057311028_p25447972123415"></a><a name="zh-cn_topic_0057311028_p25447972123415"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.29%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0057311028_p48019864123415"><a name="zh-cn_topic_0057311028_p48019864123415"></a><a name="zh-cn_topic_0057311028_p48019864123415"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0057311028_row64403739123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p49320408123415"><a name="zh-cn_topic_0057311028_p49320408123415"></a><a name="zh-cn_topic_0057311028_p49320408123415"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p35530101123415"><a name="zh-cn_topic_0057311028_p35530101123415"></a><a name="zh-cn_topic_0057311028_p35530101123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p59365914123415"><a name="zh-cn_topic_0057311028_p59365914123415"></a><a name="zh-cn_topic_0057311028_p59365914123415"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row64531184123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p59643381123415"><a name="zh-cn_topic_0057311028_p59643381123415"></a><a name="zh-cn_topic_0057311028_p59643381123415"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p66384534123415"><a name="zh-cn_topic_0057311028_p66384534123415"></a><a name="zh-cn_topic_0057311028_p66384534123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p8438205123415"><a name="zh-cn_topic_0057311028_p8438205123415"></a><a name="zh-cn_topic_0057311028_p8438205123415"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row8834981123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p44544845123415"><a name="zh-cn_topic_0057311028_p44544845123415"></a><a name="zh-cn_topic_0057311028_p44544845123415"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p51362669123415"><a name="zh-cn_topic_0057311028_p51362669123415"></a><a name="zh-cn_topic_0057311028_p51362669123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p66735534123415"><a name="zh-cn_topic_0057311028_p66735534123415"></a><a name="zh-cn_topic_0057311028_p66735534123415"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row63748898123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p63387127123415"><a name="zh-cn_topic_0057311028_p63387127123415"></a><a name="zh-cn_topic_0057311028_p63387127123415"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p34083648123415"><a name="zh-cn_topic_0057311028_p34083648123415"></a><a name="zh-cn_topic_0057311028_p34083648123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p9312102123415"><a name="zh-cn_topic_0057311028_p9312102123415"></a><a name="zh-cn_topic_0057311028_p9312102123415"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row16700055123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p10527186123415"><a name="zh-cn_topic_0057311028_p10527186123415"></a><a name="zh-cn_topic_0057311028_p10527186123415"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p47395742123415"><a name="zh-cn_topic_0057311028_p47395742123415"></a><a name="zh-cn_topic_0057311028_p47395742123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p13849890123415"><a name="zh-cn_topic_0057311028_p13849890123415"></a><a name="zh-cn_topic_0057311028_p13849890123415"></a>zone类型，公网或者内网。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row57540153123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p30240837123415"><a name="zh-cn_topic_0057311028_p30240837123415"></a><a name="zh-cn_topic_0057311028_p30240837123415"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p33588766123415"><a name="zh-cn_topic_0057311028_p33588766123415"></a><a name="zh-cn_topic_0057311028_p33588766123415"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p36335531123415"><a name="zh-cn_topic_0057311028_p36335531123415"></a><a name="zh-cn_topic_0057311028_p36335531123415"></a>该zone下SOA记录中的ttl值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row58584329123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p47710208123415"><a name="zh-cn_topic_0057311028_p47710208123415"></a><a name="zh-cn_topic_0057311028_p47710208123415"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p39321631123415"><a name="zh-cn_topic_0057311028_p39321631123415"></a><a name="zh-cn_topic_0057311028_p39321631123415"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p30935567123415"><a name="zh-cn_topic_0057311028_p30935567123415"></a><a name="zh-cn_topic_0057311028_p30935567123415"></a>该zone下SOA记录中用于标识变更的序列值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row9984653123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p3450553123415"><a name="zh-cn_topic_0057311028_p3450553123415"></a><a name="zh-cn_topic_0057311028_p3450553123415"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p11059337123415"><a name="zh-cn_topic_0057311028_p11059337123415"></a><a name="zh-cn_topic_0057311028_p11059337123415"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p23391077123415"><a name="zh-cn_topic_0057311028_p23391077123415"></a><a name="zh-cn_topic_0057311028_p23391077123415"></a>资源状态。</p>
    <p id="zh-cn_topic_0057311028_p9193108123415"><a name="zh-cn_topic_0057311028_p9193108123415"></a><a name="zh-cn_topic_0057311028_p9193108123415"></a>取值范围：PENDING_CREATE, ACTIVE, PENDING_DELETE, ERROR。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row15629110123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p57998436123415"><a name="zh-cn_topic_0057311028_p57998436123415"></a><a name="zh-cn_topic_0057311028_p57998436123415"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p252886123415"><a name="zh-cn_topic_0057311028_p252886123415"></a><a name="zh-cn_topic_0057311028_p252886123415"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p20483829123415"><a name="zh-cn_topic_0057311028_p20483829123415"></a><a name="zh-cn_topic_0057311028_p20483829123415"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row50136736123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p34543853123415"><a name="zh-cn_topic_0057311028_p34543853123415"></a><a name="zh-cn_topic_0057311028_p34543853123415"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p46588698123415"><a name="zh-cn_topic_0057311028_p46588698123415"></a><a name="zh-cn_topic_0057311028_p46588698123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p15588175123415"><a name="zh-cn_topic_0057311028_p15588175123415"></a><a name="zh-cn_topic_0057311028_p15588175123415"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row6075853123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p22382050123415"><a name="zh-cn_topic_0057311028_p22382050123415"></a><a name="zh-cn_topic_0057311028_p22382050123415"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p1006739123415"><a name="zh-cn_topic_0057311028_p1006739123415"></a><a name="zh-cn_topic_0057311028_p1006739123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p14437066123415"><a name="zh-cn_topic_0057311028_p14437066123415"></a><a name="zh-cn_topic_0057311028_p14437066123415"></a>zone所属的租户ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row62824730123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p55638354123415"><a name="zh-cn_topic_0057311028_p55638354123415"></a><a name="zh-cn_topic_0057311028_p55638354123415"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p10412802123415"><a name="zh-cn_topic_0057311028_p10412802123415"></a><a name="zh-cn_topic_0057311028_p10412802123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p38130643123415"><a name="zh-cn_topic_0057311028_p38130643123415"></a><a name="zh-cn_topic_0057311028_p38130643123415"></a>创建时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row7631471123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p14169428123415"><a name="zh-cn_topic_0057311028_p14169428123415"></a><a name="zh-cn_topic_0057311028_p14169428123415"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p6873005123415"><a name="zh-cn_topic_0057311028_p6873005123415"></a><a name="zh-cn_topic_0057311028_p6873005123415"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p19842531123415"><a name="zh-cn_topic_0057311028_p19842531123415"></a><a name="zh-cn_topic_0057311028_p19842531123415"></a>更新时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row44365052123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p36799431123415"><a name="zh-cn_topic_0057311028_p36799431123415"></a><a name="zh-cn_topic_0057311028_p36799431123415"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p27963939123415"><a name="zh-cn_topic_0057311028_p27963939123415"></a><a name="zh-cn_topic_0057311028_p27963939123415"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p5501274116741"><a name="zh-cn_topic_0057311028_p5501274116741"></a><a name="zh-cn_topic_0057311028_p5501274116741"></a>指向当前资源或者其他资源的链接。</p>
    <p id="zh-cn_topic_0057311028_p50486583123415"><a name="zh-cn_topic_0057311028_p50486583123415"></a><a name="zh-cn_topic_0057311028_p50486583123415"></a>当查询需要分页时，需要包含一个next链接指向下一页。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row51726070123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p29062162123415"><a name="zh-cn_topic_0057311028_p29062162123415"></a><a name="zh-cn_topic_0057311028_p29062162123415"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p5224955123415"><a name="zh-cn_topic_0057311028_p5224955123415"></a><a name="zh-cn_topic_0057311028_p5224955123415"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p20568216123415"><a name="zh-cn_topic_0057311028_p20568216123415"></a><a name="zh-cn_topic_0057311028_p20568216123415"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311028_row50896222123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311028_p28953317123415"><a name="zh-cn_topic_0057311028_p28953317123415"></a><a name="zh-cn_topic_0057311028_p28953317123415"></a>routers</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311028_p63517332123415"><a name="zh-cn_topic_0057311028_p63517332123415"></a><a name="zh-cn_topic_0057311028_p63517332123415"></a>List&lt;Router&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311028_p44630292123415"><a name="zh-cn_topic_0057311028_p44630292123415"></a><a name="zh-cn_topic_0057311028_p44630292123415"></a>与该zone关联的Router(VPC)列表。</p>
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
        "serial": 1,
        "masters": [],
        "status": "PENDING_DELETE",
        "links": {
            "self": "https://Endpoint/v2/zones/ff8080825b8fc86c015b94bc6f8712c3"
        },
        "pool_id": "ff8080825ab738f4015ab7513298010e",
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
        "zone_type": "private",
        "created_at": "2017-04-22T10:05:23.110",
        "updated_at": "2017-04-22T10:05:23.959",
        "record_num": 0,
        "routers": [
            {
                "status": "PENDING_DELETE",
                "router_id": "19664294-0bf6-4271-ad3a-94b8c79c6558",
                "router_region": "xx"
            },
            {
                "status": "PENDING_DELETE",
                "router_id": "f0791650-db8c-4a20-8a44-a06c6e24b15b",
                "router_region": "xx"
            }
        ]
    }
    ```


## 返回值<a name="section42637797161043"></a>

请参考[通用请求返回值](通用请求返回值.md)。

