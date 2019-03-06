# 创建内网Zone<a name="ZH-CN_TOPIC_0057311027"></a>

## 功能介绍<a name="section3569153217343"></a>

创建单个内网Zone。

## URI<a name="section6163262617350"></a>

POST /v2/zones

## 请求<a name="section4207148117353"></a>

-   参数说明

    **表 1**  请求样例的参数说明

    <a name="table3720408817742"></a>
    <table><thead align="left"><tr id="row6225671717742"><th class="cellrowborder" valign="top" width="16.330000000000002%" id="mcps1.2.5.1.1"><p id="p5153686617742"><a name="p5153686617742"></a><a name="p5153686617742"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.740000000000002%" id="mcps1.2.5.1.2"><p id="p473035017742"><a name="p473035017742"></a><a name="p473035017742"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="12.730000000000002%" id="mcps1.2.5.1.3"><p id="p386753717742"><a name="p386753717742"></a><a name="p386753717742"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.2%" id="mcps1.2.5.1.4"><p id="p5956810717742"><a name="p5956810717742"></a><a name="p5956810717742"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1329410717742"><td class="cellrowborder" valign="top" width="16.330000000000002%" headers="mcps1.2.5.1.1 "><p id="p3414560317742"><a name="p3414560317742"></a><a name="p3414560317742"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.740000000000002%" headers="mcps1.2.5.1.2 "><p id="p6603174617742"><a name="p6603174617742"></a><a name="p6603174617742"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.730000000000002%" headers="mcps1.2.5.1.3 "><p id="p360216817742"><a name="p360216817742"></a><a name="p360216817742"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.2%" headers="mcps1.2.5.1.4 "><p id="p2651334817742"><a name="p2651334817742"></a><a name="p2651334817742"></a>待创建的域名。</p>
    <a name="ul1536534155329"></a><a name="ul1536534155329"></a><ul id="ul1536534155329"><li>若以“.”号结束，总长度不超过254个字符。</li><li>若以非“.”号结束，总长度不超过253个字符。</li><li>单个字符串不超过63个字符，字符串间以点号分割。</li></ul>
    <p id="p61100872151329"><a name="p61100872151329"></a><a name="p61100872151329"></a>域名格式不区分大小写，系统会将输入的大写字母统一转换为小写。</p>
    </td>
    </tr>
    <tr id="row1973909717742"><td class="cellrowborder" valign="top" width="16.330000000000002%" headers="mcps1.2.5.1.1 "><p id="p5474826717742"><a name="p5474826717742"></a><a name="p5474826717742"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.740000000000002%" headers="mcps1.2.5.1.2 "><p id="p759162017742"><a name="p759162017742"></a><a name="p759162017742"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.730000000000002%" headers="mcps1.2.5.1.3 "><p id="p3220634117742"><a name="p3220634117742"></a><a name="p3220634117742"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.2%" headers="mcps1.2.5.1.4 "><p id="p44313881155342"><a name="p44313881155342"></a><a name="p44313881155342"></a>域名的描述信息。</p>
    <p id="p6675950017742"><a name="p6675950017742"></a><a name="p6675950017742"></a>长度不超过255个字符。</p>
    </td>
    </tr>
    <tr id="row3526956217742"><td class="cellrowborder" valign="top" width="16.330000000000002%" headers="mcps1.2.5.1.1 "><p id="p5656791917742"><a name="p5656791917742"></a><a name="p5656791917742"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.740000000000002%" headers="mcps1.2.5.1.2 "><p id="p2306625217742"><a name="p2306625217742"></a><a name="p2306625217742"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.730000000000002%" headers="mcps1.2.5.1.3 "><p id="p5927915117742"><a name="p5927915117742"></a><a name="p5927915117742"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.2%" headers="mcps1.2.5.1.4 "><p id="p92377632066"><a name="p92377632066"></a><a name="p92377632066"></a>域名类型。</p>
    <p id="p100613092066"><a name="p100613092066"></a><a name="p100613092066"></a>内网域名：域名仅被具体VPC内的主机访问。</p>
    <p id="p2001526020713"><a name="p2001526020713"></a><a name="p2001526020713"></a>取值：private。</p>
    <p id="p96596832066"><a name="p96596832066"></a><a name="p96596832066"></a>创建公网域名，请参见<a href="创建公网Zone.md">创建公网Zone</a>。</p>
    </td>
    </tr>
    <tr id="row4358988017742"><td class="cellrowborder" valign="top" width="16.330000000000002%" headers="mcps1.2.5.1.1 "><p id="p6536976617742"><a name="p6536976617742"></a><a name="p6536976617742"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.740000000000002%" headers="mcps1.2.5.1.2 "><p id="p650279617742"><a name="p650279617742"></a><a name="p650279617742"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.730000000000002%" headers="mcps1.2.5.1.3 "><p id="p2054573717742"><a name="p2054573717742"></a><a name="p2054573717742"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.2%" headers="mcps1.2.5.1.4 "><p id="p1997196517742"><a name="p1997196517742"></a><a name="p1997196517742"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="row13489593141045"><td class="cellrowborder" valign="top" width="16.330000000000002%" headers="mcps1.2.5.1.1 "><p id="p18915273141045"><a name="p18915273141045"></a><a name="p18915273141045"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.740000000000002%" headers="mcps1.2.5.1.2 "><p id="p55742162141045"><a name="p55742162141045"></a><a name="p55742162141045"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.730000000000002%" headers="mcps1.2.5.1.3 "><p id="p18821243141045"><a name="p18821243141045"></a><a name="p18821243141045"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.2%" headers="mcps1.2.5.1.4 "><p id="p3447255141334"><a name="p3447255141334"></a><a name="p3447255141334"></a>用于填写默认生成的SOA记录中有效缓存时间，以秒为单位。</p>
    <p id="p54818170173211"><a name="p54818170173211"></a><a name="p54818170173211"></a>默认值为300s。</p>
    <p id="p5335091141210"><a name="p5335091141210"></a><a name="p5335091141210"></a>取值范围：300～2147483647</p>
    </td>
    </tr>
    <tr id="row18045881171648"><td class="cellrowborder" valign="top" width="16.330000000000002%" headers="mcps1.2.5.1.1 "><p id="p20204595171650"><a name="p20204595171650"></a><a name="p20204595171650"></a>router</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.740000000000002%" headers="mcps1.2.5.1.2 "><p id="p25959495171650"><a name="p25959495171650"></a><a name="p25959495171650"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.730000000000002%" headers="mcps1.2.5.1.3 "><p id="p22344380171650"><a name="p22344380171650"></a><a name="p22344380171650"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.2%" headers="mcps1.2.5.1.4 "><p id="p65064378171650"><a name="p65064378171650"></a><a name="p65064378171650"></a>Private zone关联的Router(VPC)信息，详细信息请参见<a href="#table4448008117179">表2</a>。</p>
    </td>
    </tr>
    <tr id="row3748545412107"><td class="cellrowborder" valign="top" width="16.330000000000002%" headers="mcps1.2.5.1.1 "><p id="p6123289312107"><a name="p6123289312107"></a><a name="p6123289312107"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.740000000000002%" headers="mcps1.2.5.1.2 "><p id="p6091732812107"><a name="p6091732812107"></a><a name="p6091732812107"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.730000000000002%" headers="mcps1.2.5.1.3 "><p id="p3535651512107"><a name="p3535651512107"></a><a name="p3535651512107"></a>tag</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.2%" headers="mcps1.2.5.1.4 "><p id="p4530543812107"><a name="p4530543812107"></a><a name="p4530543812107"></a>资源标签。详细信息请参见请参见<a href="#table19530794112436">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  Router对象参数说明

    <a name="table4448008117179"></a>
    <table><thead align="left"><tr id="row6132935617179"><th class="cellrowborder" valign="top" width="18.09%" id="mcps1.2.5.1.1"><p id="p36588677171719"><a name="p36588677171719"></a><a name="p36588677171719"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="10.61%" id="mcps1.2.5.1.2"><p id="p10892865171719"><a name="p10892865171719"></a><a name="p10892865171719"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.48%" id="mcps1.2.5.1.3"><p id="p9906869171719"><a name="p9906869171719"></a><a name="p9906869171719"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="52.82%" id="mcps1.2.5.1.4"><p id="p64258954171719"><a name="p64258954171719"></a><a name="p64258954171719"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row266872817179"><td class="cellrowborder" valign="top" width="18.09%" headers="mcps1.2.5.1.1 "><p id="p25118582171719"><a name="p25118582171719"></a><a name="p25118582171719"></a>router_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="10.61%" headers="mcps1.2.5.1.2 "><p id="p21339228171719"><a name="p21339228171719"></a><a name="p21339228171719"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.48%" headers="mcps1.2.5.1.3 "><p id="p50755907171719"><a name="p50755907171719"></a><a name="p50755907171719"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.82%" headers="mcps1.2.5.1.4 "><p id="p17587794171719"><a name="p17587794171719"></a><a name="p17587794171719"></a>Router(VPC)的ID。</p>
    </td>
    </tr>
    <tr id="row6657832817179"><td class="cellrowborder" valign="top" width="18.09%" headers="mcps1.2.5.1.1 "><p id="p3709384171719"><a name="p3709384171719"></a><a name="p3709384171719"></a>router_region</p>
    </td>
    <td class="cellrowborder" valign="top" width="10.61%" headers="mcps1.2.5.1.2 "><p id="p32024676171719"><a name="p32024676171719"></a><a name="p32024676171719"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.48%" headers="mcps1.2.5.1.3 "><p id="p43861924171719"><a name="p43861924171719"></a><a name="p43861924171719"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.82%" headers="mcps1.2.5.1.4 "><p id="p63154928171719"><a name="p63154928171719"></a><a name="p63154928171719"></a>Router(VPC)所在的region。</p>
    <p id="p38645142171939"><a name="p38645142171939"></a><a name="p38645142171939"></a>如果为空，默认为token中project所在的region。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  tag对象参数说明

    <a name="table19530794112436"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0057310891_row15361836112436"><th class="cellrowborder" valign="top" width="15.21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0057310891_p58707511112436"><a name="zh-cn_topic_0057310891_p58707511112436"></a><a name="zh-cn_topic_0057310891_p58707511112436"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.57%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0057310891_p57687928112436"><a name="zh-cn_topic_0057310891_p57687928112436"></a><a name="zh-cn_topic_0057310891_p57687928112436"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.28%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0057310891_p42210623112436"><a name="zh-cn_topic_0057310891_p42210623112436"></a><a name="zh-cn_topic_0057310891_p42210623112436"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="52.94%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0057310891_p63617265112436"><a name="zh-cn_topic_0057310891_p63617265112436"></a><a name="zh-cn_topic_0057310891_p63617265112436"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0057310891_row35684479112436"><td class="cellrowborder" valign="top" width="15.21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0057310891_p13313439112530"><a name="zh-cn_topic_0057310891_p13313439112530"></a><a name="zh-cn_topic_0057310891_p13313439112530"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.57%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0057310891_p50150432112436"><a name="zh-cn_topic_0057310891_p50150432112436"></a><a name="zh-cn_topic_0057310891_p50150432112436"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.28%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0057310891_p35653193112436"><a name="zh-cn_topic_0057310891_p35653193112436"></a><a name="zh-cn_topic_0057310891_p35653193112436"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.94%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0057310891_p48921437201850"><a name="zh-cn_topic_0057310891_p48921437201850"></a><a name="zh-cn_topic_0057310891_p48921437201850"></a>键。最大长度36个unicode字符。 key不能为空。不能包含“=”,“*”,“&lt;”,“&gt;”,“\”,“,”,“|”,“/”，且首尾字符不能为空格。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057310891_row20048002112436"><td class="cellrowborder" valign="top" width="15.21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0057310891_p66095544112533"><a name="zh-cn_topic_0057310891_p66095544112533"></a><a name="zh-cn_topic_0057310891_p66095544112533"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.57%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0057310891_p1570770112436"><a name="zh-cn_topic_0057310891_p1570770112436"></a><a name="zh-cn_topic_0057310891_p1570770112436"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.28%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0057310891_p60123528112436"><a name="zh-cn_topic_0057310891_p60123528112436"></a><a name="zh-cn_topic_0057310891_p60123528112436"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.94%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0057310891_p61714725112922"><a name="zh-cn_topic_0057310891_p61714725112922"></a><a name="zh-cn_topic_0057310891_p61714725112922"></a>值。每个值最大长度43个unicode字符，可以为空字符串。 不能包含“=”,“*”,“&lt;”,“&gt;”,“\”,“,”,“|”,“/”，且首尾字符不能为空格。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "name": "example.com.",
        "description": "This is an example zone.",
        "zone_type": "private",
        "email": "xx@example.org",
        "router": {
            "router_id": "19664294-0bf6-4271-ad3a-94b8c79c6558",
            "router_region": "xx"
        }
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
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p31480160171039"><a name="p31480160171039"></a><a name="p31480160171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p55186322171039"><a name="p55186322171039"></a><a name="p55186322171039"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="row62038903171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p21725743171039"><a name="p21725743171039"></a><a name="p21725743171039"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p55078653171039"><a name="p55078653171039"></a><a name="p55078653171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p65545475171039"><a name="p65545475171039"></a><a name="p65545475171039"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="row24663709171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p56112529171039"><a name="p56112529171039"></a><a name="p56112529171039"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p46656524171039"><a name="p46656524171039"></a><a name="p46656524171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p31778607171039"><a name="p31778607171039"></a><a name="p31778607171039"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="row34212800171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p51657401171039"><a name="p51657401171039"></a><a name="p51657401171039"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p336297171039"><a name="p336297171039"></a><a name="p336297171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p66322352171039"><a name="p66322352171039"></a><a name="p66322352171039"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="row45341886171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p22374403171039"><a name="p22374403171039"></a><a name="p22374403171039"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p16323247171039"><a name="p16323247171039"></a><a name="p16323247171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p58527202171039"><a name="p58527202171039"></a><a name="p58527202171039"></a>zone类型，公网或者内网。</p>
    </td>
    </tr>
    <tr id="row36905265171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p4888971171039"><a name="p4888971171039"></a><a name="p4888971171039"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p16027579171039"><a name="p16027579171039"></a><a name="p16027579171039"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p41240291171039"><a name="p41240291171039"></a><a name="p41240291171039"></a>该zone下SOA记录中的ttl值。</p>
    </td>
    </tr>
    <tr id="row29641334171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p63311148171039"><a name="p63311148171039"></a><a name="p63311148171039"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p26678057171039"><a name="p26678057171039"></a><a name="p26678057171039"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p7524749171039"><a name="p7524749171039"></a><a name="p7524749171039"></a>该zone下SOA记录中用于标识变更的序列值。</p>
    </td>
    </tr>
    <tr id="row44990376171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p30244483171039"><a name="p30244483171039"></a><a name="p30244483171039"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p47406357171039"><a name="p47406357171039"></a><a name="p47406357171039"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p9822846171039"><a name="p9822846171039"></a><a name="p9822846171039"></a>资源状态。</p>
    <p id="p36239781171039"><a name="p36239781171039"></a><a name="p36239781171039"></a>取值范围：PENDING_CREATE、ACTIVE、PENDING_DELETE、ERROR。</p>
    </td>
    </tr>
    <tr id="row1454557171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p51202644171039"><a name="p51202644171039"></a><a name="p51202644171039"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p32016130171039"><a name="p32016130171039"></a><a name="p32016130171039"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p53878535171039"><a name="p53878535171039"></a><a name="p53878535171039"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="row48476716171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p54136527171039"><a name="p54136527171039"></a><a name="p54136527171039"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p48020249171039"><a name="p48020249171039"></a><a name="p48020249171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p63987755171039"><a name="p63987755171039"></a><a name="p63987755171039"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="row49967872171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p35791512171039"><a name="p35791512171039"></a><a name="p35791512171039"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p10454086171039"><a name="p10454086171039"></a><a name="p10454086171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p8704812171039"><a name="p8704812171039"></a><a name="p8704812171039"></a>zone所属的租户ID。</p>
    </td>
    </tr>
    <tr id="row27690345171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p48529730171039"><a name="p48529730171039"></a><a name="p48529730171039"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p59988242171039"><a name="p59988242171039"></a><a name="p59988242171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p9292793171039"><a name="p9292793171039"></a><a name="p9292793171039"></a>创建时间。</p>
    </td>
    </tr>
    <tr id="row4377608115654"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p5844041115654"><a name="p5844041115654"></a><a name="p5844041115654"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p3605288915654"><a name="p3605288915654"></a><a name="p3605288915654"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p3460290715654"><a name="p3460290715654"></a><a name="p3460290715654"></a>更新时间。</p>
    </td>
    </tr>
    <tr id="row384676871572"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p288749251572"><a name="p288749251572"></a><a name="p288749251572"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p571676251572"><a name="p571676251572"></a><a name="p571676251572"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p50014989155938"><a name="p50014989155938"></a><a name="p50014989155938"></a>指向当前资源或者其他资源的链接。</p>
    <p id="p660161572"><a name="p660161572"></a><a name="p660161572"></a>当查询需要分页时，需要包含一个next链接指向下一页。</p>
    </td>
    </tr>
    <tr id="row177328815945"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p1595959815945"><a name="p1595959815945"></a><a name="p1595959815945"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p1765902715945"><a name="p1765902715945"></a><a name="p1765902715945"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p2109506015945"><a name="p2109506015945"></a><a name="p2109506015945"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    </td>
    </tr>
    <tr id="row57448667171910"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p3560499171932"><a name="p3560499171932"></a><a name="p3560499171932"></a>router</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="p19965041171932"><a name="p19965041171932"></a><a name="p19965041171932"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p6555635171932"><a name="p6555635171932"></a><a name="p6555635171932"></a>Private zone关联的Router(VPC)信息。</p>
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


## 返回值<a name="section1917896317411"></a>

请参考[通用请求返回值](通用请求返回值.md)。

