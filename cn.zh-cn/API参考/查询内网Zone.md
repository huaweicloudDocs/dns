# 查询内网Zone<a name="dns_api_63005"></a>

## 功能介绍<a name="section55898385"></a>

查询单个内网Zone。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=DNS&api=ShowPrivateZone)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

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
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.2.5.1.3 "><p id="p50789581"><a name="p50789581"></a><a name="p50789581"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.55%" headers="mcps1.2.5.1.4 "><p id="p20315403"><a name="p20315403"></a><a name="p20315403"></a>待查询zone的ID。</p>
<p id="p1669018482183"><a name="p1669018482183"></a><a name="p1669018482183"></a>可以通过<a href="查询内网Zone列表.md">查询内网Zone列表</a>获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section31475357"></a>

-   请求参数

    无

-   请求样例

    查询Zone ID为“ff8080825b8fc86c015b94bc6f8712c3”的域名。

    ```
    GET https://{DNS_Endpoint}/v2/zones/ff8080825b8fc86c015b94bc6f8712c3
    ```


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
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p35530101123415"><a name="p35530101123415"></a><a name="p35530101123415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p59365914123415"><a name="p59365914123415"></a><a name="p59365914123415"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="row64531184123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p59643381123415"><a name="p59643381123415"></a><a name="p59643381123415"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p66384534123415"><a name="p66384534123415"></a><a name="p66384534123415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p8438205123415"><a name="p8438205123415"></a><a name="p8438205123415"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="row8834981123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p44544845123415"><a name="p44544845123415"></a><a name="p44544845123415"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p51362669123415"><a name="p51362669123415"></a><a name="p51362669123415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p66735534123415"><a name="p66735534123415"></a><a name="p66735534123415"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="row63748898123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p63387127123415"><a name="p63387127123415"></a><a name="p63387127123415"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p34083648123415"><a name="p34083648123415"></a><a name="p34083648123415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p9312102123415"><a name="p9312102123415"></a><a name="p9312102123415"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="row16700055123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p10527186123415"><a name="p10527186123415"></a><a name="p10527186123415"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p47395742123415"><a name="p47395742123415"></a><a name="p47395742123415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p9394279212"><a name="p9394279212"></a><a name="p9394279212"></a>zone类型，公网（public）或者内网（private）。</p>
    </td>
    </tr>
    <tr id="row57540153123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p30240837123415"><a name="p30240837123415"></a><a name="p30240837123415"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p33588766123415"><a name="p33588766123415"></a><a name="p33588766123415"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p36335531123415"><a name="p36335531123415"></a><a name="p36335531123415"></a>该zone下SOA记录中的ttl值。</p>
    <p id="p0662131993410"><a name="p0662131993410"></a><a name="p0662131993410"></a>取值范围：300~2147483647</p>
    <p id="p7662111973418"><a name="p7662111973418"></a><a name="p7662111973418"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="row58584329123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p47710208123415"><a name="p47710208123415"></a><a name="p47710208123415"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p39321631123415"><a name="p39321631123415"></a><a name="p39321631123415"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p201115484116"><a name="p201115484116"></a><a name="p201115484116"></a>该zone下SOA记录中用于标识zone文件变更的序列值，用于主从节点同步。</p>
    <p id="p7524749171039"><a name="p7524749171039"></a><a name="p7524749171039"></a>该参数暂未使用。</p>
    </td>
    </tr>
    <tr id="row9984653123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p3450553123415"><a name="p3450553123415"></a><a name="p3450553123415"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p11059337123415"><a name="p11059337123415"></a><a name="p11059337123415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p23391077123415"><a name="p23391077123415"></a><a name="p23391077123415"></a>资源状态。</p>
    <p id="p186242108156"><a name="p186242108156"></a><a name="p186242108156"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="row15629110123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p57998436123415"><a name="p57998436123415"></a><a name="p57998436123415"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p252886123415"><a name="p252886123415"></a><a name="p252886123415"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p20483829123415"><a name="p20483829123415"></a><a name="p20483829123415"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="row50136736123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p34543853123415"><a name="p34543853123415"></a><a name="p34543853123415"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p46588698123415"><a name="p46588698123415"></a><a name="p46588698123415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p15588175123415"><a name="p15588175123415"></a><a name="p15588175123415"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="row6075853123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p22382050123415"><a name="p22382050123415"></a><a name="p22382050123415"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p1006739123415"><a name="p1006739123415"></a><a name="p1006739123415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p8704812171039"><a name="p8704812171039"></a><a name="p8704812171039"></a>zone所属的项目ID。</p>
    </td>
    </tr>
    <tr id="row62824730123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p55638354123415"><a name="p55638354123415"></a><a name="p55638354123415"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p10412802123415"><a name="p10412802123415"></a><a name="p10412802123415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p38130643123415"><a name="p38130643123415"></a><a name="p38130643123415"></a>创建时间。</p>
    <p id="p583516468316"><a name="p583516468316"></a><a name="p583516468316"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="row7631471123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p14169428123415"><a name="p14169428123415"></a><a name="p14169428123415"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p6873005123415"><a name="p6873005123415"></a><a name="p6873005123415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p19842531123415"><a name="p19842531123415"></a><a name="p19842531123415"></a>更新时间。</p>
    <p id="p18139194012313"><a name="p18139194012313"></a><a name="p18139194012313"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="row44365052123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p36799431123415"><a name="p36799431123415"></a><a name="p36799431123415"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p27963939123415"><a name="p27963939123415"></a><a name="p27963939123415"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p5501274116741"><a name="p5501274116741"></a><a name="p5501274116741"></a>指向当前资源或者其他资源的链接。</p>
    <p id="p50486583123415"><a name="p50486583123415"></a><a name="p50486583123415"></a>当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p1379911523453"><a name="p1379911523453"></a><a name="p1379911523453"></a>详细信息请参见<a href="#table52442344175457">表3</a>。</p>
    </td>
    </tr>
    <tr id="row51726070123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p29062162123415"><a name="p29062162123415"></a><a name="p29062162123415"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p5224955123415"><a name="p5224955123415"></a><a name="p5224955123415"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p20568216123415"><a name="p20568216123415"></a><a name="p20568216123415"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    <p id="p376119772512"><a name="p376119772512"></a><a name="p376119772512"></a>目前暂未使用。</p>
    </td>
    </tr>
    <tr id="row50896222123415"><td class="cellrowborder" valign="top" width="18.38%" headers="mcps1.2.4.1.1 "><p id="p28953317123415"><a name="p28953317123415"></a><a name="p28953317123415"></a>routers</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.4.1.2 "><p id="p63517332123415"><a name="p63517332123415"></a><a name="p63517332123415"></a>Array of object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.29%" headers="mcps1.2.4.1.3 "><p id="p44630292123415"><a name="p44630292123415"></a><a name="p44630292123415"></a>与该zone关联的Router(VPC)列表。详细信息请参见<a href="#table4448008117179">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  links参数说明

    <a name="table52442344175457"></a>
    <table><thead align="left"><tr id="row58979189175457"><th class="cellrowborder" valign="top" width="18.3018301830183%" id="mcps1.2.4.1.1"><p id="p46156243175457"><a name="p46156243175457"></a><a name="p46156243175457"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.591959195919593%" id="mcps1.2.4.1.2"><p id="p47668234175457"><a name="p47668234175457"></a><a name="p47668234175457"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.10621062106211%" id="mcps1.2.4.1.3"><p id="p35921708175457"><a name="p35921708175457"></a><a name="p35921708175457"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row54859922175457"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p14468674175457"><a name="p14468674175457"></a><a name="p14468674175457"></a>self</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.591959195919593%" headers="mcps1.2.4.1.2 "><p id="p31111955175457"><a name="p31111955175457"></a><a name="p31111955175457"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.10621062106211%" headers="mcps1.2.4.1.3 "><p id="p37040428175457"><a name="p37040428175457"></a><a name="p37040428175457"></a>当前资源的链接。</p>
    </td>
    </tr>
    <tr id="row345421154813"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.591959195919593%" headers="mcps1.2.4.1.2 "><p id="p19656144517367"><a name="p19656144517367"></a><a name="p19656144517367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.10621062106211%" headers="mcps1.2.4.1.3 "><p id="p76567451365"><a name="p76567451365"></a><a name="p76567451365"></a>下一页资源的链接。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  routers对象参数说明

    <a name="table4448008117179"></a>
    <table><thead align="left"><tr id="row6132935617179"><th class="cellrowborder" valign="top" width="18.538146185381464%" id="mcps1.2.4.1.1"><p id="p36588677171719"><a name="p36588677171719"></a><a name="p36588677171719"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.458054194580544%" id="mcps1.2.4.1.2"><p id="p9906869171719"><a name="p9906869171719"></a><a name="p9906869171719"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.003799620037995%" id="mcps1.2.4.1.3"><p id="p64258954171719"><a name="p64258954171719"></a><a name="p64258954171719"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1024510342619"><td class="cellrowborder" valign="top" width="18.538146185381464%" headers="mcps1.2.4.1.1 "><p id="p38120631175524"><a name="p38120631175524"></a><a name="p38120631175524"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.458054194580544%" headers="mcps1.2.4.1.2 "><p id="p57184665175519"><a name="p57184665175519"></a><a name="p57184665175519"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.003799620037995%" headers="mcps1.2.4.1.3 "><p id="p1635999216648"><a name="p1635999216648"></a><a name="p1635999216648"></a>资源状态。</p>
    <p id="p656495918714"><a name="p656495918714"></a><a name="p656495918714"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="row266872817179"><td class="cellrowborder" valign="top" width="18.538146185381464%" headers="mcps1.2.4.1.1 "><p id="p25118582171719"><a name="p25118582171719"></a><a name="p25118582171719"></a>router_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.458054194580544%" headers="mcps1.2.4.1.2 "><p id="p50755907171719"><a name="p50755907171719"></a><a name="p50755907171719"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.003799620037995%" headers="mcps1.2.4.1.3 "><p id="p17587794171719"><a name="p17587794171719"></a><a name="p17587794171719"></a>Router(VPC)所属VPC的ID。</p>
    <p id="p143411822947"><a name="p143411822947"></a><a name="p143411822947"></a>该参数的值可以通过如下两种方式获取：</p>
    <a name="ul1938314911411"></a><a name="ul1938314911411"></a><ul id="ul1938314911411"><li>通过虚拟私有云的管理控制台，在VPC的详情页面中获取VPC的ID。</li><li>通过<a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0003.html" target="_blank" rel="noopener noreferrer">查询VPC列表</a>获取VPC ID。</li></ul>
    </td>
    </tr>
    <tr id="row6657832817179"><td class="cellrowborder" valign="top" width="18.538146185381464%" headers="mcps1.2.4.1.1 "><p id="p3709384171719"><a name="p3709384171719"></a><a name="p3709384171719"></a>router_region</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.458054194580544%" headers="mcps1.2.4.1.2 "><p id="p43861924171719"><a name="p43861924171719"></a><a name="p43861924171719"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.003799620037995%" headers="mcps1.2.4.1.3 "><p id="p63154928171719"><a name="p63154928171719"></a><a name="p63154928171719"></a>Router(VPC)所在的region。</p>
    <p id="p38645142171939"><a name="p38645142171939"></a><a name="p38645142171939"></a>如果为空，默认为token中project所在的region。</p>
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


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

