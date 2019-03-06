# 删除Record Set<a name="ZH-CN_TOPIC_0082840631"></a>

## 功能介绍<a name="section49332166"></a>

删除单个Record Set。

## URI<a name="section41336317"></a>

DELETE  /v2.1/zones/\{zone\_id\}/recordsets/\{recordset\_id\}

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
<tbody><tr id="row51170717"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p51187411"><a name="p51187411"></a><a name="p51187411"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.24222422242224%" headers="mcps1.2.4.1.2 "><p id="p52539597"><a name="p52539597"></a><a name="p52539597"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="44.42444244424442%" headers="mcps1.2.4.1.3 "><p id="p27848947"><a name="p27848947"></a><a name="p27848947"></a>所属zone的ID。仅支持公网zone。</p>
</td>
</tr>
<tr id="row49313939"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p35006119"><a name="p35006119"></a><a name="p35006119"></a>recordset_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.24222422242224%" headers="mcps1.2.4.1.2 "><p id="p16923420"><a name="p16923420"></a><a name="p16923420"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="44.42444244424442%" headers="mcps1.2.4.1.3 "><p id="p28619802"><a name="p28619802"></a><a name="p28619802"></a>待删除recordset的ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section36482533"></a>

无

## 响应<a name="section59907344"></a>

-   参数说明

    **表 2**  响应样例的参数说明

    <a name="table2027435217127"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0082840627_row52466955175323"><th class="cellrowborder" valign="top" width="27.889999999999997%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0082840627_p2769858175323"><a name="zh-cn_topic_0082840627_p2769858175323"></a><a name="zh-cn_topic_0082840627_p2769858175323"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0082840627_p46296309175323"><a name="zh-cn_topic_0082840627_p46296309175323"></a><a name="zh-cn_topic_0082840627_p46296309175323"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.3%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0082840627_p62697904175323"><a name="zh-cn_topic_0082840627_p62697904175323"></a><a name="zh-cn_topic_0082840627_p62697904175323"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0082840627_row47909891175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p64112397175323"><a name="zh-cn_topic_0082840627_p64112397175323"></a><a name="zh-cn_topic_0082840627_p64112397175323"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p1660870175323"><a name="zh-cn_topic_0082840627_p1660870175323"></a><a name="zh-cn_topic_0082840627_p1660870175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p1249204175323"><a name="zh-cn_topic_0082840627_p1249204175323"></a><a name="zh-cn_topic_0082840627_p1249204175323"></a>Record Set的ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row6942422175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p64097412175323"><a name="zh-cn_topic_0082840627_p64097412175323"></a><a name="zh-cn_topic_0082840627_p64097412175323"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p44990515175323"><a name="zh-cn_topic_0082840627_p44990515175323"></a><a name="zh-cn_topic_0082840627_p44990515175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p32019574175323"><a name="zh-cn_topic_0082840627_p32019574175323"></a><a name="zh-cn_topic_0082840627_p32019574175323"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row61442071175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p51194416175323"><a name="zh-cn_topic_0082840627_p51194416175323"></a><a name="zh-cn_topic_0082840627_p51194416175323"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p63301991175323"><a name="zh-cn_topic_0082840627_p63301991175323"></a><a name="zh-cn_topic_0082840627_p63301991175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p43966660175323"><a name="zh-cn_topic_0082840627_p43966660175323"></a><a name="zh-cn_topic_0082840627_p43966660175323"></a>Record Set的描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row2176746175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p11805366175323"><a name="zh-cn_topic_0082840627_p11805366175323"></a><a name="zh-cn_topic_0082840627_p11805366175323"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p1051908175323"><a name="zh-cn_topic_0082840627_p1051908175323"></a><a name="zh-cn_topic_0082840627_p1051908175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p10043845175323"><a name="zh-cn_topic_0082840627_p10043845175323"></a><a name="zh-cn_topic_0082840627_p10043845175323"></a>托管该记录的zone_id。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row61212722175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p8318586175323"><a name="zh-cn_topic_0082840627_p8318586175323"></a><a name="zh-cn_topic_0082840627_p8318586175323"></a>zone_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p31287919175323"><a name="zh-cn_topic_0082840627_p31287919175323"></a><a name="zh-cn_topic_0082840627_p31287919175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p16372315175323"><a name="zh-cn_topic_0082840627_p16372315175323"></a><a name="zh-cn_topic_0082840627_p16372315175323"></a>托管该记录的zone_name。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row38132372175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p37461920175323"><a name="zh-cn_topic_0082840627_p37461920175323"></a><a name="zh-cn_topic_0082840627_p37461920175323"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p27536075175323"><a name="zh-cn_topic_0082840627_p27536075175323"></a><a name="zh-cn_topic_0082840627_p27536075175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p24813356175323"><a name="zh-cn_topic_0082840627_p24813356175323"></a><a name="zh-cn_topic_0082840627_p24813356175323"></a>记录类型。</p>
    <p id="zh-cn_topic_0082840627_p52445812175323"><a name="zh-cn_topic_0082840627_p52445812175323"></a><a name="zh-cn_topic_0082840627_p52445812175323"></a>取值范围：A，AAAA，MX，CNAME，TXT，NS（仅限公网Zone），SRV，CAA（仅限公网Zone）。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row20796819175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p4811553175323"><a name="zh-cn_topic_0082840627_p4811553175323"></a><a name="zh-cn_topic_0082840627_p4811553175323"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p47559731175323"><a name="zh-cn_topic_0082840627_p47559731175323"></a><a name="zh-cn_topic_0082840627_p47559731175323"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p22097398175323"><a name="zh-cn_topic_0082840627_p22097398175323"></a><a name="zh-cn_topic_0082840627_p22097398175323"></a>域名的缓存时间，单位为秒，缓存时间越长更新生效越慢。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row13978060175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p43388342175323"><a name="zh-cn_topic_0082840627_p43388342175323"></a><a name="zh-cn_topic_0082840627_p43388342175323"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p29596719175323"><a name="zh-cn_topic_0082840627_p29596719175323"></a><a name="zh-cn_topic_0082840627_p29596719175323"></a>List&lt;string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p30492925175323"><a name="zh-cn_topic_0082840627_p30492925175323"></a><a name="zh-cn_topic_0082840627_p30492925175323"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row23148559175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p36524189175323"><a name="zh-cn_topic_0082840627_p36524189175323"></a><a name="zh-cn_topic_0082840627_p36524189175323"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p47080972175323"><a name="zh-cn_topic_0082840627_p47080972175323"></a><a name="zh-cn_topic_0082840627_p47080972175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p15737135175323"><a name="zh-cn_topic_0082840627_p15737135175323"></a><a name="zh-cn_topic_0082840627_p15737135175323"></a>创建时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row33465792175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p42570937175323"><a name="zh-cn_topic_0082840627_p42570937175323"></a><a name="zh-cn_topic_0082840627_p42570937175323"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p27449776175323"><a name="zh-cn_topic_0082840627_p27449776175323"></a><a name="zh-cn_topic_0082840627_p27449776175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p63703533175323"><a name="zh-cn_topic_0082840627_p63703533175323"></a><a name="zh-cn_topic_0082840627_p63703533175323"></a>更新时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row17850883175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p36228271175323"><a name="zh-cn_topic_0082840627_p36228271175323"></a><a name="zh-cn_topic_0082840627_p36228271175323"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p6480061175323"><a name="zh-cn_topic_0082840627_p6480061175323"></a><a name="zh-cn_topic_0082840627_p6480061175323"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p65781854175323"><a name="zh-cn_topic_0082840627_p65781854175323"></a><a name="zh-cn_topic_0082840627_p65781854175323"></a>资源状态。</p>
    <p id="zh-cn_topic_0082840627_p51374523175323"><a name="zh-cn_topic_0082840627_p51374523175323"></a><a name="zh-cn_topic_0082840627_p51374523175323"></a>取值范围：PENDING_CREATE，ACTIVE，PENDING_DELETE，PENDING_UPDATE，ERROR，FREEZE，DISABLE。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row61184424175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p49633411175323"><a name="zh-cn_topic_0082840627_p49633411175323"></a><a name="zh-cn_topic_0082840627_p49633411175323"></a>default</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p56048766175323"><a name="zh-cn_topic_0082840627_p56048766175323"></a><a name="zh-cn_topic_0082840627_p56048766175323"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p37768157175323"><a name="zh-cn_topic_0082840627_p37768157175323"></a><a name="zh-cn_topic_0082840627_p37768157175323"></a>标识是否由系统默认生成，系统默认生成的Record Set不能删除与修改。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row15199048201026"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p23163408201026"><a name="zh-cn_topic_0082840627_p23163408201026"></a><a name="zh-cn_topic_0082840627_p23163408201026"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p40653752201026"><a name="zh-cn_topic_0082840627_p40653752201026"></a><a name="zh-cn_topic_0082840627_p40653752201026"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p4619625201026"><a name="zh-cn_topic_0082840627_p4619625201026"></a><a name="zh-cn_topic_0082840627_p4619625201026"></a>该Record Set所属的租户ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row3965248419366"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p2132803819366"><a name="zh-cn_topic_0082840627_p2132803819366"></a><a name="zh-cn_topic_0082840627_p2132803819366"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p1127763319366"><a name="zh-cn_topic_0082840627_p1127763319366"></a><a name="zh-cn_topic_0082840627_p1127763319366"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p4107308719366"><a name="zh-cn_topic_0082840627_p4107308719366"></a><a name="zh-cn_topic_0082840627_p4107308719366"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row15869402143342"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p13813035143342"><a name="zh-cn_topic_0082840627_p13813035143342"></a><a name="zh-cn_topic_0082840627_p13813035143342"></a>line</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p45114021143342"><a name="zh-cn_topic_0082840627_p45114021143342"></a><a name="zh-cn_topic_0082840627_p45114021143342"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p30357067143342"><a name="zh-cn_topic_0082840627_p30357067143342"></a><a name="zh-cn_topic_0082840627_p30357067143342"></a>解析线路。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row5250267143345"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p46748947143345"><a name="zh-cn_topic_0082840627_p46748947143345"></a><a name="zh-cn_topic_0082840627_p46748947143345"></a>weight</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p28568349143345"><a name="zh-cn_topic_0082840627_p28568349143345"></a><a name="zh-cn_topic_0082840627_p28568349143345"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p32334952143345"><a name="zh-cn_topic_0082840627_p32334952143345"></a><a name="zh-cn_topic_0082840627_p32334952143345"></a>解析记录的权重。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row2642850715221"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p6033434615221"><a name="zh-cn_topic_0082840627_p6033434615221"></a><a name="zh-cn_topic_0082840627_p6033434615221"></a>health_check_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p5524385315221"><a name="zh-cn_topic_0082840627_p5524385315221"></a><a name="zh-cn_topic_0082840627_p5524385315221"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p4556711715221"><a name="zh-cn_topic_0082840627_p4556711715221"></a><a name="zh-cn_topic_0082840627_p4556711715221"></a>健康检查ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0082840627_row67748315437"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0082840627_p1777583174312"><a name="zh-cn_topic_0082840627_p1777583174312"></a><a name="zh-cn_topic_0082840627_p1777583174312"></a>alias_target</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0082840627_p477512344313"><a name="zh-cn_topic_0082840627_p477512344313"></a><a name="zh-cn_topic_0082840627_p477512344313"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0082840627_p7775113154320"><a name="zh-cn_topic_0082840627_p7775113154320"></a><a name="zh-cn_topic_0082840627_p7775113154320"></a>别名记录。详细信息请参见<a href="创建Record-Set-0.md#table11888161342410">表4</a>。</p>
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
        "ttl": 300,
        "status": "PENDING_DELETE",
        "links": {
            "self": "https://Endpoint/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587228570158722b6ac30007"
        },
        "alias_target": null,
        "zone_id": "2c9eb155587194ec01587224c9f90149",
        "zone_name": "example.com.",
        "created_at": "2016-11-17T12:03:17.827",
        "updated_at": "2016-11-17T12:56:06.439",
        "default": false,
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
        "line": "default_view",
        "weight": 1,
        "health_check_id":null
    }
    ```


## 返回值<a name="section2295192"></a>

请参考[通用请求返回值](通用请求返回值.md)。

