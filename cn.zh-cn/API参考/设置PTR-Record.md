# 设置PTR Record<a name="dns_api_66002"></a>

## 功能介绍<a name="section2763065016101"></a>

设置弹性IP的PTR记录。

## URI<a name="section53701671161015"></a>

PATCH /v2/reverse/floatingips/\{region\}:\{floatingip\_id\}

参数说明请参见[表1](#table6099729418149)。

**表 1**  URI格式的参数说明

<a name="table6099729418149"></a>
<table><thead align="left"><tr id="row3442661918149"><th class="cellrowborder" valign="top" width="22.64%" id="mcps1.2.5.1.1"><p id="p3709279118149"><a name="p3709279118149"></a><a name="p3709279118149"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.37%" id="mcps1.2.5.1.2"><p id="p5172606218149"><a name="p5172606218149"></a><a name="p5172606218149"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.3"><p id="p2906151418149"><a name="p2906151418149"></a><a name="p2906151418149"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.64%" id="mcps1.2.5.1.4"><p id="p517246718149"><a name="p517246718149"></a><a name="p517246718149"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1631668818149"><td class="cellrowborder" valign="top" width="22.64%" headers="mcps1.2.5.1.1 "><p id="p4658337018149"><a name="p4658337018149"></a><a name="p4658337018149"></a>region</p>
</td>
<td class="cellrowborder" valign="top" width="17.37%" headers="mcps1.2.5.1.2 "><p id="p1515661618149"><a name="p1515661618149"></a><a name="p1515661618149"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="p1972638718149"><a name="p1972638718149"></a><a name="p1972638718149"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.64%" headers="mcps1.2.5.1.4 "><p id="p5433349018149"><a name="p5433349018149"></a><a name="p5433349018149"></a>租户的区域信息。详细内容请参见<a href="终端节点（Endpoint）.md">终端节点（Endpoint）</a>。</p>
</td>
</tr>
<tr id="row1923936518149"><td class="cellrowborder" valign="top" width="22.64%" headers="mcps1.2.5.1.1 "><p id="p1488470218149"><a name="p1488470218149"></a><a name="p1488470218149"></a>floatingip_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.37%" headers="mcps1.2.5.1.2 "><p id="p6481017518149"><a name="p6481017518149"></a><a name="p6481017518149"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="p1513281718149"><a name="p1513281718149"></a><a name="p1513281718149"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.64%" headers="mcps1.2.5.1.4 "><p id="p1779865118149"><a name="p1779865118149"></a><a name="p1779865118149"></a>弹性IP的ID。</p>
<p id="p5553155134916"><a name="p5553155134916"></a><a name="p5553155134916"></a>可以通过网络控制台的弹性公网IP页面获取或者通过<a href="https://support.huaweicloud.com/api-eip/eip_api_0003.html" target="_blank" rel="noopener noreferrer">查询弹性公网IP列表</a>获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section44958995161021"></a>

-   参数说明

    **表 2**  请求样例的参数说明

    <a name="table239794161830"></a>
    <table><thead align="left"><tr id="row654560711830"><th class="cellrowborder" valign="top" width="21.517848215178486%" id="mcps1.2.5.1.1"><p id="p3415211830"><a name="p3415211830"></a><a name="p3415211830"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.538146185381464%" id="mcps1.2.5.1.2"><p id="p276632601830"><a name="p276632601830"></a><a name="p276632601830"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.818218178182182%" id="mcps1.2.5.1.3"><p id="p261316001830"><a name="p261316001830"></a><a name="p261316001830"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="42.125787421257876%" id="mcps1.2.5.1.4"><p id="p362848191830"><a name="p362848191830"></a><a name="p362848191830"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row533892641830"><td class="cellrowborder" valign="top" width="21.517848215178486%" headers="mcps1.2.5.1.1 "><p id="p295631171830"><a name="p295631171830"></a><a name="p295631171830"></a>ptrdname</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.538146185381464%" headers="mcps1.2.5.1.2 "><p id="p458022581830"><a name="p458022581830"></a><a name="p458022581830"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.818218178182182%" headers="mcps1.2.5.1.3 "><p id="p189954321830"><a name="p189954321830"></a><a name="p189954321830"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="42.125787421257876%" headers="mcps1.2.5.1.4 "><p id="p622350301830"><a name="p622350301830"></a><a name="p622350301830"></a>PTR记录对应的域名。</p>
    <p id="p27471407151355"><a name="p27471407151355"></a><a name="p27471407151355"></a>域名格式不区分大小写，系统会将输入的大写字母统一转换为小写。</p>
    </td>
    </tr>
    <tr id="row232443661830"><td class="cellrowborder" valign="top" width="21.517848215178486%" headers="mcps1.2.5.1.1 "><p id="p37455251830"><a name="p37455251830"></a><a name="p37455251830"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.538146185381464%" headers="mcps1.2.5.1.2 "><p id="p349520711830"><a name="p349520711830"></a><a name="p349520711830"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.818218178182182%" headers="mcps1.2.5.1.3 "><p id="p125455181830"><a name="p125455181830"></a><a name="p125455181830"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="42.125787421257876%" headers="mcps1.2.5.1.4 "><p id="p95540661830"><a name="p95540661830"></a><a name="p95540661830"></a>对PTR记录的描述。</p>
    <p id="p14845539143311"><a name="p14845539143311"></a><a name="p14845539143311"></a>默认值为空。</p>
    </td>
    </tr>
    <tr id="row356818821830"><td class="cellrowborder" valign="top" width="21.517848215178486%" headers="mcps1.2.5.1.1 "><p id="p45513431830"><a name="p45513431830"></a><a name="p45513431830"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.538146185381464%" headers="mcps1.2.5.1.2 "><p id="p331144881830"><a name="p331144881830"></a><a name="p331144881830"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.818218178182182%" headers="mcps1.2.5.1.3 "><p id="p650278701830"><a name="p650278701830"></a><a name="p650278701830"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="42.125787421257876%" headers="mcps1.2.5.1.4 "><p id="p123031523174010"><a name="p123031523174010"></a><a name="p123031523174010"></a>PTR记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="p1030317233408"><a name="p1030317233408"></a><a name="p1030317233408"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    <p id="p368074541830"><a name="p368074541830"></a><a name="p368074541830"></a>取值范围：</p>
    <p id="p628316381830"><a name="p628316381830"></a><a name="p628316381830"></a>1～2147483647</p>
    <p id="p1339417482339"><a name="p1339417482339"></a><a name="p1339417482339"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="row9223123010229"><td class="cellrowborder" valign="top" width="21.517848215178486%" headers="mcps1.2.5.1.1 "><p id="p2408231966"><a name="p2408231966"></a><a name="p2408231966"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.538146185381464%" headers="mcps1.2.5.1.2 "><p id="p73741754191510"><a name="p73741754191510"></a><a name="p73741754191510"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.818218178182182%" headers="mcps1.2.5.1.3 "><p id="p43741954111519"><a name="p43741954111519"></a><a name="p43741954111519"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="42.125787421257876%" headers="mcps1.2.5.1.4 "><p id="p13997747155711"><a name="p13997747155711"></a><a name="p13997747155711"></a>反向解析关联的企业项目ID，长度不超过36个字符。</p>
    <p id="p131131925172318"><a name="p131131925172318"></a><a name="p131131925172318"></a>默认值为0。</p>
    </td>
    </tr>
    <tr id="row13969437195229"><td class="cellrowborder" valign="top" width="21.517848215178486%" headers="mcps1.2.5.1.1 "><p id="p42211177195229"><a name="p42211177195229"></a><a name="p42211177195229"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.538146185381464%" headers="mcps1.2.5.1.2 "><p id="p63662158195229"><a name="p63662158195229"></a><a name="p63662158195229"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.818218178182182%" headers="mcps1.2.5.1.3 "><p id="p56361188195229"><a name="p56361188195229"></a><a name="p56361188195229"></a>Array of object</p>
    </td>
    <td class="cellrowborder" valign="top" width="42.125787421257876%" headers="mcps1.2.5.1.4 "><p id="p1853522195229"><a name="p1853522195229"></a><a name="p1853522195229"></a>资源标签。详细信息请参见<a href="#table9752964195025">表3</a>。</p>
    <p id="p15941338343"><a name="p15941338343"></a><a name="p15941338343"></a>默认值为空。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  tags对象参数说明

    <a name="table9752964195025"></a>
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

-   请求样例

    设置PTR解析记录，对应的弹性IP的ID为“c5504932-bf23-4171-b655-b87a6bc59334”。

    ```
    PATCH https://{DNS_Endpoint}/v2/reverse/floatingips/region_id:c5504932-bf23-4171-b655-b87a6bc59334
    ```

    ```
    {
        "ptrdname": "www.example.com",
        "description": "Description for this PTR record",
        "ttl": 300,
        "tags": [ 
            { 
              "key": "key1", 
              "value": "value1" 
            } 
        ] 
    }
    ```


## 响应<a name="section40090803161031"></a>

-   参数说明

    **表 4**  响应样例的参数说明

    <a name="table6558745818456"></a>
    <table><thead align="left"><tr id="row5725206118456"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="p690539418456"><a name="p690539418456"></a><a name="p690539418456"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.189999999999998%" id="mcps1.2.4.1.2"><p id="p2246606418456"><a name="p2246606418456"></a><a name="p2246606418456"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.629999999999995%" id="mcps1.2.4.1.3"><p id="p781187018456"><a name="p781187018456"></a><a name="p781187018456"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2878170018456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p4961636318456"><a name="p4961636318456"></a><a name="p4961636318456"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="p5950245818456"><a name="p5950245818456"></a><a name="p5950245818456"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p5496981818456"><a name="p5496981818456"></a><a name="p5496981818456"></a>PTR记录的ID，格式形如{region}:{floatingip_id}。</p>
    </td>
    </tr>
    <tr id="row3274940018456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p3545576918456"><a name="p3545576918456"></a><a name="p3545576918456"></a>ptrdname</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="p5334507918456"><a name="p5334507918456"></a><a name="p5334507918456"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p2598415318456"><a name="p2598415318456"></a><a name="p2598415318456"></a>PTR记录对应的域名。</p>
    </td>
    </tr>
    <tr id="row3253079218456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p1774845918456"><a name="p1774845918456"></a><a name="p1774845918456"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="p2833911218456"><a name="p2833911218456"></a><a name="p2833911218456"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p1376672518456"><a name="p1376672518456"></a><a name="p1376672518456"></a>对PTR记录的描述。</p>
    </td>
    </tr>
    <tr id="row5679166318456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p3672198418456"><a name="p3672198418456"></a><a name="p3672198418456"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="p2169069318456"><a name="p2169069318456"></a><a name="p2169069318456"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p73714549431"><a name="p73714549431"></a><a name="p73714549431"></a>PTR记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="p1837175484310"><a name="p1837175484310"></a><a name="p1837175484310"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    <p id="p4184654118456"><a name="p4184654118456"></a><a name="p4184654118456"></a>取值范围：</p>
    <p id="p4107454918456"><a name="p4107454918456"></a><a name="p4107454918456"></a>1～2147483647。</p>
    <p id="p8320130104412"><a name="p8320130104412"></a><a name="p8320130104412"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="row3412662318456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p1279309418456"><a name="p1279309418456"></a><a name="p1279309418456"></a>address</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="p2960772218456"><a name="p2960772218456"></a><a name="p2960772218456"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p4941528218456"><a name="p4941528218456"></a><a name="p4941528218456"></a>弹性IP的IP地址。</p>
    </td>
    </tr>
    <tr id="row4208435918456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p5338995318456"><a name="p5338995318456"></a><a name="p5338995318456"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="p2961896418456"><a name="p2961896418456"></a><a name="p2961896418456"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p5032586318456"><a name="p5032586318456"></a><a name="p5032586318456"></a>资源状态。</p>
    <p id="p55966391353"><a name="p55966391353"></a><a name="p55966391353"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="row4986307418456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p1237719818456"><a name="p1237719818456"></a><a name="p1237719818456"></a>action</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="p6302897818456"><a name="p6302897818456"></a><a name="p6302897818456"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p507362318456"><a name="p507362318456"></a><a name="p507362318456"></a>对该资源的当前操作。</p>
    <p id="p13931119183618"><a name="p13931119183618"></a><a name="p13931119183618"></a>取值范围：CREATE，UPDATE，DELETE，NONE</p>
    <p id="p178601911399"><a name="p178601911399"></a><a name="p178601911399"></a>CREATE：表示创建，UPDATE：表示更新，DELETE：表示删除，NONE：表示无操作</p>
    </td>
    </tr>
    <tr id="row831034118456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p204899518456"><a name="p204899518456"></a><a name="p204899518456"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="p3175087318456"><a name="p3175087318456"></a><a name="p3175087318456"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p2168392018456"><a name="p2168392018456"></a><a name="p2168392018456"></a>指向当前资源或者其他相关资源的链接。</p>
    <p id="p6093755518456"><a name="p6093755518456"></a><a name="p6093755518456"></a>当响应需要分页时，需要包含一个next链接来进行分页。详细信息请参见<a href="#table354521744216">表5</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  links参数说明

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
    <tr id="row62371226175119"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
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
        "id": "region_id:c5504932-bf23-4171-b655-b87a6bc59334",
        "ptrdname": "www.example.com.",
        "description": "Description for this PTR record",
        "address": "10.154.52.138",
        "action": "CREATE",
        "ttl": 300,
        "status": "PENDING_CREATE",
        "links": {
            "self": "https://Endpoint/v2/reverse/floatingips/region_id:c5504932-bf23-4171-b655-b87a6bc59334"
        }
    }
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

