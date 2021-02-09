# 创建内网Zone<a name="dns_api_63002"></a>

## 功能介绍<a name="section3569153217343"></a>

创建单个内网Zone。

## URI<a name="section6163262617350"></a>

POST /v2/zones

## 请求<a name="section4207148117353"></a>

-   参数说明

    **表 1**  请求样例的参数说明

    <a name="table3720408817742"></a>
    <table><thead align="left"><tr id="row6225671717742"><th class="cellrowborder" valign="top" width="23.45%" id="mcps1.2.5.1.1"><p id="p5153686617742"><a name="p5153686617742"></a><a name="p5153686617742"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.05%" id="mcps1.2.5.1.2"><p id="p473035017742"><a name="p473035017742"></a><a name="p473035017742"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.66%" id="mcps1.2.5.1.3"><p id="p386753717742"><a name="p386753717742"></a><a name="p386753717742"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="45.839999999999996%" id="mcps1.2.5.1.4"><p id="p5956810717742"><a name="p5956810717742"></a><a name="p5956810717742"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1329410717742"><td class="cellrowborder" valign="top" width="23.45%" headers="mcps1.2.5.1.1 "><p id="p3414560317742"><a name="p3414560317742"></a><a name="p3414560317742"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.05%" headers="mcps1.2.5.1.2 "><p id="p6603174617742"><a name="p6603174617742"></a><a name="p6603174617742"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.66%" headers="mcps1.2.5.1.3 "><p id="p360216817742"><a name="p360216817742"></a><a name="p360216817742"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.4 "><p id="p2651334817742"><a name="p2651334817742"></a><a name="p2651334817742"></a>待创建的域名。</p>
    <a name="ul1536534155329"></a><a name="ul1536534155329"></a><ul id="ul1536534155329"><li>若以“.”号结束，总长度不超过254个字符。</li><li>若以非“.”号结束，总长度不超过253个字符。</li><li>单个字符串不超过63个字符，字符串间以点号分割。</li></ul>
    <p id="p61100872151329"><a name="p61100872151329"></a><a name="p61100872151329"></a>域名格式不区分大小写，系统会将输入的大写字母统一转换为小写。</p>
    </td>
    </tr>
    <tr id="row1973909717742"><td class="cellrowborder" valign="top" width="23.45%" headers="mcps1.2.5.1.1 "><p id="p5474826717742"><a name="p5474826717742"></a><a name="p5474826717742"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.05%" headers="mcps1.2.5.1.2 "><p id="p759162017742"><a name="p759162017742"></a><a name="p759162017742"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.66%" headers="mcps1.2.5.1.3 "><p id="p3220634117742"><a name="p3220634117742"></a><a name="p3220634117742"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.4 "><p id="p44313881155342"><a name="p44313881155342"></a><a name="p44313881155342"></a>域名的描述信息。</p>
    <p id="p6675950017742"><a name="p6675950017742"></a><a name="p6675950017742"></a>长度不超过255个字符。</p>
    <p id="p10578150184319"><a name="p10578150184319"></a><a name="p10578150184319"></a>默认值为空。</p>
    </td>
    </tr>
    <tr id="row3526956217742"><td class="cellrowborder" valign="top" width="23.45%" headers="mcps1.2.5.1.1 "><p id="p5656791917742"><a name="p5656791917742"></a><a name="p5656791917742"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.05%" headers="mcps1.2.5.1.2 "><p id="p2306625217742"><a name="p2306625217742"></a><a name="p2306625217742"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.66%" headers="mcps1.2.5.1.3 "><p id="p5927915117742"><a name="p5927915117742"></a><a name="p5927915117742"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.4 "><p id="p92377632066"><a name="p92377632066"></a><a name="p92377632066"></a>域名类型。</p>
    <p id="p100613092066"><a name="p100613092066"></a><a name="p100613092066"></a>内网域名：域名仅被具体VPC内的主机访问。</p>
    <p id="p2001526020713"><a name="p2001526020713"></a><a name="p2001526020713"></a>取值：private。</p>
    <p id="p96596832066"><a name="p96596832066"></a><a name="p96596832066"></a>创建公网域名，请参见<a href="创建公网Zone.md">创建公网Zone</a>。</p>
    </td>
    </tr>
    <tr id="row4358988017742"><td class="cellrowborder" valign="top" width="23.45%" headers="mcps1.2.5.1.1 "><p id="p6536976617742"><a name="p6536976617742"></a><a name="p6536976617742"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.05%" headers="mcps1.2.5.1.2 "><p id="p650279617742"><a name="p650279617742"></a><a name="p650279617742"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.66%" headers="mcps1.2.5.1.3 "><p id="p2054573717742"><a name="p2054573717742"></a><a name="p2054573717742"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.4 "><p id="p1997196517742"><a name="p1997196517742"></a><a name="p1997196517742"></a>管理该zone的管理员邮箱。</p>
    <p id="p1609108834"><a name="p1609108834"></a><a name="p1609108834"></a>默认值为售后服务邮箱。</p>
    </td>
    </tr>
    <tr id="row13489593141045"><td class="cellrowborder" valign="top" width="23.45%" headers="mcps1.2.5.1.1 "><p id="p18915273141045"><a name="p18915273141045"></a><a name="p18915273141045"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.05%" headers="mcps1.2.5.1.2 "><p id="p55742162141045"><a name="p55742162141045"></a><a name="p55742162141045"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.66%" headers="mcps1.2.5.1.3 "><p id="p18821243141045"><a name="p18821243141045"></a><a name="p18821243141045"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.4 "><p id="p3447255141334"><a name="p3447255141334"></a><a name="p3447255141334"></a>用于填写默认生成的SOA记录中有效缓存时间，以秒为单位。</p>
    <p id="p5335091141210"><a name="p5335091141210"></a><a name="p5335091141210"></a>取值范围：1~2147483647</p>
    <p id="p977916161437"><a name="p977916161437"></a><a name="p977916161437"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="row18045881171648"><td class="cellrowborder" valign="top" width="23.45%" headers="mcps1.2.5.1.1 "><p id="p20204595171650"><a name="p20204595171650"></a><a name="p20204595171650"></a>router</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.05%" headers="mcps1.2.5.1.2 "><p id="p25959495171650"><a name="p25959495171650"></a><a name="p25959495171650"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.66%" headers="mcps1.2.5.1.3 "><p id="p22344380171650"><a name="p22344380171650"></a><a name="p22344380171650"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.4 "><p id="p65064378171650"><a name="p65064378171650"></a><a name="p65064378171650"></a>Private zone关联的Router(VPC)信息，详细信息请参见<a href="#table4448008117179">表2</a>。</p>
    </td>
    </tr>
    <tr id="row3748545412107"><td class="cellrowborder" valign="top" width="23.45%" headers="mcps1.2.5.1.1 "><p id="p6123289312107"><a name="p6123289312107"></a><a name="p6123289312107"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.05%" headers="mcps1.2.5.1.2 "><p id="p6091732812107"><a name="p6091732812107"></a><a name="p6091732812107"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.66%" headers="mcps1.2.5.1.3 "><p id="p3535651512107"><a name="p3535651512107"></a><a name="p3535651512107"></a>Array of object</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.4 "><p id="p4530543812107"><a name="p4530543812107"></a><a name="p4530543812107"></a>资源标签。详细信息请参见<a href="#table58807309208">表3</a>。</p>
    <p id="p39666299312"><a name="p39666299312"></a><a name="p39666299312"></a>默认值为空。</p>
    </td>
    </tr>
    <tr id="row11374354121511"><td class="cellrowborder" valign="top" width="23.45%" headers="mcps1.2.5.1.1 "><p id="p2408231966"><a name="p2408231966"></a><a name="p2408231966"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.05%" headers="mcps1.2.5.1.2 "><p id="p73741754191510"><a name="p73741754191510"></a><a name="p73741754191510"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.66%" headers="mcps1.2.5.1.3 "><p id="p43741954111519"><a name="p43741954111519"></a><a name="p43741954111519"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.839999999999996%" headers="mcps1.2.5.1.4 "><p id="p13997747155711"><a name="p13997747155711"></a><a name="p13997747155711"></a>域名关联的企业项目ID，长度不超过36个字符。</p>
    <p id="p131131925172318"><a name="p131131925172318"></a><a name="p131131925172318"></a>默认值为0。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  router对象参数说明

    <a name="table4448008117179"></a>
    <table><thead align="left"><tr id="row6132935617179"><th class="cellrowborder" valign="top" width="23.59%" id="mcps1.2.5.1.1"><p id="p36588677171719"><a name="p36588677171719"></a><a name="p36588677171719"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.24%" id="mcps1.2.5.1.2"><p id="p06011644121012"><a name="p06011644121012"></a><a name="p06011644121012"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.21%" id="mcps1.2.5.1.3"><p id="p9906869171719"><a name="p9906869171719"></a><a name="p9906869171719"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="45.96%" id="mcps1.2.5.1.4"><p id="p64258954171719"><a name="p64258954171719"></a><a name="p64258954171719"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row266872817179"><td class="cellrowborder" valign="top" width="23.59%" headers="mcps1.2.5.1.1 "><p id="p25118582171719"><a name="p25118582171719"></a><a name="p25118582171719"></a>router_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.24%" headers="mcps1.2.5.1.2 "><p id="p11602144151017"><a name="p11602144151017"></a><a name="p11602144151017"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.21%" headers="mcps1.2.5.1.3 "><p id="p50755907171719"><a name="p50755907171719"></a><a name="p50755907171719"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.96%" headers="mcps1.2.5.1.4 "><p id="p17587794171719"><a name="p17587794171719"></a><a name="p17587794171719"></a>Router(VPC)所属VPC的ID。</p>
    <p id="p143411822947"><a name="p143411822947"></a><a name="p143411822947"></a>该参数的值可以通过如下两种方式获取：</p>
    <a name="ul1938314911411"></a><a name="ul1938314911411"></a><ul id="ul1938314911411"><li>通过虚拟私有云的管理控制台，在VPC的详情页面中获取VPC的ID。</li><li>通过<a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0003.html" target="_blank" rel="noopener noreferrer">查询VPC列表</a>获取VPC ID。</li></ul>
    </td>
    </tr>
    <tr id="row6657832817179"><td class="cellrowborder" valign="top" width="23.59%" headers="mcps1.2.5.1.1 "><p id="p3709384171719"><a name="p3709384171719"></a><a name="p3709384171719"></a>router_region</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.24%" headers="mcps1.2.5.1.2 "><p id="p8602134413102"><a name="p8602134413102"></a><a name="p8602134413102"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.21%" headers="mcps1.2.5.1.3 "><p id="p43861924171719"><a name="p43861924171719"></a><a name="p43861924171719"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.96%" headers="mcps1.2.5.1.4 "><p id="p63154928171719"><a name="p63154928171719"></a><a name="p63154928171719"></a>Router(VPC)所在的region。</p>
    <p id="p38645142171939"><a name="p38645142171939"></a><a name="p38645142171939"></a>如果为空，默认为token中project所在的region。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  tags对象参数说明

    <a name="table58807309208"></a>
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

    创建一个内网域名，域名为“example.com”。

    ```
    POST https://{DNS_Endpoint}/v2/zones
    ```

    ```
    {
        "name": "example.com.",
        "description": "This is an example zone.",
        "zone_type": "private",
        "email": "xx@example.org",
        "router": {
            "router_id": "19664294-0bf6-4271-ad3a-94b8c79c6558",
            "router_region": "xx"
        },
        "tags": [
            {
              "key": "key1",
              "value": "value1"
            }
        ]
    }
    ```


## 响应<a name="section2142173017358"></a>

-   要素说明

    **表 4**  响应样例的要素说明

    <a name="table54601120171039"></a>
    <table><thead align="left"><tr id="row54125868171039"><th class="cellrowborder" valign="top" width="18.37%" id="mcps1.2.4.1.1"><p id="p46128019171039"><a name="p46128019171039"></a><a name="p46128019171039"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.39%" id="mcps1.2.4.1.2"><p id="p61288737171039"><a name="p61288737171039"></a><a name="p61288737171039"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.239999999999995%" id="mcps1.2.4.1.3"><p id="p39427830171039"><a name="p39427830171039"></a><a name="p39427830171039"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3275315171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p13677558171039"><a name="p13677558171039"></a><a name="p13677558171039"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p31480160171039"><a name="p31480160171039"></a><a name="p31480160171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p55186322171039"><a name="p55186322171039"></a><a name="p55186322171039"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="row62038903171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p21725743171039"><a name="p21725743171039"></a><a name="p21725743171039"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p55078653171039"><a name="p55078653171039"></a><a name="p55078653171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p65545475171039"><a name="p65545475171039"></a><a name="p65545475171039"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="row24663709171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p56112529171039"><a name="p56112529171039"></a><a name="p56112529171039"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p46656524171039"><a name="p46656524171039"></a><a name="p46656524171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p31778607171039"><a name="p31778607171039"></a><a name="p31778607171039"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="row34212800171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p51657401171039"><a name="p51657401171039"></a><a name="p51657401171039"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p336297171039"><a name="p336297171039"></a><a name="p336297171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p66322352171039"><a name="p66322352171039"></a><a name="p66322352171039"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="row45341886171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p22374403171039"><a name="p22374403171039"></a><a name="p22374403171039"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p16323247171039"><a name="p16323247171039"></a><a name="p16323247171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p9394279212"><a name="p9394279212"></a><a name="p9394279212"></a>zone类型，公网（public）或者内网（private）。</p>
    </td>
    </tr>
    <tr id="row36905265171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p4888971171039"><a name="p4888971171039"></a><a name="p4888971171039"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p16027579171039"><a name="p16027579171039"></a><a name="p16027579171039"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p41240291171039"><a name="p41240291171039"></a><a name="p41240291171039"></a>该zone下SOA记录中的ttl值。</p>
    </td>
    </tr>
    <tr id="row29641334171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p63311148171039"><a name="p63311148171039"></a><a name="p63311148171039"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p26678057171039"><a name="p26678057171039"></a><a name="p26678057171039"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p201115484116"><a name="p201115484116"></a><a name="p201115484116"></a>该zone下SOA记录中用于标识zone文件变更的序列值，用于主从节点同步。</p>
    <p id="p7524749171039"><a name="p7524749171039"></a><a name="p7524749171039"></a>该参数暂未使用。</p>
    </td>
    </tr>
    <tr id="row44990376171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p30244483171039"><a name="p30244483171039"></a><a name="p30244483171039"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p47406357171039"><a name="p47406357171039"></a><a name="p47406357171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p9822846171039"><a name="p9822846171039"></a><a name="p9822846171039"></a>资源状态。</p>
    <p id="p878313571410"><a name="p878313571410"></a><a name="p878313571410"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="row1454557171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p51202644171039"><a name="p51202644171039"></a><a name="p51202644171039"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p32016130171039"><a name="p32016130171039"></a><a name="p32016130171039"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p53878535171039"><a name="p53878535171039"></a><a name="p53878535171039"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="row48476716171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p54136527171039"><a name="p54136527171039"></a><a name="p54136527171039"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p48020249171039"><a name="p48020249171039"></a><a name="p48020249171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p63987755171039"><a name="p63987755171039"></a><a name="p63987755171039"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="row49967872171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p35791512171039"><a name="p35791512171039"></a><a name="p35791512171039"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p10454086171039"><a name="p10454086171039"></a><a name="p10454086171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p8704812171039"><a name="p8704812171039"></a><a name="p8704812171039"></a>zone所属的项目ID。</p>
    </td>
    </tr>
    <tr id="row27690345171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p48529730171039"><a name="p48529730171039"></a><a name="p48529730171039"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p59988242171039"><a name="p59988242171039"></a><a name="p59988242171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p9292793171039"><a name="p9292793171039"></a><a name="p9292793171039"></a>创建时间。</p>
    <p id="p583516468316"><a name="p583516468316"></a><a name="p583516468316"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="row4377608115654"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p5844041115654"><a name="p5844041115654"></a><a name="p5844041115654"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p3605288915654"><a name="p3605288915654"></a><a name="p3605288915654"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p3460290715654"><a name="p3460290715654"></a><a name="p3460290715654"></a>更新时间。</p>
    <p id="p799714202510"><a name="p799714202510"></a><a name="p799714202510"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="row384676871572"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p288749251572"><a name="p288749251572"></a><a name="p288749251572"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p571676251572"><a name="p571676251572"></a><a name="p571676251572"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p50014989155938"><a name="p50014989155938"></a><a name="p50014989155938"></a>指向当前资源或者其他资源的链接。</p>
    <p id="p660161572"><a name="p660161572"></a><a name="p660161572"></a>当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p1967113511455"><a name="p1967113511455"></a><a name="p1967113511455"></a>详细信息请参见<a href="#table52442344175457">表5</a>。</p>
    </td>
    </tr>
    <tr id="row177328815945"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p1595959815945"><a name="p1595959815945"></a><a name="p1595959815945"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p1765902715945"><a name="p1765902715945"></a><a name="p1765902715945"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p2109506015945"><a name="p2109506015945"></a><a name="p2109506015945"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    <p id="p9475575518"><a name="p9475575518"></a><a name="p9475575518"></a>目前暂未使用。</p>
    </td>
    </tr>
    <tr id="row57448667171910"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p3560499171932"><a name="p3560499171932"></a><a name="p3560499171932"></a>router</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p19965041171932"><a name="p19965041171932"></a><a name="p19965041171932"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p6555635171932"><a name="p6555635171932"></a><a name="p6555635171932"></a>Private zone关联的Router(VPC)信息。详细信息请参考<a href="#table4512106017551">表6</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  links参数说明

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
    <tr id="row54251544174716"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.591959195919593%" headers="mcps1.2.4.1.2 "><p id="p19656144517367"><a name="p19656144517367"></a><a name="p19656144517367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.10621062106211%" headers="mcps1.2.4.1.3 "><p id="p76567451365"><a name="p76567451365"></a><a name="p76567451365"></a>下一页资源的链接。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  router对象参数说明

    <a name="table4512106017551"></a>
    <table><thead align="left"><tr id="row2225931917551"><th class="cellrowborder" valign="top" width="18.54%" id="mcps1.2.4.1.1"><p id="p5817443517551"><a name="p5817443517551"></a><a name="p5817443517551"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.46%" id="mcps1.2.4.1.2"><p id="p3436442517551"><a name="p3436442517551"></a><a name="p3436442517551"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62%" id="mcps1.2.4.1.3"><p id="p3205505917551"><a name="p3205505917551"></a><a name="p3205505917551"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row4470351134"><td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.1 "><p id="p38120631175524"><a name="p38120631175524"></a><a name="p38120631175524"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p57184665175519"><a name="p57184665175519"></a><a name="p57184665175519"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p1635999216648"><a name="p1635999216648"></a><a name="p1635999216648"></a>资源状态。</p>
    <p id="p656495918714"><a name="p656495918714"></a><a name="p656495918714"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="row4632297717551"><td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.1 "><p id="p6117366017551"><a name="p6117366017551"></a><a name="p6117366017551"></a>router_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p4937778317551"><a name="p4937778317551"></a><a name="p4937778317551"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p4017744717551"><a name="p4017744717551"></a><a name="p4017744717551"></a>Router(VPC)的ID。</p>
    </td>
    </tr>
    <tr id="row2605270417551"><td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.1 "><p id="p2989427417551"><a name="p2989427417551"></a><a name="p2989427417551"></a>router_region</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46%" headers="mcps1.2.4.1.2 "><p id="p4423327117551"><a name="p4423327117551"></a><a name="p4423327117551"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p2612521117551"><a name="p2612521117551"></a><a name="p2612521117551"></a>Router(VPC)所在的region。</p>
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
        "status": "PENDING_CREATE",
        "links": {
            "self": "https://Endpoint/v2/zones/ff8080825b8fc86c015b94bc6f8712c3"
        },
        "pool_id": "ff8080825ab738f4015ab7513298010e",
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
        "zone_type": "private",
        "created_at": "2017-04-22T08:17:08.997",
        "updated_at": null,
        "record_num": 0,
        "router": {
            "status": "PENDING_CREATE",
            "router_id": "19664294-0bf6-4271-ad3a-94b8c79c6558",
            "router_region": "xx"
        }
    }
    
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

