# 创建Record Set<a name="dns_api_65001"></a>

## 功能介绍<a name="section2763065016101"></a>

创建单个Record Set。

>![](public_sys-resources/icon-note.gif) **说明：** 
>仅公网域名支持创建多线路Record Set，该接口仅适用于公网DNS。

## URI<a name="section53701671161015"></a>

POST /v2.1/zones/\{zone\_id\}/recordsets

参数说明请参见[表1](#table30807893173129)。

**表 1**  URI格式的参数说明

<a name="table30807893173129"></a>
<table><thead align="left"><tr id="row38661368173129"><th class="cellrowborder" valign="top" width="21.71217121712171%" id="mcps1.2.5.1.1"><p id="p14212988173129"><a name="p14212988173129"></a><a name="p14212988173129"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.551855185518555%" id="mcps1.2.5.1.2"><p id="p23287688173129"><a name="p23287688173129"></a><a name="p23287688173129"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.88188818881888%" id="mcps1.2.5.1.3"><p id="p223780153116"><a name="p223780153116"></a><a name="p223780153116"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.85408540854086%" id="mcps1.2.5.1.4"><p id="p1114682173129"><a name="p1114682173129"></a><a name="p1114682173129"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row6301875173129"><td class="cellrowborder" valign="top" width="21.71217121712171%" headers="mcps1.2.5.1.1 "><p id="p5124116173129"><a name="p5124116173129"></a><a name="p5124116173129"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.551855185518555%" headers="mcps1.2.5.1.2 "><p id="p65804667173129"><a name="p65804667173129"></a><a name="p65804667173129"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.88188818881888%" headers="mcps1.2.5.1.3 "><p id="p82374043119"><a name="p82374043119"></a><a name="p82374043119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.85408540854086%" headers="mcps1.2.5.1.4 "><p id="p13017963195717"><a name="p13017963195717"></a><a name="p13017963195717"></a>所属zone的ID。仅支持公网zone。</p>
<p id="p22777371252"><a name="p22777371252"></a><a name="p22777371252"></a>可以通过<a href="查询公网Zone列表.md">查询公网Zone列表</a>获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section44958995161021"></a>

-   参数说明

    **表 2**  请求样例的参数说明

    <a name="table9470531173211"></a>
    <table><thead align="left"><tr id="row60397351173211"><th class="cellrowborder" valign="top" width="22.45%" id="mcps1.2.5.1.1"><p id="p65819295173211"><a name="p65819295173211"></a><a name="p65819295173211"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.57%" id="mcps1.2.5.1.2"><p id="p42278174173211"><a name="p42278174173211"></a><a name="p42278174173211"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.61%" id="mcps1.2.5.1.3"><p id="p26309572173211"><a name="p26309572173211"></a><a name="p26309572173211"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.37%" id="mcps1.2.5.1.4"><p id="p67071922173211"><a name="p67071922173211"></a><a name="p67071922173211"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row65160710173211"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p21415905173211"><a name="p21415905173211"></a><a name="p21415905173211"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.2.5.1.2 "><p id="p58188388173211"><a name="p58188388173211"></a><a name="p58188388173211"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.61%" headers="mcps1.2.5.1.3 "><p id="p45293229173211"><a name="p45293229173211"></a><a name="p45293229173211"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p5054941173211"><a name="p5054941173211"></a><a name="p5054941173211"></a>域名，后缀需以zone name结束且为FQDN（即以“.”号结束的完整主机名）。</p>
    <p id="p27471407151355"><a name="p27471407151355"></a><a name="p27471407151355"></a>域名格式不区分大小写，系统会将输入的大写字母统一转换为小写。</p>
    </td>
    </tr>
    <tr id="row34337486173211"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p33154613173211"><a name="p33154613173211"></a><a name="p33154613173211"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.2.5.1.2 "><p id="p28540882173211"><a name="p28540882173211"></a><a name="p28540882173211"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.61%" headers="mcps1.2.5.1.3 "><p id="p37402311173211"><a name="p37402311173211"></a><a name="p37402311173211"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p43441715173211"><a name="p43441715173211"></a><a name="p43441715173211"></a>可选配置，对域名的描述。</p>
    <p id="p9966775173211"><a name="p9966775173211"></a><a name="p9966775173211"></a>长度不超过255个字符。</p>
    <p id="p971275116536"><a name="p971275116536"></a><a name="p971275116536"></a>默认值为空。</p>
    </td>
    </tr>
    <tr id="row52503862173211"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p4265712173211"><a name="p4265712173211"></a><a name="p4265712173211"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.2.5.1.2 "><p id="p43588224173211"><a name="p43588224173211"></a><a name="p43588224173211"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.61%" headers="mcps1.2.5.1.3 "><p id="p44233480173211"><a name="p44233480173211"></a><a name="p44233480173211"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p29114279173211"><a name="p29114279173211"></a><a name="p29114279173211"></a>Record Set的类型。</p>
    <p id="p1579233173211"><a name="p1579233173211"></a><a name="p1579233173211"></a>取值范围：A、AAAA、MX、CNAME、TXT、NS、SRV、CAA。</p>
    <p id="p1193201604"><a name="p1193201604"></a><a name="p1193201604"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a>。</p>
    </td>
    </tr>
    <tr id="row71465392615"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p1743955511345"><a name="p1743955511345"></a><a name="p1743955511345"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.2.5.1.2 "><p id="p11439135523413"><a name="p11439135523413"></a><a name="p11439135523413"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.61%" headers="mcps1.2.5.1.3 "><p id="p64398557341"><a name="p64398557341"></a><a name="p64398557341"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p8439125518342"><a name="p8439125518342"></a><a name="p8439125518342"></a>解析记录的状态。</p>
    <p id="p17490132016386"><a name="p17490132016386"></a><a name="p17490132016386"></a>取值范围：</p>
    <a name="ul1827912763818"></a><a name="ul1827912763818"></a><ul id="ul1827912763818"><li>ENABLE，表示创建启用状态的解析记录。</li><li>DISABLE，表示创建暂停状态的解析记录。</li></ul>
    <p id="p17279153643910"><a name="p17279153643910"></a><a name="p17279153643910"></a>当参数为空时：</p>
    <a name="ul69214558499"></a><a name="ul69214558499"></a><ul id="ul69214558499"><li>若域名状态为“正常”时，默认创建的Record Set状态为“正常”。</li><li>若域名状态为“暂停”时，默认创建的Record Set状态为“暂停”。</li></ul>
    </td>
    </tr>
    <tr id="row44235645173211"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p56753577173211"><a name="p56753577173211"></a><a name="p56753577173211"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.2.5.1.2 "><p id="p44923213173211"><a name="p44923213173211"></a><a name="p44923213173211"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.61%" headers="mcps1.2.5.1.3 "><p id="p3678318721261"><a name="p3678318721261"></a><a name="p3678318721261"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p123031523174010"><a name="p123031523174010"></a><a name="p123031523174010"></a>解析记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="p1030317233408"><a name="p1030317233408"></a><a name="p1030317233408"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    <p id="p20437753173211"><a name="p20437753173211"></a><a name="p20437753173211"></a>取值范围：1~2147483647</p>
    <p id="p16101157135412"><a name="p16101157135412"></a><a name="p16101157135412"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="row59750658173211"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p62596825173211"><a name="p62596825173211"></a><a name="p62596825173211"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.2.5.1.2 "><p id="p32296167173211"><a name="p32296167173211"></a><a name="p32296167173211"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.61%" headers="mcps1.2.5.1.3 "><p id="p2089211781115"><a name="p2089211781115"></a><a name="p2089211781115"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p8321575173211"><a name="p8321575173211"></a><a name="p8321575173211"></a>解析记录的值。不同类型解析记录对应的值的规则不同。</p>
    <p id="p813988173211"><a name="p813988173211"></a><a name="p813988173211"></a>如Type为AAAA类型，Value是域名对应的IPv6地址列表。</p>
    <p id="p59053902173211"><a name="p59053902173211"></a><a name="p59053902173211"></a>具体参见《云解析服务用户指南》中“<a href="https://support.huaweicloud.com/usermanual-dns/zh-cn_topic_0035467703.html" target="_blank" rel="noopener noreferrer">管理记录集</a>”章节的说明及请求样例。</p>
    <p id="p178785222384"><a name="p178785222384"></a><a name="p178785222384"></a>别名记录时，该值不用填。</p>
    </td>
    </tr>
    <tr id="row19347487142432"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p19620443142437"><a name="p19620443142437"></a><a name="p19620443142437"></a>line</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.2.5.1.2 "><p id="p43599524142447"><a name="p43599524142447"></a><a name="p43599524142447"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.61%" headers="mcps1.2.5.1.3 "><p id="p30969417142432"><a name="p30969417142432"></a><a name="p30969417142432"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p25494838142432"><a name="p25494838142432"></a><a name="p25494838142432"></a>解析线路ID。请参见<a href="解析线路类型.md">解析线路类型</a>。</p>
    <p id="p39210194549"><a name="p39210194549"></a><a name="p39210194549"></a>默认值为默认线路。</p>
    </td>
    </tr>
    <tr id="row46318244195034"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p17706388195034"><a name="p17706388195034"></a><a name="p17706388195034"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.2.5.1.2 "><p id="p24931324195034"><a name="p24931324195034"></a><a name="p24931324195034"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.61%" headers="mcps1.2.5.1.3 "><p id="p6171377195034"><a name="p6171377195034"></a><a name="p6171377195034"></a>Array of object</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p30119514195034"><a name="p30119514195034"></a><a name="p30119514195034"></a>资源标签。详细信息请参见<a href="数据结构.md#table19530794112436">表2</a>。</p>
    <p id="p1194174212555"><a name="p1194174212555"></a><a name="p1194174212555"></a>默认值为空。</p>
    </td>
    </tr>
    <tr id="row3778990815215"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p3329183915215"><a name="p3329183915215"></a><a name="p3329183915215"></a>weight</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.2.5.1.2 "><p id="p1228445215215"><a name="p1228445215215"></a><a name="p1228445215215"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.61%" headers="mcps1.2.5.1.3 "><p id="p5551654115215"><a name="p5551654115215"></a><a name="p5551654115215"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p54597115215"><a name="p54597115215"></a><a name="p54597115215"></a>解析记录的权重。</p>
    <a name="ul2108239317221"></a><a name="ul2108239317221"></a><ul id="ul2108239317221"><li>当不填时，取默认值1。</li></ul>
    <a name="ul1341791710223"></a><a name="ul1341791710223"></a><ul id="ul1341791710223"><li>当weight=0，表示备用域名解析记录。</li><li>当weight&gt;0，表示主用域名解析记录。</li></ul>
    <p id="p11866386153334"><a name="p11866386153334"></a><a name="p11866386153334"></a>取值范围：0~100。</p>
    <p id="p370012193816"><a name="p370012193816"></a><a name="p370012193816"></a>相同名称、相同记录集类型、相同线路下的域名，权重记录集个数的上限是20。</p>
    </td>
    </tr>
    <tr id="row165518115379"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p16554113713"><a name="p16554113713"></a><a name="p16554113713"></a>alias_target</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.2.5.1.2 "><p id="p865517103714"><a name="p865517103714"></a><a name="p865517103714"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.61%" headers="mcps1.2.5.1.3 "><p id="p46551414372"><a name="p46551414372"></a><a name="p46551414372"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p365512111377"><a name="p365512111377"></a><a name="p365512111377"></a>别名记录。详细信息请参见<a href="#table374113120594">表4</a>。</p>
    <p id="p064135635410"><a name="p064135635410"></a><a name="p064135635410"></a>默认值为空。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  tags对象参数说明

    <a name="table3911153711258"></a>
    <table><thead align="left"><tr id="dns_api_62001_row15361836112436"><th class="cellrowborder" valign="top" width="24.54%" id="mcps1.2.5.1.1"><p id="dns_api_62001_p58707511112436"><a name="dns_api_62001_p58707511112436"></a><a name="dns_api_62001_p58707511112436"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.64%" id="mcps1.2.5.1.2"><p id="dns_api_62001_p791763775720"><a name="dns_api_62001_p791763775720"></a><a name="dns_api_62001_p791763775720"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.700000000000001%" id="mcps1.2.5.1.3"><p id="dns_api_62001_p42210623112436"><a name="dns_api_62001_p42210623112436"></a><a name="dns_api_62001_p42210623112436"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.12%" id="mcps1.2.5.1.4"><p id="dns_api_62001_p63617265112436"><a name="dns_api_62001_p63617265112436"></a><a name="dns_api_62001_p63617265112436"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="dns_api_62001_row35684479112436"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.5.1.1 "><p id="dns_api_62001_p13313439112530"><a name="dns_api_62001_p13313439112530"></a><a name="dns_api_62001_p13313439112530"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.64%" headers="mcps1.2.5.1.2 "><p id="dns_api_62001_p89180372570"><a name="dns_api_62001_p89180372570"></a><a name="dns_api_62001_p89180372570"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.700000000000001%" headers="mcps1.2.5.1.3 "><p id="dns_api_62001_p35653193112436"><a name="dns_api_62001_p35653193112436"></a><a name="dns_api_62001_p35653193112436"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.12%" headers="mcps1.2.5.1.4 "><p id="dns_api_62001_p48921437201850"><a name="dns_api_62001_p48921437201850"></a><a name="dns_api_62001_p48921437201850"></a>键。最大长度36个unicode字符。 key不能为空。不能包含“=”、“*”、“&lt;”、“&gt;”、“\”、“,”、“|”和“/”，且首尾字符不能为空格。</p>
    </td>
    </tr>
    <tr id="dns_api_62001_row20048002112436"><td class="cellrowborder" valign="top" width="24.54%" headers="mcps1.2.5.1.1 "><p id="dns_api_62001_p66095544112533"><a name="dns_api_62001_p66095544112533"></a><a name="dns_api_62001_p66095544112533"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.64%" headers="mcps1.2.5.1.2 "><p id="dns_api_62001_p13918103725715"><a name="dns_api_62001_p13918103725715"></a><a name="dns_api_62001_p13918103725715"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.700000000000001%" headers="mcps1.2.5.1.3 "><p id="dns_api_62001_p60123528112436"><a name="dns_api_62001_p60123528112436"></a><a name="dns_api_62001_p60123528112436"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.12%" headers="mcps1.2.5.1.4 "><p id="dns_api_62001_p61714725112922"><a name="dns_api_62001_p61714725112922"></a><a name="dns_api_62001_p61714725112922"></a>值。每个值最大长度43个unicode字符，可以为空字符串。 不能包含“=”、“*”、“&lt;”、“&gt;”、“\”、“,”、“|”和“/”，且首尾字符不能为空格。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  alias\_target对象参数说明

    <a name="table374113120594"></a>
    <table><thead align="left"><tr id="row157419105911"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p13742917592"><a name="p13742917592"></a><a name="p13742917592"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.78%" id="mcps1.2.5.1.2"><p id="p07421819595"><a name="p07421819595"></a><a name="p07421819595"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.43%" id="mcps1.2.5.1.3"><p id="p67422111597"><a name="p67422111597"></a><a name="p67422111597"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.79%" id="mcps1.2.5.1.4"><p id="p11742612599"><a name="p11742612599"></a><a name="p11742612599"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row187429115919"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p19742718598"><a name="p19742718598"></a><a name="p19742718598"></a>resource_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.78%" headers="mcps1.2.5.1.2 "><p id="p374211125916"><a name="p374211125916"></a><a name="p374211125916"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.43%" headers="mcps1.2.5.1.3 "><p id="p197423155915"><a name="p197423155915"></a><a name="p197423155915"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.79%" headers="mcps1.2.5.1.4 "><p id="p17917183417599"><a name="p17917183417599"></a><a name="p17917183417599"></a>资源服务类型，支持别名记录的服务。</p>
    <p id="p1691810346593"><a name="p1691810346593"></a><a name="p1691810346593"></a>取值：</p>
    <a name="ul59191634115910"></a><a name="ul59191634115910"></a><ul id="ul59191634115910"><li>cloudsite：云速建站</li><li>waf：Web应用防火墙</li></ul>
    </td>
    </tr>
    <tr id="row674219117592"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p10241133420012"><a name="p10241133420012"></a><a name="p10241133420012"></a>resource_domain_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.78%" headers="mcps1.2.5.1.2 "><p id="p117422135911"><a name="p117422135911"></a><a name="p117422135911"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.43%" headers="mcps1.2.5.1.3 "><p id="p2074217112599"><a name="p2074217112599"></a><a name="p2074217112599"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.79%" headers="mcps1.2.5.1.4 "><p id="p843964412591"><a name="p843964412591"></a><a name="p843964412591"></a>对应服务下的域名，由各服务提供。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    为Zone ID为“2c9eb155587194ec01587224c9f90149”的域名添加记录集。

    ```
    POST https://{DNS_Endpoint}/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets
    ```

    -   A类型

        ```
        {
            "name": "www.example.com.",
            "description": "This is an example record set.",
            "type": "A",
            "ttl": 3600,
            "records": [
                "192.168.10.1",
                "192.168.10.2"
            ],
            "line":"default_view",
            "weight":1,
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```

    -   AAAA类型

        ```
        {
            "name": "www.example.com.",
            "description": "This is an example record set.",
            "type": "AAAA",
            "ttl": 3600,
            "records": [
                "fe80:0:0:0:202:b3ff:fe1e:8329",
                "ff03:0db8:85a3:0:0:8a2e:0370:7334"
            ],
            "line":"default_view",
            "weight":1,
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```

    -   MX类型

        ```
        {
            "name": "www.example.com.",
            "description": "This is an example record set.",
            "type": "MX",
            "ttl": 3600,
            "records": [
                "1 mail.example.com"
            ],
            "line":"default_view",
            "weight":1,
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```

    -   CNAME类型

        ```
        {
            "name": "sale.example.com.",
            "description": "This is an example record set.",
            "type": "CNAME",
            "ttl": 3600,
            "records": [
                "server1.example.com"
            ],
            "line":"default_view",
            "weight":1,
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```

    -   TXT类型

        ```
        {
            "name": "server1.example.com.",
            "description": "This is an example record set.",
            "type": "TXT",
            "ttl": 300,
            "records": [
                "\"This host is used for sale.\""
            ],
            "line":"default_view",
            "weight":1,
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```

    -   NS类型

        ```
        {
            "name": "server1.example.com.",
            "description": "This is an example record set.",
            "type": "NS",
            "ttl": 300,
            "records": [
                "node1.example.com.",
                "node2.example.com."
            ],
            "line":"default_view",
            "weight": 1,
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```

    -   SRV类型

        ```
        {
            "name": "_sip._tcp.example.com.",
            "description": "This is an example record set.",
            "type": "SRV",
            "ttl": 300,
            "records": [
                "3 60 2176 sipserver.example.com.",
                "10 100 2176 sipserver.example.com."
            ],
            "line":"default_view",
            "weight":1,
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        
        ```

    -   CAA类型

        ```
        {
            "name": "www.example.com.",
            "description": "This is an example record set.",
            "type": "CAA",
            "ttl": 300,
            "records": [
                "0 issue \"example.com\"",
                "0 issuewild \"www.certinomis.com\"",
                "0 iodef \"mailto:xx@example.org\"",
                "0 iodef \"http://iodef.example.com\""
            ],
            "line":"default_view",
            "weight":1,
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```

    -   A类型（alias）

        ```
        {
            "name": "www.example.com.",
            "description": "This is an example record set.",
            "type": "A",
            "ttl": 3600,
            "alias_target": {
                         "resource_type": "cloudsite",
                         "resource_domain_name": "2018122211053616ucavdwdh.cname.ysjianzhan.cn."
                    }
        }
        ```



## 响应<a name="section40090803161031"></a>

-   参数说明

    **表 5**  响应样例的参数说明

    <a name="table7669703175323"></a>
    <table><thead align="left"><tr id="row52466955175323"><th class="cellrowborder" valign="top" width="18.33%" id="mcps1.2.4.1.1"><p id="p2769858175323"><a name="p2769858175323"></a><a name="p2769858175323"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.46%" id="mcps1.2.4.1.2"><p id="p46296309175323"><a name="p46296309175323"></a><a name="p46296309175323"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.21%" id="mcps1.2.4.1.3"><p id="p62697904175323"><a name="p62697904175323"></a><a name="p62697904175323"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row47909891175323"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p64112397175323"><a name="p64112397175323"></a><a name="p64112397175323"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p1660870175323"><a name="p1660870175323"></a><a name="p1660870175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p1249204175323"><a name="p1249204175323"></a><a name="p1249204175323"></a>Record Set的ID。</p>
    </td>
    </tr>
    <tr id="row6942422175323"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p64097412175323"><a name="p64097412175323"></a><a name="p64097412175323"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p44990515175323"><a name="p44990515175323"></a><a name="p44990515175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p32019574175323"><a name="p32019574175323"></a><a name="p32019574175323"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="row61442071175323"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p51194416175323"><a name="p51194416175323"></a><a name="p51194416175323"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p63301991175323"><a name="p63301991175323"></a><a name="p63301991175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p43966660175323"><a name="p43966660175323"></a><a name="p43966660175323"></a>Record Set的描述信息。</p>
    </td>
    </tr>
    <tr id="row2176746175323"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p11805366175323"><a name="p11805366175323"></a><a name="p11805366175323"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p1051908175323"><a name="p1051908175323"></a><a name="p1051908175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p10043845175323"><a name="p10043845175323"></a><a name="p10043845175323"></a>托管该记录的zone_id。</p>
    </td>
    </tr>
    <tr id="row61212722175323"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p8318586175323"><a name="p8318586175323"></a><a name="p8318586175323"></a>zone_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p31287919175323"><a name="p31287919175323"></a><a name="p31287919175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p16372315175323"><a name="p16372315175323"></a><a name="p16372315175323"></a>托管该记录的zone_name。</p>
    </td>
    </tr>
    <tr id="row38132372175323"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p37461920175323"><a name="p37461920175323"></a><a name="p37461920175323"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p27536075175323"><a name="p27536075175323"></a><a name="p27536075175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p24813356175323"><a name="p24813356175323"></a><a name="p24813356175323"></a>记录类型。</p>
    <p id="p52445812175323"><a name="p52445812175323"></a><a name="p52445812175323"></a>取值范围：A、AAAA、MX、CNAME、TXT、NS、SRV、CAA。</p>
    <p id="p104661629809"><a name="p104661629809"></a><a name="p104661629809"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a>。</p>
    </td>
    </tr>
    <tr id="row20796819175323"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p4811553175323"><a name="p4811553175323"></a><a name="p4811553175323"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p47559731175323"><a name="p47559731175323"></a><a name="p47559731175323"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p613657144219"><a name="p613657144219"></a><a name="p613657144219"></a>解析记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="p1913617716427"><a name="p1913617716427"></a><a name="p1913617716427"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    </td>
    </tr>
    <tr id="row13978060175323"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p43388342175323"><a name="p43388342175323"></a><a name="p43388342175323"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p29596719175323"><a name="p29596719175323"></a><a name="p29596719175323"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p30492925175323"><a name="p30492925175323"></a><a name="p30492925175323"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="row23148559175323"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p36524189175323"><a name="p36524189175323"></a><a name="p36524189175323"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p47080972175323"><a name="p47080972175323"></a><a name="p47080972175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p15737135175323"><a name="p15737135175323"></a><a name="p15737135175323"></a>创建时间。</p>
    <p id="p583516468316"><a name="p583516468316"></a><a name="p583516468316"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="row33465792175323"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p42570937175323"><a name="p42570937175323"></a><a name="p42570937175323"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p27449776175323"><a name="p27449776175323"></a><a name="p27449776175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p63703533175323"><a name="p63703533175323"></a><a name="p63703533175323"></a>更新时间。</p>
    <p id="p1418163015915"><a name="p1418163015915"></a><a name="p1418163015915"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="row17850883175323"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p36228271175323"><a name="p36228271175323"></a><a name="p36228271175323"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p6480061175323"><a name="p6480061175323"></a><a name="p6480061175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p65781854175323"><a name="p65781854175323"></a><a name="p65781854175323"></a>资源状态。</p>
    <p id="p1252325325910"><a name="p1252325325910"></a><a name="p1252325325910"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="row61184424175323"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p49633411175323"><a name="p49633411175323"></a><a name="p49633411175323"></a>default</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p56048766175323"><a name="p56048766175323"></a><a name="p56048766175323"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p37768157175323"><a name="p37768157175323"></a><a name="p37768157175323"></a>标识是否由系统默认生成，系统默认生成的Record Set不能删除。</p>
    </td>
    </tr>
    <tr id="row15199048201026"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p23163408201026"><a name="p23163408201026"></a><a name="p23163408201026"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p40653752201026"><a name="p40653752201026"></a><a name="p40653752201026"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p4619625201026"><a name="p4619625201026"></a><a name="p4619625201026"></a>该Record Set所属的项目ID。</p>
    </td>
    </tr>
    <tr id="row3965248419366"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p2132803819366"><a name="p2132803819366"></a><a name="p2132803819366"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p1127763319366"><a name="p1127763319366"></a><a name="p1127763319366"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p4107308719366"><a name="p4107308719366"></a><a name="p4107308719366"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。详细信息请参见<a href="#table354521744216">表6</a>。</p>
    </td>
    </tr>
    <tr id="row15869402143342"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p13813035143342"><a name="p13813035143342"></a><a name="p13813035143342"></a>line</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p45114021143342"><a name="p45114021143342"></a><a name="p45114021143342"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p30357067143342"><a name="p30357067143342"></a><a name="p30357067143342"></a>解析线路ID。</p>
    </td>
    </tr>
    <tr id="row5250267143345"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p46748947143345"><a name="p46748947143345"></a><a name="p46748947143345"></a>weight</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p28568349143345"><a name="p28568349143345"></a><a name="p28568349143345"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p32334952143345"><a name="p32334952143345"></a><a name="p32334952143345"></a>解析记录的权重。</p>
    </td>
    </tr>
    <tr id="row2642850715221"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p6033434615221"><a name="p6033434615221"></a><a name="p6033434615221"></a>health_check_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p5524385315221"><a name="p5524385315221"></a><a name="p5524385315221"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p4556711715221"><a name="p4556711715221"></a><a name="p4556711715221"></a>健康检查ID。</p>
    </td>
    </tr>
    <tr id="row67748315437"><td class="cellrowborder" valign="top" width="18.33%" headers="mcps1.2.4.1.1 "><p id="p1777583174312"><a name="p1777583174312"></a><a name="p1777583174312"></a>alias_target</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p477512344313"><a name="p477512344313"></a><a name="p477512344313"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.21%" headers="mcps1.2.4.1.3 "><p id="p7775113154320"><a name="p7775113154320"></a><a name="p7775113154320"></a>别名记录。详细信息请参见<a href="数据结构.md#table11888161342410">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  links参数说明

    <a name="table354521744216"></a>
    <table><thead align="left"><tr id="row954518179427"><th class="cellrowborder" valign="top" width="18.3018301830183%" id="mcps1.2.4.1.1"><p id="p654513173424"><a name="p654513173424"></a><a name="p654513173424"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.591959195919593%" id="mcps1.2.4.1.2"><p id="p654551714212"><a name="p654551714212"></a><a name="p654551714212"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.10621062106211%" id="mcps1.2.4.1.3"><p id="p1545141717427"><a name="p1545141717427"></a><a name="p1545141717427"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3545101710429"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p115467171428"><a name="p115467171428"></a><a name="p115467171428"></a>self</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.591959195919593%" headers="mcps1.2.4.1.2 "><p id="p254611713427"><a name="p254611713427"></a><a name="p254611713427"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.10621062106211%" headers="mcps1.2.4.1.3 "><p id="p5546171744214"><a name="p5546171744214"></a><a name="p5546171744214"></a>当前资源的链接。</p>
    </td>
    </tr>
    <tr id="row4823101010506"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.591959195919593%" headers="mcps1.2.4.1.2 "><p id="p19656144517367"><a name="p19656144517367"></a><a name="p19656144517367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.10621062106211%" headers="mcps1.2.4.1.3 "><p id="p76567451365"><a name="p76567451365"></a><a name="p76567451365"></a>下一页资源的链接。</p>
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
        "records": [
            "192.168.10.1",
            "192.168.10.2"
        ],
        "status": "PENDING_CREATE",
        "links": {
            "self": "https://Endpoint/v2.1/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587228570158722b6ac30007"
        },
        "zone_id": "2c9eb155587194ec01587224c9f90149",
        "zone_name": "example.com.",
        "created_at": "2016-11-17T12:03:17.827",
        "updated_at": null,
        "default": false,
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
        "line": "default_view",
        "weight": 1,
        "health_check_id":null
    }
    
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

