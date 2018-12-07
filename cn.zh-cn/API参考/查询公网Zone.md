# 查询公网Zone<a name="ZH-CN_TOPIC_0037129973"></a>

## 功能介绍<a name="section55898385"></a>

查询单个公网Zone。

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

    <a name="table54967495"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0057310891_row54125868171039"><th class="cellrowborder" valign="top" width="18.37%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0057310891_p46128019171039"><a name="zh-cn_topic_0057310891_p46128019171039"></a><a name="zh-cn_topic_0057310891_p46128019171039"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.39%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0057310891_p61288737171039"><a name="zh-cn_topic_0057310891_p61288737171039"></a><a name="zh-cn_topic_0057310891_p61288737171039"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.239999999999995%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0057310891_p39427830171039"><a name="zh-cn_topic_0057310891_p39427830171039"></a><a name="zh-cn_topic_0057310891_p39427830171039"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0057310891_row3275315171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p13677558171039"><a name="zh-cn_topic_0057310891_p13677558171039"></a><a name="zh-cn_topic_0057310891_p13677558171039"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p31480160171039"><a name="zh-cn_topic_0057310891_p31480160171039"></a><a name="zh-cn_topic_0057310891_p31480160171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p55186322171039"><a name="zh-cn_topic_0057310891_p55186322171039"></a><a name="zh-cn_topic_0057310891_p55186322171039"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row62038903171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p21725743171039"><a name="zh-cn_topic_0057310891_p21725743171039"></a><a name="zh-cn_topic_0057310891_p21725743171039"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p55078653171039"><a name="zh-cn_topic_0057310891_p55078653171039"></a><a name="zh-cn_topic_0057310891_p55078653171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p65545475171039"><a name="zh-cn_topic_0057310891_p65545475171039"></a><a name="zh-cn_topic_0057310891_p65545475171039"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row24663709171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p56112529171039"><a name="zh-cn_topic_0057310891_p56112529171039"></a><a name="zh-cn_topic_0057310891_p56112529171039"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p46656524171039"><a name="zh-cn_topic_0057310891_p46656524171039"></a><a name="zh-cn_topic_0057310891_p46656524171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p31778607171039"><a name="zh-cn_topic_0057310891_p31778607171039"></a><a name="zh-cn_topic_0057310891_p31778607171039"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row34212800171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p51657401171039"><a name="zh-cn_topic_0057310891_p51657401171039"></a><a name="zh-cn_topic_0057310891_p51657401171039"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p336297171039"><a name="zh-cn_topic_0057310891_p336297171039"></a><a name="zh-cn_topic_0057310891_p336297171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p66322352171039"><a name="zh-cn_topic_0057310891_p66322352171039"></a><a name="zh-cn_topic_0057310891_p66322352171039"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row45341886171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p22374403171039"><a name="zh-cn_topic_0057310891_p22374403171039"></a><a name="zh-cn_topic_0057310891_p22374403171039"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p16323247171039"><a name="zh-cn_topic_0057310891_p16323247171039"></a><a name="zh-cn_topic_0057310891_p16323247171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p58527202171039"><a name="zh-cn_topic_0057310891_p58527202171039"></a><a name="zh-cn_topic_0057310891_p58527202171039"></a>zone类型，公网或者内网。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row36905265171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p4888971171039"><a name="zh-cn_topic_0057310891_p4888971171039"></a><a name="zh-cn_topic_0057310891_p4888971171039"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p16027579171039"><a name="zh-cn_topic_0057310891_p16027579171039"></a><a name="zh-cn_topic_0057310891_p16027579171039"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p41240291171039"><a name="zh-cn_topic_0057310891_p41240291171039"></a><a name="zh-cn_topic_0057310891_p41240291171039"></a>该zone下SOA记录中的ttl值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row29641334171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p63311148171039"><a name="zh-cn_topic_0057310891_p63311148171039"></a><a name="zh-cn_topic_0057310891_p63311148171039"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p26678057171039"><a name="zh-cn_topic_0057310891_p26678057171039"></a><a name="zh-cn_topic_0057310891_p26678057171039"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p7524749171039"><a name="zh-cn_topic_0057310891_p7524749171039"></a><a name="zh-cn_topic_0057310891_p7524749171039"></a>该zone下SOA记录中用于标识变更的序列值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row44990376171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p30244483171039"><a name="zh-cn_topic_0057310891_p30244483171039"></a><a name="zh-cn_topic_0057310891_p30244483171039"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p47406357171039"><a name="zh-cn_topic_0057310891_p47406357171039"></a><a name="zh-cn_topic_0057310891_p47406357171039"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p9822846171039"><a name="zh-cn_topic_0057310891_p9822846171039"></a><a name="zh-cn_topic_0057310891_p9822846171039"></a>资源状态。</p>
    <p id="zh-cn_topic_0057310891_p36239781171039"><a name="zh-cn_topic_0057310891_p36239781171039"></a><a name="zh-cn_topic_0057310891_p36239781171039"></a>取值范围：PENDING_CREATE, ACTIVE, PENDING_DELETE, ERROR。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row1454557171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p51202644171039"><a name="zh-cn_topic_0057310891_p51202644171039"></a><a name="zh-cn_topic_0057310891_p51202644171039"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p32016130171039"><a name="zh-cn_topic_0057310891_p32016130171039"></a><a name="zh-cn_topic_0057310891_p32016130171039"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p53878535171039"><a name="zh-cn_topic_0057310891_p53878535171039"></a><a name="zh-cn_topic_0057310891_p53878535171039"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row48476716171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p54136527171039"><a name="zh-cn_topic_0057310891_p54136527171039"></a><a name="zh-cn_topic_0057310891_p54136527171039"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p48020249171039"><a name="zh-cn_topic_0057310891_p48020249171039"></a><a name="zh-cn_topic_0057310891_p48020249171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p63987755171039"><a name="zh-cn_topic_0057310891_p63987755171039"></a><a name="zh-cn_topic_0057310891_p63987755171039"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row49967872171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p35791512171039"><a name="zh-cn_topic_0057310891_p35791512171039"></a><a name="zh-cn_topic_0057310891_p35791512171039"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p10454086171039"><a name="zh-cn_topic_0057310891_p10454086171039"></a><a name="zh-cn_topic_0057310891_p10454086171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p8704812171039"><a name="zh-cn_topic_0057310891_p8704812171039"></a><a name="zh-cn_topic_0057310891_p8704812171039"></a>zone所属的租户ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row27690345171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p48529730171039"><a name="zh-cn_topic_0057310891_p48529730171039"></a><a name="zh-cn_topic_0057310891_p48529730171039"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p59988242171039"><a name="zh-cn_topic_0057310891_p59988242171039"></a><a name="zh-cn_topic_0057310891_p59988242171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p9292793171039"><a name="zh-cn_topic_0057310891_p9292793171039"></a><a name="zh-cn_topic_0057310891_p9292793171039"></a>创建时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row4377608115654"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p5844041115654"><a name="zh-cn_topic_0057310891_p5844041115654"></a><a name="zh-cn_topic_0057310891_p5844041115654"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p3605288915654"><a name="zh-cn_topic_0057310891_p3605288915654"></a><a name="zh-cn_topic_0057310891_p3605288915654"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p3460290715654"><a name="zh-cn_topic_0057310891_p3460290715654"></a><a name="zh-cn_topic_0057310891_p3460290715654"></a>更新时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row384676871572"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p288749251572"><a name="zh-cn_topic_0057310891_p288749251572"></a><a name="zh-cn_topic_0057310891_p288749251572"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p571676251572"><a name="zh-cn_topic_0057310891_p571676251572"></a><a name="zh-cn_topic_0057310891_p571676251572"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p660161572"><a name="zh-cn_topic_0057310891_p660161572"></a><a name="zh-cn_topic_0057310891_p660161572"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row177328815945"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057310891_p1595959815945"><a name="zh-cn_topic_0057310891_p1595959815945"></a><a name="zh-cn_topic_0057310891_p1595959815945"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057310891_p1765902715945"><a name="zh-cn_topic_0057310891_p1765902715945"></a><a name="zh-cn_topic_0057310891_p1765902715945"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057310891_p2109506015945"><a name="zh-cn_topic_0057310891_p2109506015945"></a><a name="zh-cn_topic_0057310891_p2109506015945"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "id": "2c9eb155587194ec01587224c9f90149",
        "name": "example.com.",
        "description": "This is an example zone.",
        "email": "xx@example.com",
        "ttl": 300,
        "serial": 0,
        "masters": [],
        "status": "ACTIVE",
        "links": {
            "self": "https://Endpoint/v2/zones/2c9eb155587194ec01587224c9f90149"
        },
        "pool_id": "00000000570e54ee01570e9939b20019",
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
        "zone_type": "public",
        "created_at": "2016-11-17T11:56:03.439",
        "updated_at": "2016-11-17T11:56:05.528",
        "record_num": 2
    }
    
    ```


## 返回值<a name="section66476022"></a>

请参考[通用请求返回值](通用请求返回值.md)。

