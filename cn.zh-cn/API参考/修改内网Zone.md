# 修改内网Zone<a name="ZH-CN_TOPIC_0080996887"></a>

## 功能介绍<a name="section3569153217343"></a>

修改单个Zone。

## URI<a name="section6163262617350"></a>

PATCH /v2/zones/\{zone\_id\}

参数说明请参见[表1](#zh-cn_topic_0080995382_table56746773172616)。

**表 1**  URI格式的参数说明

<a name="zh-cn_topic_0080995382_table56746773172616"></a>
<table><thead align="left"><tr id="zh-cn_topic_0080995382_row12848229172616"><th class="cellrowborder" valign="top" width="15.459999999999999%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0080995382_p44975878172616"><a name="zh-cn_topic_0080995382_p44975878172616"></a><a name="zh-cn_topic_0080995382_p44975878172616"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.459999999999999%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0080995382_p46443918172616"><a name="zh-cn_topic_0080995382_p46443918172616"></a><a name="zh-cn_topic_0080995382_p46443918172616"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.53%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0080995382_p1368350172616"><a name="zh-cn_topic_0080995382_p1368350172616"></a><a name="zh-cn_topic_0080995382_p1368350172616"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.55%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0080995382_p24157908172616"><a name="zh-cn_topic_0080995382_p24157908172616"></a><a name="zh-cn_topic_0080995382_p24157908172616"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0080995382_row39993297172616"><td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0080995382_p43071797172616"><a name="zh-cn_topic_0080995382_p43071797172616"></a><a name="zh-cn_topic_0080995382_p43071797172616"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0080995382_p26647585172616"><a name="zh-cn_topic_0080995382_p26647585172616"></a><a name="zh-cn_topic_0080995382_p26647585172616"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0080995382_p21075379172616"><a name="zh-cn_topic_0080995382_p21075379172616"></a><a name="zh-cn_topic_0080995382_p21075379172616"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="51.55%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0080995382_p4976396172616"><a name="zh-cn_topic_0080995382_p4976396172616"></a><a name="zh-cn_topic_0080995382_p4976396172616"></a>待修改zone的ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section4207148117353"></a>

-   参数说明

    **表 2**  请求样例的参数说明

    <a name="zh-cn_topic_0080995382_table3720408817742"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0080995382_row6225671717742"><th class="cellrowborder" valign="top" width="16.33%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0080995382_p5153686617742"><a name="zh-cn_topic_0080995382_p5153686617742"></a><a name="zh-cn_topic_0080995382_p5153686617742"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="12.24%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0080995382_p473035017742"><a name="zh-cn_topic_0080995382_p473035017742"></a><a name="zh-cn_topic_0080995382_p473035017742"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.37%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0080995382_p386753717742"><a name="zh-cn_topic_0080995382_p386753717742"></a><a name="zh-cn_topic_0080995382_p386753717742"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.059999999999995%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0080995382_p5956810717742"><a name="zh-cn_topic_0080995382_p5956810717742"></a><a name="zh-cn_topic_0080995382_p5956810717742"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0080995382_row1973909717742"><td class="cellrowborder" valign="top" width="16.33%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0080995382_p5474826717742"><a name="zh-cn_topic_0080995382_p5474826717742"></a><a name="zh-cn_topic_0080995382_p5474826717742"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0080995382_p759162017742"><a name="zh-cn_topic_0080995382_p759162017742"></a><a name="zh-cn_topic_0080995382_p759162017742"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0080995382_p3220634117742"><a name="zh-cn_topic_0080995382_p3220634117742"></a><a name="zh-cn_topic_0080995382_p3220634117742"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.059999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0080995382_p6675950017742"><a name="zh-cn_topic_0080995382_p6675950017742"></a><a name="zh-cn_topic_0080995382_p6675950017742"></a>域名的描述信息。长度不超过255个字符。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0080995382_row4358988017742"><td class="cellrowborder" valign="top" width="16.33%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0080995382_p6536976617742"><a name="zh-cn_topic_0080995382_p6536976617742"></a><a name="zh-cn_topic_0080995382_p6536976617742"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0080995382_p650279617742"><a name="zh-cn_topic_0080995382_p650279617742"></a><a name="zh-cn_topic_0080995382_p650279617742"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0080995382_p2054573717742"><a name="zh-cn_topic_0080995382_p2054573717742"></a><a name="zh-cn_topic_0080995382_p2054573717742"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.059999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0080995382_p1997196517742"><a name="zh-cn_topic_0080995382_p1997196517742"></a><a name="zh-cn_topic_0080995382_p1997196517742"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0080995382_row13489593141045"><td class="cellrowborder" valign="top" width="16.33%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0080995382_p18915273141045"><a name="zh-cn_topic_0080995382_p18915273141045"></a><a name="zh-cn_topic_0080995382_p18915273141045"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0080995382_p55742162141045"><a name="zh-cn_topic_0080995382_p55742162141045"></a><a name="zh-cn_topic_0080995382_p55742162141045"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0080995382_p18821243141045"><a name="zh-cn_topic_0080995382_p18821243141045"></a><a name="zh-cn_topic_0080995382_p18821243141045"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.059999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0080995382_p3447255141334"><a name="zh-cn_topic_0080995382_p3447255141334"></a><a name="zh-cn_topic_0080995382_p3447255141334"></a>用于填写默认生成的SOA记录中有效缓存时间，以秒为单位。</p>
    <p id="zh-cn_topic_0080995382_p54818170173211"><a name="zh-cn_topic_0080995382_p54818170173211"></a><a name="zh-cn_topic_0080995382_p54818170173211"></a>默认值为300s。</p>
    <p id="zh-cn_topic_0080995382_p5335091141210"><a name="zh-cn_topic_0080995382_p5335091141210"></a><a name="zh-cn_topic_0080995382_p5335091141210"></a>取值范围：</p>
    <p id="zh-cn_topic_0080995382_p43707626141214"><a name="zh-cn_topic_0080995382_p43707626141214"></a><a name="zh-cn_topic_0080995382_p43707626141214"></a>300-2147483647。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "description": "This is an example zone.",
        "email": "xx@example.org",
        "ttl": 300
    }
    ```


## 响应<a name="section2142173017358"></a>

-   要素说明

    **表 3**  响应样例的要素说明

    <a name="table54601120171039"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0057311027_row54125868171039"><th class="cellrowborder" valign="top" width="18.37%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0057311027_p46128019171039"><a name="zh-cn_topic_0057311027_p46128019171039"></a><a name="zh-cn_topic_0057311027_p46128019171039"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.39%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0057311027_p61288737171039"><a name="zh-cn_topic_0057311027_p61288737171039"></a><a name="zh-cn_topic_0057311027_p61288737171039"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.239999999999995%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0057311027_p39427830171039"><a name="zh-cn_topic_0057311027_p39427830171039"></a><a name="zh-cn_topic_0057311027_p39427830171039"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0057311027_row3275315171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p13677558171039"><a name="zh-cn_topic_0057311027_p13677558171039"></a><a name="zh-cn_topic_0057311027_p13677558171039"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p31480160171039"><a name="zh-cn_topic_0057311027_p31480160171039"></a><a name="zh-cn_topic_0057311027_p31480160171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p55186322171039"><a name="zh-cn_topic_0057311027_p55186322171039"></a><a name="zh-cn_topic_0057311027_p55186322171039"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row62038903171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p21725743171039"><a name="zh-cn_topic_0057311027_p21725743171039"></a><a name="zh-cn_topic_0057311027_p21725743171039"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p55078653171039"><a name="zh-cn_topic_0057311027_p55078653171039"></a><a name="zh-cn_topic_0057311027_p55078653171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p65545475171039"><a name="zh-cn_topic_0057311027_p65545475171039"></a><a name="zh-cn_topic_0057311027_p65545475171039"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row24663709171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p56112529171039"><a name="zh-cn_topic_0057311027_p56112529171039"></a><a name="zh-cn_topic_0057311027_p56112529171039"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p46656524171039"><a name="zh-cn_topic_0057311027_p46656524171039"></a><a name="zh-cn_topic_0057311027_p46656524171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p31778607171039"><a name="zh-cn_topic_0057311027_p31778607171039"></a><a name="zh-cn_topic_0057311027_p31778607171039"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row34212800171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p51657401171039"><a name="zh-cn_topic_0057311027_p51657401171039"></a><a name="zh-cn_topic_0057311027_p51657401171039"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p336297171039"><a name="zh-cn_topic_0057311027_p336297171039"></a><a name="zh-cn_topic_0057311027_p336297171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p66322352171039"><a name="zh-cn_topic_0057311027_p66322352171039"></a><a name="zh-cn_topic_0057311027_p66322352171039"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row45341886171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p22374403171039"><a name="zh-cn_topic_0057311027_p22374403171039"></a><a name="zh-cn_topic_0057311027_p22374403171039"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p16323247171039"><a name="zh-cn_topic_0057311027_p16323247171039"></a><a name="zh-cn_topic_0057311027_p16323247171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p58527202171039"><a name="zh-cn_topic_0057311027_p58527202171039"></a><a name="zh-cn_topic_0057311027_p58527202171039"></a>zone类型，公网或者内网。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row36905265171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p4888971171039"><a name="zh-cn_topic_0057311027_p4888971171039"></a><a name="zh-cn_topic_0057311027_p4888971171039"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p16027579171039"><a name="zh-cn_topic_0057311027_p16027579171039"></a><a name="zh-cn_topic_0057311027_p16027579171039"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p41240291171039"><a name="zh-cn_topic_0057311027_p41240291171039"></a><a name="zh-cn_topic_0057311027_p41240291171039"></a>该zone下SOA记录中的ttl值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row29641334171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p63311148171039"><a name="zh-cn_topic_0057311027_p63311148171039"></a><a name="zh-cn_topic_0057311027_p63311148171039"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p26678057171039"><a name="zh-cn_topic_0057311027_p26678057171039"></a><a name="zh-cn_topic_0057311027_p26678057171039"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p7524749171039"><a name="zh-cn_topic_0057311027_p7524749171039"></a><a name="zh-cn_topic_0057311027_p7524749171039"></a>该zone下SOA记录中用于标识变更的序列值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row44990376171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p30244483171039"><a name="zh-cn_topic_0057311027_p30244483171039"></a><a name="zh-cn_topic_0057311027_p30244483171039"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p47406357171039"><a name="zh-cn_topic_0057311027_p47406357171039"></a><a name="zh-cn_topic_0057311027_p47406357171039"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p9822846171039"><a name="zh-cn_topic_0057311027_p9822846171039"></a><a name="zh-cn_topic_0057311027_p9822846171039"></a>资源状态。</p>
    <p id="zh-cn_topic_0057311027_p36239781171039"><a name="zh-cn_topic_0057311027_p36239781171039"></a><a name="zh-cn_topic_0057311027_p36239781171039"></a>取值范围：PENDING_CREATE、ACTIVE、PENDING_DELETE、ERROR。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row1454557171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p51202644171039"><a name="zh-cn_topic_0057311027_p51202644171039"></a><a name="zh-cn_topic_0057311027_p51202644171039"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p32016130171039"><a name="zh-cn_topic_0057311027_p32016130171039"></a><a name="zh-cn_topic_0057311027_p32016130171039"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p53878535171039"><a name="zh-cn_topic_0057311027_p53878535171039"></a><a name="zh-cn_topic_0057311027_p53878535171039"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row48476716171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p54136527171039"><a name="zh-cn_topic_0057311027_p54136527171039"></a><a name="zh-cn_topic_0057311027_p54136527171039"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p48020249171039"><a name="zh-cn_topic_0057311027_p48020249171039"></a><a name="zh-cn_topic_0057311027_p48020249171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p63987755171039"><a name="zh-cn_topic_0057311027_p63987755171039"></a><a name="zh-cn_topic_0057311027_p63987755171039"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row49967872171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p35791512171039"><a name="zh-cn_topic_0057311027_p35791512171039"></a><a name="zh-cn_topic_0057311027_p35791512171039"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p10454086171039"><a name="zh-cn_topic_0057311027_p10454086171039"></a><a name="zh-cn_topic_0057311027_p10454086171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p8704812171039"><a name="zh-cn_topic_0057311027_p8704812171039"></a><a name="zh-cn_topic_0057311027_p8704812171039"></a>zone所属的租户ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row27690345171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p48529730171039"><a name="zh-cn_topic_0057311027_p48529730171039"></a><a name="zh-cn_topic_0057311027_p48529730171039"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p59988242171039"><a name="zh-cn_topic_0057311027_p59988242171039"></a><a name="zh-cn_topic_0057311027_p59988242171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p9292793171039"><a name="zh-cn_topic_0057311027_p9292793171039"></a><a name="zh-cn_topic_0057311027_p9292793171039"></a>创建时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row4377608115654"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p5844041115654"><a name="zh-cn_topic_0057311027_p5844041115654"></a><a name="zh-cn_topic_0057311027_p5844041115654"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p3605288915654"><a name="zh-cn_topic_0057311027_p3605288915654"></a><a name="zh-cn_topic_0057311027_p3605288915654"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p3460290715654"><a name="zh-cn_topic_0057311027_p3460290715654"></a><a name="zh-cn_topic_0057311027_p3460290715654"></a>更新时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row384676871572"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p288749251572"><a name="zh-cn_topic_0057311027_p288749251572"></a><a name="zh-cn_topic_0057311027_p288749251572"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p571676251572"><a name="zh-cn_topic_0057311027_p571676251572"></a><a name="zh-cn_topic_0057311027_p571676251572"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p50014989155938"><a name="zh-cn_topic_0057311027_p50014989155938"></a><a name="zh-cn_topic_0057311027_p50014989155938"></a>指向当前资源或者其他资源的链接。</p>
    <p id="zh-cn_topic_0057311027_p660161572"><a name="zh-cn_topic_0057311027_p660161572"></a><a name="zh-cn_topic_0057311027_p660161572"></a>当查询需要分页时，需要包含一个next链接指向下一页。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row177328815945"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p1595959815945"><a name="zh-cn_topic_0057311027_p1595959815945"></a><a name="zh-cn_topic_0057311027_p1595959815945"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p1765902715945"><a name="zh-cn_topic_0057311027_p1765902715945"></a><a name="zh-cn_topic_0057311027_p1765902715945"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p2109506015945"><a name="zh-cn_topic_0057311027_p2109506015945"></a><a name="zh-cn_topic_0057311027_p2109506015945"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057311027_row57448667171910"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057311027_p3560499171932"><a name="zh-cn_topic_0057311027_p3560499171932"></a><a name="zh-cn_topic_0057311027_p3560499171932"></a>router</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0057311027_p19965041171932"><a name="zh-cn_topic_0057311027_p19965041171932"></a><a name="zh-cn_topic_0057311027_p19965041171932"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057311027_p6555635171932"><a name="zh-cn_topic_0057311027_p6555635171932"></a><a name="zh-cn_topic_0057311027_p6555635171932"></a>Private zone关联的Router(VPC)信息。</p>
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
        "status": "ACTIVE",
        "links": {
            "self": "https://Endpoint/v2/zones/ff8080825b8fc86c015b94bc6f8712c3"
        },
        "pool_id": "ff8080825ab738f4015ab7513298010e",
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
        "zone_type": "private",
        "created_at": "2017-04-22T08:17:08.997",
        "updated_at": "2017-04-22T08:17:10.849",
        "record_num": 2,
        "routers": {
            "status": "PENDING_CREATE",
            "router_id": "19664294-0bf6-4271-ad3a-94b8c79c6558",
            "router_region": "xx"
        }
    }
    
    ```


## 返回值<a name="section1917896317411"></a>

请参考[通用请求返回值](通用请求返回值.md)。

