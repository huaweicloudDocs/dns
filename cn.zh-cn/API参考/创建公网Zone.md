# 创建公网Zone<a name="zh-cn_topic_0057310891"></a>

## 功能介绍<a name="section3569153217343"></a>

创建单个公网Zone。

## URI<a name="section6163262617350"></a>

POST /v2/zones

## 请求<a name="section4207148117353"></a>

-   参数说明

    **表 1**  请求样例的参数说明

    <a name="table3720408817742"></a>
    <table><thead align="left"><tr id="row6225671717742"><th class="cellrowborder" valign="top" width="16.33%" id="mcps1.2.5.1.1"><p id="p5153686617742"><a name="p5153686617742"></a><a name="p5153686617742"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="12.24%" id="mcps1.2.5.1.2"><p id="p473035017742"><a name="p473035017742"></a><a name="p473035017742"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.37%" id="mcps1.2.5.1.3"><p id="p386753717742"><a name="p386753717742"></a><a name="p386753717742"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.059999999999995%" id="mcps1.2.5.1.4"><p id="p5956810717742"><a name="p5956810717742"></a><a name="p5956810717742"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1329410717742"><td class="cellrowborder" valign="top" width="16.33%" headers="mcps1.2.5.1.1 "><p id="p3414560317742"><a name="p3414560317742"></a><a name="p3414560317742"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.2 "><p id="p6603174617742"><a name="p6603174617742"></a><a name="p6603174617742"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.3 "><p id="p360216817742"><a name="p360216817742"></a><a name="p360216817742"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.059999999999995%" headers="mcps1.2.5.1.4 "><p id="p2651334817742"><a name="p2651334817742"></a><a name="p2651334817742"></a>从域名注册商处获得的授权域名。</p>
    <a name="ul1677295557"></a><a name="ul1677295557"></a><ul id="ul1677295557"><li>若以“.”号结束，总长度不超过254个字符。</li><li>若以非“.”号结束，总长度不超过253个字符。</li><li>单个字符串不超过63个字符，字符串间以点号分割。</li></ul>
    <p id="p3680010615524"><a name="p3680010615524"></a><a name="p3680010615524"></a>域名格式不区分大小写，系统会将输入的大写字母统一转换为小写。</p>
    </td>
    </tr>
    <tr id="row1973909717742"><td class="cellrowborder" valign="top" width="16.33%" headers="mcps1.2.5.1.1 "><p id="p5474826717742"><a name="p5474826717742"></a><a name="p5474826717742"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.2 "><p id="p759162017742"><a name="p759162017742"></a><a name="p759162017742"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.3 "><p id="p3220634117742"><a name="p3220634117742"></a><a name="p3220634117742"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.059999999999995%" headers="mcps1.2.5.1.4 "><p id="p6675950017742"><a name="p6675950017742"></a><a name="p6675950017742"></a>域名的描述信息。长度不超过255个字符。</p>
    <p id="p10578150184319"><a name="p10578150184319"></a><a name="p10578150184319"></a>默认值为空。</p>
    </td>
    </tr>
    <tr id="row3526956217742"><td class="cellrowborder" valign="top" width="16.33%" headers="mcps1.2.5.1.1 "><p id="p5656791917742"><a name="p5656791917742"></a><a name="p5656791917742"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.2 "><p id="p2306625217742"><a name="p2306625217742"></a><a name="p2306625217742"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.3 "><p id="p5927915117742"><a name="p5927915117742"></a><a name="p5927915117742"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.059999999999995%" headers="mcps1.2.5.1.4 "><p id="p1460824917742"><a name="p1460824917742"></a><a name="p1460824917742"></a>域名类型，包括公网域名和内网域名。</p>
    <a name="ul3411250511841"></a><a name="ul3411250511841"></a><ul id="ul3411250511841"><li>公网域名（public）：域名可以被internet上的主机访问。</li><li>内网域名（private）：域名仅被具体VPC内的主机访问。</li></ul>
    <p id="p49843158113913"><a name="p49843158113913"></a><a name="p49843158113913"></a>取值范围：public、private。</p>
    <p id="p4789645117742"><a name="p4789645117742"></a><a name="p4789645117742"></a>如果为空，则默认为public。创建内网域名，请参见<a href="创建内网Zone.md">创建内网Zone</a>。</p>
    </td>
    </tr>
    <tr id="row4358988017742"><td class="cellrowborder" valign="top" width="16.33%" headers="mcps1.2.5.1.1 "><p id="p6536976617742"><a name="p6536976617742"></a><a name="p6536976617742"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.2 "><p id="p650279617742"><a name="p650279617742"></a><a name="p650279617742"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.3 "><p id="p2054573717742"><a name="p2054573717742"></a><a name="p2054573717742"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.059999999999995%" headers="mcps1.2.5.1.4 "><p id="p1997196517742"><a name="p1997196517742"></a><a name="p1997196517742"></a>管理该zone的管理员邮箱。</p>
    <p id="p435013473818"><a name="p435013473818"></a><a name="p435013473818"></a>默认值为售后服务邮箱。</p>
    </td>
    </tr>
    <tr id="row13489593141045"><td class="cellrowborder" valign="top" width="16.33%" headers="mcps1.2.5.1.1 "><p id="p18915273141045"><a name="p18915273141045"></a><a name="p18915273141045"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.2 "><p id="p55742162141045"><a name="p55742162141045"></a><a name="p55742162141045"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.3 "><p id="p18821243141045"><a name="p18821243141045"></a><a name="p18821243141045"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.059999999999995%" headers="mcps1.2.5.1.4 "><p id="p3447255141334"><a name="p3447255141334"></a><a name="p3447255141334"></a>用于填写默认生成的SOA记录中有效缓存时间，以秒为单位。</p>
    <p id="p5335091141210"><a name="p5335091141210"></a><a name="p5335091141210"></a>取值范围：</p>
    <p id="p43707626141214"><a name="p43707626141214"></a><a name="p43707626141214"></a>1~2147483647。</p>
    <p id="p9461175874917"><a name="p9461175874917"></a><a name="p9461175874917"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="row964631312824"><td class="cellrowborder" valign="top" width="16.33%" headers="mcps1.2.5.1.1 "><p id="p5754504312824"><a name="p5754504312824"></a><a name="p5754504312824"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.2 "><p id="p3063693212824"><a name="p3063693212824"></a><a name="p3063693212824"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.3 "><p id="p6567246612824"><a name="p6567246612824"></a><a name="p6567246612824"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.059999999999995%" headers="mcps1.2.5.1.4 "><p id="p1786954012824"><a name="p1786954012824"></a><a name="p1786954012824"></a>资源标签。详细信息请参见<a href="数据结构.md#table19530794112436">表2</a>。</p>
    <p id="p391920411506"><a name="p391920411506"></a><a name="p391920411506"></a>默认值为空。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    创建一个公网Zone，域名为“example.com”。

    ```
    POST https://{DNS_Endpoint}/v2/zones
    ```

    ```
    {
        "name": "example.com.",
        "description": "This is an example zone.",
        "zone_type": "public",
        "email": "xx@example.org",
        "ttl": 300,
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

    **表 2**  响应样例的要素说明

    <a name="table54601120171039"></a>
    <table><thead align="left"><tr id="row54125868171039"><th class="cellrowborder" valign="top" width="18.41%" id="mcps1.2.4.1.1"><p id="p46128019171039"><a name="p46128019171039"></a><a name="p46128019171039"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.35%" id="mcps1.2.4.1.2"><p id="p61288737171039"><a name="p61288737171039"></a><a name="p61288737171039"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.239999999999995%" id="mcps1.2.4.1.3"><p id="p39427830171039"><a name="p39427830171039"></a><a name="p39427830171039"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3275315171039"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p13677558171039"><a name="p13677558171039"></a><a name="p13677558171039"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p31480160171039"><a name="p31480160171039"></a><a name="p31480160171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p55186322171039"><a name="p55186322171039"></a><a name="p55186322171039"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="row62038903171039"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p21725743171039"><a name="p21725743171039"></a><a name="p21725743171039"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p55078653171039"><a name="p55078653171039"></a><a name="p55078653171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p65545475171039"><a name="p65545475171039"></a><a name="p65545475171039"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="row24663709171039"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p56112529171039"><a name="p56112529171039"></a><a name="p56112529171039"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p46656524171039"><a name="p46656524171039"></a><a name="p46656524171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p31778607171039"><a name="p31778607171039"></a><a name="p31778607171039"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="row34212800171039"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p51657401171039"><a name="p51657401171039"></a><a name="p51657401171039"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p336297171039"><a name="p336297171039"></a><a name="p336297171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p66322352171039"><a name="p66322352171039"></a><a name="p66322352171039"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="row45341886171039"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p22374403171039"><a name="p22374403171039"></a><a name="p22374403171039"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p16323247171039"><a name="p16323247171039"></a><a name="p16323247171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p58527202171039"><a name="p58527202171039"></a><a name="p58527202171039"></a>zone类型，公网（public）或者内网（private）。</p>
    </td>
    </tr>
    <tr id="row36905265171039"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p4888971171039"><a name="p4888971171039"></a><a name="p4888971171039"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p16027579171039"><a name="p16027579171039"></a><a name="p16027579171039"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p41240291171039"><a name="p41240291171039"></a><a name="p41240291171039"></a>该zone下SOA记录中的ttl值。</p>
    </td>
    </tr>
    <tr id="row29641334171039"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p63311148171039"><a name="p63311148171039"></a><a name="p63311148171039"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p26678057171039"><a name="p26678057171039"></a><a name="p26678057171039"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p201115484116"><a name="p201115484116"></a><a name="p201115484116"></a>该zone下SOA记录中用于标识zone文件变更的序列值，用于主从节点同步。</p>
    <p id="p7524749171039"><a name="p7524749171039"></a><a name="p7524749171039"></a>该参数暂未使用。</p>
    </td>
    </tr>
    <tr id="row44990376171039"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p30244483171039"><a name="p30244483171039"></a><a name="p30244483171039"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p47406357171039"><a name="p47406357171039"></a><a name="p47406357171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p9822846171039"><a name="p9822846171039"></a><a name="p9822846171039"></a>资源状态。</p>
    <p id="p1829154618238"><a name="p1829154618238"></a><a name="p1829154618238"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="row1454557171039"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p51202644171039"><a name="p51202644171039"></a><a name="p51202644171039"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p32016130171039"><a name="p32016130171039"></a><a name="p32016130171039"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p53878535171039"><a name="p53878535171039"></a><a name="p53878535171039"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="row48476716171039"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p54136527171039"><a name="p54136527171039"></a><a name="p54136527171039"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p48020249171039"><a name="p48020249171039"></a><a name="p48020249171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p63987755171039"><a name="p63987755171039"></a><a name="p63987755171039"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="row49967872171039"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p35791512171039"><a name="p35791512171039"></a><a name="p35791512171039"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p10454086171039"><a name="p10454086171039"></a><a name="p10454086171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p8704812171039"><a name="p8704812171039"></a><a name="p8704812171039"></a>zone所属的项目ID。</p>
    </td>
    </tr>
    <tr id="row27690345171039"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p48529730171039"><a name="p48529730171039"></a><a name="p48529730171039"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p59988242171039"><a name="p59988242171039"></a><a name="p59988242171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p9292793171039"><a name="p9292793171039"></a><a name="p9292793171039"></a>创建时间。</p>
    <p id="p1283123217317"><a name="p1283123217317"></a><a name="p1283123217317"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="row4377608115654"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p5844041115654"><a name="p5844041115654"></a><a name="p5844041115654"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p3605288915654"><a name="p3605288915654"></a><a name="p3605288915654"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p3460290715654"><a name="p3460290715654"></a><a name="p3460290715654"></a>更新时间。</p>
    <p id="p583516468316"><a name="p583516468316"></a><a name="p583516468316"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="row384676871572"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p288749251572"><a name="p288749251572"></a><a name="p288749251572"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p571676251572"><a name="p571676251572"></a><a name="p571676251572"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p660161572"><a name="p660161572"></a><a name="p660161572"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p134911211113714"><a name="p134911211113714"></a><a name="p134911211113714"></a>详细信息请参见<a href="#table0172144213344">表3</a>。</p>
    </td>
    </tr>
    <tr id="row177328815945"><td class="cellrowborder" valign="top" width="18.41%" headers="mcps1.2.4.1.1 "><p id="p1595959815945"><a name="p1595959815945"></a><a name="p1595959815945"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.35%" headers="mcps1.2.4.1.2 "><p id="p1765902715945"><a name="p1765902715945"></a><a name="p1765902715945"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="p2109506015945"><a name="p2109506015945"></a><a name="p2109506015945"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    <p id="p05918233215"><a name="p05918233215"></a><a name="p05918233215"></a>目前暂未使用。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  links对象参数说明

    <a name="table0172144213344"></a>
    <table><thead align="left"><tr id="row917304253418"><th class="cellrowborder" valign="top" width="18%" id="mcps1.2.4.1.1"><p id="p101731742153416"><a name="p101731742153416"></a><a name="p101731742153416"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.25%" id="mcps1.2.4.1.2"><p id="p0174542163418"><a name="p0174542163418"></a><a name="p0174542163418"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.74999999999999%" id="mcps1.2.4.1.3"><p id="p7174194243414"><a name="p7174194243414"></a><a name="p7174194243414"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1390694871216"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="p8907184881217"><a name="p8907184881217"></a><a name="p8907184881217"></a>self</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.25%" headers="mcps1.2.4.1.2 "><p id="p9907184891219"><a name="p9907184891219"></a><a name="p9907184891219"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.74999999999999%" headers="mcps1.2.4.1.3 "><p id="p1890754813127"><a name="p1890754813127"></a><a name="p1890754813127"></a>当前资源的链接。</p>
    </td>
    </tr>
    <tr id="row19871743164619"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.25%" headers="mcps1.2.4.1.2 "><p id="p19656144517367"><a name="p19656144517367"></a><a name="p19656144517367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.74999999999999%" headers="mcps1.2.4.1.3 "><p id="p76567451365"><a name="p76567451365"></a><a name="p76567451365"></a>下一页资源的链接。</p>
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
        "serial": 1,
        "masters": [],
        "status": "PENDING_CREATE",
        "links": {
            "self": "https://Endpoint/v2/zones/2c9eb155587194ec01587224c9f90149"
        },
        "pool_id": "00000000570e54ee01570e9939b20019",
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
        "zone_type": "public",
        "created_at": "2016-11-17T11:56:03.439",
        "updated_at": null,
        "record_num": 0
    }
    
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

