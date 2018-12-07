# 查询公网Zone列表<a name="ZH-CN_TOPIC_0037134402"></a>

## 功能介绍<a name="section2763065016101"></a>

查询公网Zone的列表。

## URI<a name="section53701671161015"></a>

GET /v2/zones?type=\{type\}&limit=\{limit\}&marker=\{marker\}&offset=\{offset\}&tags=\{tags\}

参数说明请参见[表1](#table36421405182556)。

**表 1**  URI格式的参数说明

<a name="table36421405182556"></a>
<table><thead align="left"><tr id="row35113810182556"><th class="cellrowborder" valign="top" width="12.78%" id="mcps1.2.5.1.1"><p id="p29205341182624"><a name="p29205341182624"></a><a name="p29205341182624"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.219999999999999%" id="mcps1.2.5.1.2"><p id="p16822416182624"><a name="p16822416182624"></a><a name="p16822416182624"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.600000000000001%" id="mcps1.2.5.1.3"><p id="p20438464182624"><a name="p20438464182624"></a><a name="p20438464182624"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="59.4%" id="mcps1.2.5.1.4"><p id="p44902868182624"><a name="p44902868182624"></a><a name="p44902868182624"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7883687182556"><td class="cellrowborder" valign="top" width="12.78%" headers="mcps1.2.5.1.1 "><p id="p29178851182717"><a name="p29178851182717"></a><a name="p29178851182717"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="14.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p2590622182717"><a name="p2590622182717"></a><a name="p2590622182717"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.600000000000001%" headers="mcps1.2.5.1.3 "><p id="p66359104182717"><a name="p66359104182717"></a><a name="p66359104182717"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="59.4%" headers="mcps1.2.5.1.4 "><p id="p53225083153722"><a name="p53225083153722"></a><a name="p53225083153722"></a>待查询的zone的类型。</p>
<p id="p4877093182943"><a name="p4877093182943"></a><a name="p4877093182943"></a>取值范围：public、private</p>
<a name="ul7470137153957"></a><a name="ul7470137153957"></a><ul id="ul7470137153957"><li>如果为空，表示查询公网类型的zone。</li><li>如果为public，表示查询公网类型的zone。</li><li>如果为private，表示查询内网类型的zone。</li></ul>
</td>
</tr>
<tr id="row12208459182556"><td class="cellrowborder" valign="top" width="12.78%" headers="mcps1.2.5.1.1 "><p id="p17456213182720"><a name="p17456213182720"></a><a name="p17456213182720"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="14.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p4667185182720"><a name="p4667185182720"></a><a name="p4667185182720"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.600000000000001%" headers="mcps1.2.5.1.3 "><p id="p42497672182720"><a name="p42497672182720"></a><a name="p42497672182720"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="59.4%" headers="mcps1.2.5.1.4 "><p id="p19759428182720"><a name="p19759428182720"></a><a name="p19759428182720"></a>分页查询起始的资源ID，为空时为查询第一页。</p>
</td>
</tr>
<tr id="row29489517182630"><td class="cellrowborder" valign="top" width="12.78%" headers="mcps1.2.5.1.1 "><p id="p43326778182720"><a name="p43326778182720"></a><a name="p43326778182720"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="14.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p19808096182720"><a name="p19808096182720"></a><a name="p19808096182720"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.600000000000001%" headers="mcps1.2.5.1.3 "><p id="p60951943182720"><a name="p60951943182720"></a><a name="p60951943182720"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="59.4%" headers="mcps1.2.5.1.4 "><a name="ul38160342182720"></a><a name="ul38160342182720"></a><ul id="ul38160342182720"><li>取值范围：0~500<p id="p3980022182720"><a name="p3980022182720"></a><a name="p3980022182720"></a>取值一般为10，20，50</p>
</li><li>功能说明：每页返回的资源个数。</li></ul>
</td>
</tr>
<tr id="row56409238193951"><td class="cellrowborder" valign="top" width="12.78%" headers="mcps1.2.5.1.1 "><p id="p5745576193951"><a name="p5745576193951"></a><a name="p5745576193951"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="14.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p62738535193951"><a name="p62738535193951"></a><a name="p62738535193951"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.600000000000001%" headers="mcps1.2.5.1.3 "><p id="p48656570193951"><a name="p48656570193951"></a><a name="p48656570193951"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="59.4%" headers="mcps1.2.5.1.4 "><a name="ul35486924194016"></a><a name="ul35486924194016"></a><ul id="ul35486924194016"><li>取值范围：0~2147483647</li><li>分页查询起始页码，起始值为0。当前设置marker不为空时，以marker为分页起始标识。</li></ul>
</td>
</tr>
<tr id="row1736769311550"><td class="cellrowborder" valign="top" width="12.78%" headers="mcps1.2.5.1.1 "><p id="p1821826211550"><a name="p1821826211550"></a><a name="p1821826211550"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="14.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p6639315411550"><a name="p6639315411550"></a><a name="p6639315411550"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.600000000000001%" headers="mcps1.2.5.1.3 "><p id="p913636111550"><a name="p913636111550"></a><a name="p913636111550"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="59.4%" headers="mcps1.2.5.1.4 "><p id="p28691609115519"><a name="p28691609115519"></a><a name="p28691609115519"></a>资源标签。</p>
<p id="p6833525115523"><a name="p6833525115523"></a><a name="p6833525115523"></a>取值格式：key1,value1|key2,value2</p>
<p id="p32051112114146"><a name="p32051112114146"></a><a name="p32051112114146"></a>多个标签之间用"|"分开，每个标签的键值用英文逗号","相隔。</p>
<p id="p15239506115938"><a name="p15239506115938"></a><a name="p15239506115938"></a>多个标签之间为“与”的关系。</p>
<p id="p39866681115027"><a name="p39866681115027"></a><a name="p39866681115027"></a>关于资源标签，请参见<a href="添加资源标签.md">添加资源标签</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section44958995161021"></a>

无

## 响应<a name="section40090803161031"></a>

-   要素说明

    **表 2**  响应样例的要素说明

    <a name="table6655637171923"></a>
    <table><thead align="left"><tr id="row12436182171923"><th class="cellrowborder" valign="top" width="18.529999999999998%" id="mcps1.2.4.1.1"><p id="p18040723171923"><a name="p18040723171923"></a><a name="p18040723171923"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.45%" id="mcps1.2.4.1.2"><p id="p12288867171923"><a name="p12288867171923"></a><a name="p12288867171923"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.019999999999996%" id="mcps1.2.4.1.3"><p id="p16021685171923"><a name="p16021685171923"></a><a name="p16021685171923"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row33084878171923"><td class="cellrowborder" valign="top" width="18.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p10518479171923"><a name="p10518479171923"></a><a name="p10518479171923"></a>zones</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.45%" headers="mcps1.2.4.1.2 "><p id="p17816324171923"><a name="p17816324171923"></a><a name="p17816324171923"></a>列表数据结构</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.019999999999996%" headers="mcps1.2.4.1.3 "><p id="p64387025171923"><a name="p64387025171923"></a><a name="p64387025171923"></a>zone列表对象。</p>
    </td>
    </tr>
    <tr id="row45921614175143"><td class="cellrowborder" valign="top" width="18.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p10641344175143"><a name="p10641344175143"></a><a name="p10641344175143"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.45%" headers="mcps1.2.4.1.2 "><p id="p24643947175143"><a name="p24643947175143"></a><a name="p24643947175143"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.019999999999996%" headers="mcps1.2.4.1.3 "><p id="p50002691175143"><a name="p50002691175143"></a><a name="p50002691175143"></a>返回满足过滤条件的资源总数。</p>
    </td>
    </tr>
    </tbody>
    </table>

    其中，[表2](#table6655637171923)中的zones参数说明，请参见[表3](#table6348803417233)；metadata参数说明，请参见[表4](#table52442344175457)。 

    **表 3**  zones参数说明

    <a name="table6348803417233"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0037139748_row54125868171039"><th class="cellrowborder" valign="top" width="18.37%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0037139748_p46128019171039"><a name="zh-cn_topic_0037139748_p46128019171039"></a><a name="zh-cn_topic_0037139748_p46128019171039"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.39%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0037139748_p61288737171039"><a name="zh-cn_topic_0037139748_p61288737171039"></a><a name="zh-cn_topic_0037139748_p61288737171039"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.239999999999995%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0037139748_p39427830171039"><a name="zh-cn_topic_0037139748_p39427830171039"></a><a name="zh-cn_topic_0037139748_p39427830171039"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0037139748_row3275315171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p13677558171039"><a name="zh-cn_topic_0037139748_p13677558171039"></a><a name="zh-cn_topic_0037139748_p13677558171039"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p31480160171039"><a name="zh-cn_topic_0037139748_p31480160171039"></a><a name="zh-cn_topic_0037139748_p31480160171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p55186322171039"><a name="zh-cn_topic_0037139748_p55186322171039"></a><a name="zh-cn_topic_0037139748_p55186322171039"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037139748_row62038903171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p21725743171039"><a name="zh-cn_topic_0037139748_p21725743171039"></a><a name="zh-cn_topic_0037139748_p21725743171039"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p55078653171039"><a name="zh-cn_topic_0037139748_p55078653171039"></a><a name="zh-cn_topic_0037139748_p55078653171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p65545475171039"><a name="zh-cn_topic_0037139748_p65545475171039"></a><a name="zh-cn_topic_0037139748_p65545475171039"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037139748_row24663709171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p56112529171039"><a name="zh-cn_topic_0037139748_p56112529171039"></a><a name="zh-cn_topic_0037139748_p56112529171039"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p46656524171039"><a name="zh-cn_topic_0037139748_p46656524171039"></a><a name="zh-cn_topic_0037139748_p46656524171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p31778607171039"><a name="zh-cn_topic_0037139748_p31778607171039"></a><a name="zh-cn_topic_0037139748_p31778607171039"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037139748_row34212800171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p51657401171039"><a name="zh-cn_topic_0037139748_p51657401171039"></a><a name="zh-cn_topic_0037139748_p51657401171039"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p336297171039"><a name="zh-cn_topic_0037139748_p336297171039"></a><a name="zh-cn_topic_0037139748_p336297171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p66322352171039"><a name="zh-cn_topic_0037139748_p66322352171039"></a><a name="zh-cn_topic_0037139748_p66322352171039"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037139748_row45341886171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p22374403171039"><a name="zh-cn_topic_0037139748_p22374403171039"></a><a name="zh-cn_topic_0037139748_p22374403171039"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p16323247171039"><a name="zh-cn_topic_0037139748_p16323247171039"></a><a name="zh-cn_topic_0037139748_p16323247171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p58527202171039"><a name="zh-cn_topic_0037139748_p58527202171039"></a><a name="zh-cn_topic_0037139748_p58527202171039"></a>zone类型，公网或者内网。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037139748_row36905265171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p4888971171039"><a name="zh-cn_topic_0037139748_p4888971171039"></a><a name="zh-cn_topic_0037139748_p4888971171039"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p16027579171039"><a name="zh-cn_topic_0037139748_p16027579171039"></a><a name="zh-cn_topic_0037139748_p16027579171039"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p41240291171039"><a name="zh-cn_topic_0037139748_p41240291171039"></a><a name="zh-cn_topic_0037139748_p41240291171039"></a>该zone下SOA记录中的ttl值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037139748_row29641334171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p63311148171039"><a name="zh-cn_topic_0037139748_p63311148171039"></a><a name="zh-cn_topic_0037139748_p63311148171039"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p26678057171039"><a name="zh-cn_topic_0037139748_p26678057171039"></a><a name="zh-cn_topic_0037139748_p26678057171039"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p7524749171039"><a name="zh-cn_topic_0037139748_p7524749171039"></a><a name="zh-cn_topic_0037139748_p7524749171039"></a>该zone下SOA记录中用于标识变更的序列值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037139748_row44990376171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p30244483171039"><a name="zh-cn_topic_0037139748_p30244483171039"></a><a name="zh-cn_topic_0037139748_p30244483171039"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p47406357171039"><a name="zh-cn_topic_0037139748_p47406357171039"></a><a name="zh-cn_topic_0037139748_p47406357171039"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p9822846171039"><a name="zh-cn_topic_0037139748_p9822846171039"></a><a name="zh-cn_topic_0037139748_p9822846171039"></a>资源状态。</p>
    <p id="zh-cn_topic_0037139748_p36239781171039"><a name="zh-cn_topic_0037139748_p36239781171039"></a><a name="zh-cn_topic_0037139748_p36239781171039"></a>取值范围：PENDING_CREATE, ACTIVE, PENDING_DELETE, ERROR。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037139748_row1454557171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p51202644171039"><a name="zh-cn_topic_0037139748_p51202644171039"></a><a name="zh-cn_topic_0037139748_p51202644171039"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p32016130171039"><a name="zh-cn_topic_0037139748_p32016130171039"></a><a name="zh-cn_topic_0037139748_p32016130171039"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p53878535171039"><a name="zh-cn_topic_0037139748_p53878535171039"></a><a name="zh-cn_topic_0037139748_p53878535171039"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037139748_row48476716171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p54136527171039"><a name="zh-cn_topic_0037139748_p54136527171039"></a><a name="zh-cn_topic_0037139748_p54136527171039"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p48020249171039"><a name="zh-cn_topic_0037139748_p48020249171039"></a><a name="zh-cn_topic_0037139748_p48020249171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p63987755171039"><a name="zh-cn_topic_0037139748_p63987755171039"></a><a name="zh-cn_topic_0037139748_p63987755171039"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037139748_row49967872171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p35791512171039"><a name="zh-cn_topic_0037139748_p35791512171039"></a><a name="zh-cn_topic_0037139748_p35791512171039"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p10454086171039"><a name="zh-cn_topic_0037139748_p10454086171039"></a><a name="zh-cn_topic_0037139748_p10454086171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p8704812171039"><a name="zh-cn_topic_0037139748_p8704812171039"></a><a name="zh-cn_topic_0037139748_p8704812171039"></a>zone所属的租户ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037139748_row27690345171039"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p48529730171039"><a name="zh-cn_topic_0037139748_p48529730171039"></a><a name="zh-cn_topic_0037139748_p48529730171039"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p59988242171039"><a name="zh-cn_topic_0037139748_p59988242171039"></a><a name="zh-cn_topic_0037139748_p59988242171039"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p9292793171039"><a name="zh-cn_topic_0037139748_p9292793171039"></a><a name="zh-cn_topic_0037139748_p9292793171039"></a>创建时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037139748_row4377608115654"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p5844041115654"><a name="zh-cn_topic_0037139748_p5844041115654"></a><a name="zh-cn_topic_0037139748_p5844041115654"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p3605288915654"><a name="zh-cn_topic_0037139748_p3605288915654"></a><a name="zh-cn_topic_0037139748_p3605288915654"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p3460290715654"><a name="zh-cn_topic_0037139748_p3460290715654"></a><a name="zh-cn_topic_0037139748_p3460290715654"></a>更新时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037139748_row384676871572"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p288749251572"><a name="zh-cn_topic_0037139748_p288749251572"></a><a name="zh-cn_topic_0037139748_p288749251572"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p571676251572"><a name="zh-cn_topic_0037139748_p571676251572"></a><a name="zh-cn_topic_0037139748_p571676251572"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p660161572"><a name="zh-cn_topic_0037139748_p660161572"></a><a name="zh-cn_topic_0037139748_p660161572"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037139748_row177328815945"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p1595959815945"><a name="zh-cn_topic_0037139748_p1595959815945"></a><a name="zh-cn_topic_0037139748_p1595959815945"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p1765902715945"><a name="zh-cn_topic_0037139748_p1765902715945"></a><a name="zh-cn_topic_0037139748_p1765902715945"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.239999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p2109506015945"><a name="zh-cn_topic_0037139748_p2109506015945"></a><a name="zh-cn_topic_0037139748_p2109506015945"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  metadata参数说明

    <a name="table52442344175457"></a>
    <table><thead align="left"><tr id="row58979189175457"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p46156243175457"><a name="p46156243175457"></a><a name="p46156243175457"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p47668234175457"><a name="p47668234175457"></a><a name="p47668234175457"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p35921708175457"><a name="p35921708175457"></a><a name="p35921708175457"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row54859922175457"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p14468674175457"><a name="p14468674175457"></a><a name="p14468674175457"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p31111955175457"><a name="p31111955175457"></a><a name="p31111955175457"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p37040428175457"><a name="p37040428175457"></a><a name="p37040428175457"></a>资源总数</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "links": {
            "self": "https://Endpoint/v2/zones?type=public&limit=11&marker=&name=&status="
        },
        "zones": [
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
            },
            {
                "id": "2c9eb155587228570158722996c50001",
                "name": "example.org.",
                "description": "This is an example zone.",
                "email": "xx@example.org",
                "ttl": 300,
                "serial": 0,
                "masters": [],
                "status": "PENDING_CREATE",
                "links": {
                    "self": "https://Endpoint/v2/zones/2c9eb155587228570158722996c50001"
                },
                "pool_id": "00000000570e54ee01570e9939b20019",
                "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c",
                "zone_type": "public",
                "created_at": "2016-11-17T12:01:17.996",
                "updated_at": "2016-11-17T12:01:18.528",
                "record_num": 2
            }
        ],
        "metadata": {
            "total_count": 2
        }
    }
    
    ```


## 返回值<a name="section42637797161043"></a>

请参考[通用请求返回值](通用请求返回值.md)。

