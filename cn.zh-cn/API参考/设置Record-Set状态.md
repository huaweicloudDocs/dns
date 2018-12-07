# 设置Record Set状态<a name="ZH-CN_TOPIC_0083084650"></a>

## 功能介绍<a name="section49332166"></a>

设置Record Set状态。

## URI<a name="section41336317"></a>

PUT  /v2.1/recordsets/\{recordset\_id\}/statuses/set

参数说明请参见[表1](#table52104579)。

**表 1**  URI格式的参数说明

<a name="table52104579"></a>
<table><thead align="left"><tr id="row50570707"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p2586631"><a name="p2586631"></a><a name="p2586631"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="22.24222422242224%" id="mcps1.2.4.1.2"><p id="p8190559"><a name="p8190559"></a><a name="p8190559"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="44.42444244424442%" id="mcps1.2.4.1.3"><p id="p59455556"><a name="p59455556"></a><a name="p59455556"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row49313939"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p35006119"><a name="p35006119"></a><a name="p35006119"></a>recordset_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.24222422242224%" headers="mcps1.2.4.1.2 "><p id="p16923420"><a name="p16923420"></a><a name="p16923420"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="44.42444244424442%" headers="mcps1.2.4.1.3 "><p id="p28619802"><a name="p28619802"></a><a name="p28619802"></a>待设置的recordset的ID。仅支持公网zone。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section36482533"></a>

-   参数说明

    **表 2**  请求样例的参数说明

    <a name="table9470531173211"></a>
    <table><thead align="left"><tr id="row60397351173211"><th class="cellrowborder" valign="top" width="22.45%" id="mcps1.2.5.1.1"><p id="p65819295173211"><a name="p65819295173211"></a><a name="p65819295173211"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.29%" id="mcps1.2.5.1.2"><p id="p42278174173211"><a name="p42278174173211"></a><a name="p42278174173211"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.89%" id="mcps1.2.5.1.3"><p id="p26309572173211"><a name="p26309572173211"></a><a name="p26309572173211"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.37%" id="mcps1.2.5.1.4"><p id="p67071922173211"><a name="p67071922173211"></a><a name="p67071922173211"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row34337486173211"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p33154613173211"><a name="p33154613173211"></a><a name="p33154613173211"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.5.1.2 "><p id="p28540882173211"><a name="p28540882173211"></a><a name="p28540882173211"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.5.1.3 "><p id="p37402311173211"><a name="p37402311173211"></a><a name="p37402311173211"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p5093610513636"><a name="p5093610513636"></a><a name="p5093610513636"></a>解析记录状态。</p>
    <p id="p9966775173211"><a name="p9966775173211"></a><a name="p9966775173211"></a>取值范围：DISABLE、ENABLE。</p>
    <p id="p4811513713842"><a name="p4811513713842"></a><a name="p4811513713842"></a>ENABLE: 启用解析</p>
    <p id="p5801827913819"><a name="p5801827913819"></a><a name="p5801827913819"></a>DISABLE: 暂停解析</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "status": "DISABLE"
    }
    ```


## 响应<a name="section40090803161031"></a>

-   参数说明

    **表 3**  响应样例的参数说明

    <a name="table44131970191032"></a>
    <table><thead align="left"><tr id="row56209659112410"><th class="cellrowborder" valign="top" width="27.889999999999997%" id="mcps1.2.4.1.1"><p id="p56688548112410"><a name="p56688548112410"></a><a name="p56688548112410"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.2.4.1.2"><p id="p28369645112410"><a name="p28369645112410"></a><a name="p28369645112410"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.3%" id="mcps1.2.4.1.3"><p id="p16239870112410"><a name="p16239870112410"></a><a name="p16239870112410"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row40361088112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p48022682112410"><a name="p48022682112410"></a><a name="p48022682112410"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p64632053112410"><a name="p64632053112410"></a><a name="p64632053112410"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p704953112410"><a name="p704953112410"></a><a name="p704953112410"></a>Record Set的ID。</p>
    </td>
    </tr>
    <tr id="row6344577112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p44148724112410"><a name="p44148724112410"></a><a name="p44148724112410"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p19276900112410"><a name="p19276900112410"></a><a name="p19276900112410"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p17925048112410"><a name="p17925048112410"></a><a name="p17925048112410"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="row27107707112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p48240673112410"><a name="p48240673112410"></a><a name="p48240673112410"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p15180447112410"><a name="p15180447112410"></a><a name="p15180447112410"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p21656734112410"><a name="p21656734112410"></a><a name="p21656734112410"></a>Record Set的描述信息。</p>
    </td>
    </tr>
    <tr id="row60692886112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p17176696112410"><a name="p17176696112410"></a><a name="p17176696112410"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p49135151112410"><a name="p49135151112410"></a><a name="p49135151112410"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p20524323112410"><a name="p20524323112410"></a><a name="p20524323112410"></a>托管该记录的zone_id。</p>
    </td>
    </tr>
    <tr id="row50501183112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p64064024112410"><a name="p64064024112410"></a><a name="p64064024112410"></a>zone_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p21803490112410"><a name="p21803490112410"></a><a name="p21803490112410"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p21252293112410"><a name="p21252293112410"></a><a name="p21252293112410"></a>托管该记录的zone_name。</p>
    </td>
    </tr>
    <tr id="row57052911112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p57883049112410"><a name="p57883049112410"></a><a name="p57883049112410"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p58015375112410"><a name="p58015375112410"></a><a name="p58015375112410"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p1624971112410"><a name="p1624971112410"></a><a name="p1624971112410"></a>记录类型。</p>
    <p id="p14624739112410"><a name="p14624739112410"></a><a name="p14624739112410"></a>取值范围：A，AAAA，MX，CNAME，TXT，NS（仅限公网Zone），SRV，CAA（仅限公网Zone）。</p>
    </td>
    </tr>
    <tr id="row64513794112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p58234846112410"><a name="p58234846112410"></a><a name="p58234846112410"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p19402119112410"><a name="p19402119112410"></a><a name="p19402119112410"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p28067812112410"><a name="p28067812112410"></a><a name="p28067812112410"></a>域名的缓存时间，单位为秒，缓存时间越长更新生效越慢。</p>
    </td>
    </tr>
    <tr id="row51283722112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p60340817112410"><a name="p60340817112410"></a><a name="p60340817112410"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p55768000112410"><a name="p55768000112410"></a><a name="p55768000112410"></a>List&lt;string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p20914176112410"><a name="p20914176112410"></a><a name="p20914176112410"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="row54009862112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p12722690112410"><a name="p12722690112410"></a><a name="p12722690112410"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p23904930112410"><a name="p23904930112410"></a><a name="p23904930112410"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p57251150112410"><a name="p57251150112410"></a><a name="p57251150112410"></a>创建时间。</p>
    </td>
    </tr>
    <tr id="row45498309112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p61484399112410"><a name="p61484399112410"></a><a name="p61484399112410"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p14180442112410"><a name="p14180442112410"></a><a name="p14180442112410"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p7765166112410"><a name="p7765166112410"></a><a name="p7765166112410"></a>更新时间。</p>
    </td>
    </tr>
    <tr id="row2777630112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p23661473112410"><a name="p23661473112410"></a><a name="p23661473112410"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p37531169112410"><a name="p37531169112410"></a><a name="p37531169112410"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p20125829112410"><a name="p20125829112410"></a><a name="p20125829112410"></a>资源状态。</p>
    <p id="p46914736112410"><a name="p46914736112410"></a><a name="p46914736112410"></a>取值范围：ACTIVE，DISABLE。</p>
    </td>
    </tr>
    <tr id="row13988283112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p59309123112410"><a name="p59309123112410"></a><a name="p59309123112410"></a>default</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p39309635112410"><a name="p39309635112410"></a><a name="p39309635112410"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p29963876112410"><a name="p29963876112410"></a><a name="p29963876112410"></a>标识是否由系统默认生成，系统默认生成的Record Set不能删除与修改。</p>
    </td>
    </tr>
    <tr id="row1239432112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p33285181112410"><a name="p33285181112410"></a><a name="p33285181112410"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p11745126112410"><a name="p11745126112410"></a><a name="p11745126112410"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p11831148112410"><a name="p11831148112410"></a><a name="p11831148112410"></a>该Record Set所属的租户ID。</p>
    </td>
    </tr>
    <tr id="row39371469112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p34972392112410"><a name="p34972392112410"></a><a name="p34972392112410"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p14191508112410"><a name="p14191508112410"></a><a name="p14191508112410"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p8661496112410"><a name="p8661496112410"></a><a name="p8661496112410"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    </td>
    </tr>
    <tr id="row10844607112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p5997995112410"><a name="p5997995112410"></a><a name="p5997995112410"></a>line</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p16075620112410"><a name="p16075620112410"></a><a name="p16075620112410"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p27056849112410"><a name="p27056849112410"></a><a name="p27056849112410"></a>解析线路。</p>
    </td>
    </tr>
    <tr id="row42185055112410"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p61546294112410"><a name="p61546294112410"></a><a name="p61546294112410"></a>weight</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p19193909112410"><a name="p19193909112410"></a><a name="p19193909112410"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p11202821112410"><a name="p11202821112410"></a><a name="p11202821112410"></a>解析记录的权重。</p>
    </td>
    </tr>
    <tr id="row3073387153547"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="p56689514153547"><a name="p56689514153547"></a><a name="p56689514153547"></a>health_check_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="p28447961153547"><a name="p28447961153547"></a><a name="p28447961153547"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="p22583537153547"><a name="p22583537153547"></a><a name="p22583537153547"></a>健康检查ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "id": "2c9eb155587228570158722b6ac30007",
        "name": "www.example.com.",
        "description": "This is an example record set.",
        "type": "A",
        "ttl": 3600,
        "records": [
            "192.168.10.1",
            "192.168.10.2"
        ],
        "status": "DISABLE",
        "links": {
            "self": "https://Endpoint/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587228570158722b6ac30007"
        },
        "zone_id": "2c9eb155587194ec01587224c9f90149",
        "zone_name": "example.com.",
        "created_at": "2017-11-09T11:13:17.827",
        "updated_at": "2017-11-10T12:03:18.827",
        "default": false,
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
        "line": "default_view",
        "weight": 1,
        "health_check_id":null
    }
    ```


## 返回值<a name="section42637797161043"></a>

请参考[通用请求返回值](通用请求返回值.md)。

