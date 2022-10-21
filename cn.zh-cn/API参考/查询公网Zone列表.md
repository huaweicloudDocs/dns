# 查询公网Zone列表<a name="dns_api_62003"></a>

## 功能介绍<a name="section2763065016101"></a>

查询公网Zone的列表。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=DNS&api=ListPublicZones)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI<a name="section53701671161015"></a>

GET /v2/zones

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
<td class="cellrowborder" valign="top" width="13.600000000000001%" headers="mcps1.2.5.1.3 "><p id="p66359104182717"><a name="p66359104182717"></a><a name="p66359104182717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59.4%" headers="mcps1.2.5.1.4 "><p id="p53225083153722"><a name="p53225083153722"></a><a name="p53225083153722"></a>待查询的zone的类型。</p>
<p id="p4877093182943"><a name="p4877093182943"></a><a name="p4877093182943"></a>取值范围：public、private</p>
<a name="ul7470137153957"></a><a name="ul7470137153957"></a><ul id="ul7470137153957"><li>如果为空，表示查询公网类型的zone。</li><li>如果为public，表示查询公网类型的zone。</li><li>如果为private，表示查询内网类型的zone。</li></ul>
<p id="p12624433152816"><a name="p12624433152816"></a><a name="p12624433152816"></a>搜索模式默认为模糊搜索。</p>
<p id="p23756351441"><a name="p23756351441"></a><a name="p23756351441"></a>默认值为空。</p>
</td>
</tr>
<tr id="row12208459182556"><td class="cellrowborder" valign="top" width="12.78%" headers="mcps1.2.5.1.1 "><p id="p17456213182720"><a name="p17456213182720"></a><a name="p17456213182720"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="14.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p4667185182720"><a name="p4667185182720"></a><a name="p4667185182720"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.600000000000001%" headers="mcps1.2.5.1.3 "><p id="p42497672182720"><a name="p42497672182720"></a><a name="p42497672182720"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59.4%" headers="mcps1.2.5.1.4 "><p id="p19759428182720"><a name="p19759428182720"></a><a name="p19759428182720"></a>分页查询起始的资源ID，为空时为查询第一页。</p>
</td>
</tr>
<tr id="row29489517182630"><td class="cellrowborder" valign="top" width="12.78%" headers="mcps1.2.5.1.1 "><p id="p43326778182720"><a name="p43326778182720"></a><a name="p43326778182720"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="14.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p19808096182720"><a name="p19808096182720"></a><a name="p19808096182720"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.600000000000001%" headers="mcps1.2.5.1.3 "><p id="p60951943182720"><a name="p60951943182720"></a><a name="p60951943182720"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="59.4%" headers="mcps1.2.5.1.4 "><p id="p230120311413"><a name="p230120311413"></a><a name="p230120311413"></a>每页返回的资源个数。</p>
<p id="p147131447514"><a name="p147131447514"></a><a name="p147131447514"></a>取值范围：0~500</p>
<p id="p1385813431412"><a name="p1385813431412"></a><a name="p1385813431412"></a>取值一般为10，20，50。默认值为500。</p>
</td>
</tr>
<tr id="row56409238193951"><td class="cellrowborder" valign="top" width="12.78%" headers="mcps1.2.5.1.1 "><p id="p5745576193951"><a name="p5745576193951"></a><a name="p5745576193951"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="14.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p62738535193951"><a name="p62738535193951"></a><a name="p62738535193951"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.600000000000001%" headers="mcps1.2.5.1.3 "><p id="p48656570193951"><a name="p48656570193951"></a><a name="p48656570193951"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="59.4%" headers="mcps1.2.5.1.4 "><p id="p35951433204916"><a name="p35951433204916"></a><a name="p35951433204916"></a>分页查询起始偏移量，表示从偏移量的下一个资源开始查询。</p>
<p id="p18898143914915"><a name="p18898143914915"></a><a name="p18898143914915"></a>取值范围：0-2147483647</p>
<p id="p13209172234718"><a name="p13209172234718"></a><a name="p13209172234718"></a>默认值为0。</p>
<p id="p167712216335"><a name="p167712216335"></a><a name="p167712216335"></a>当前设置marker不为空时，以marker为分页起始标识。</p>
</td>
</tr>
<tr id="row1736769311550"><td class="cellrowborder" valign="top" width="12.78%" headers="mcps1.2.5.1.1 "><p id="p1821826211550"><a name="p1821826211550"></a><a name="p1821826211550"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="14.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p6639315411550"><a name="p6639315411550"></a><a name="p6639315411550"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.600000000000001%" headers="mcps1.2.5.1.3 "><p id="p913636111550"><a name="p913636111550"></a><a name="p913636111550"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59.4%" headers="mcps1.2.5.1.4 "><p id="p28691609115519"><a name="p28691609115519"></a><a name="p28691609115519"></a>资源标签。</p>
<p id="p6833525115523"><a name="p6833525115523"></a><a name="p6833525115523"></a>取值格式：key1,value1|key2,value2</p>
<p id="p32051112114146"><a name="p32051112114146"></a><a name="p32051112114146"></a>多个标签之间用"|"分开，每个标签的键值用英文逗号","相隔。</p>
<p id="p15239506115938"><a name="p15239506115938"></a><a name="p15239506115938"></a>多个标签之间为“与”的关系。</p>
<p id="p39866681115027"><a name="p39866681115027"></a><a name="p39866681115027"></a>关于资源标签，请参见<a href="添加资源标签.md">添加资源标签</a>。</p>
<p id="p12571115182919"><a name="p12571115182919"></a><a name="p12571115182919"></a>搜索模式为精确搜索。如果资源标签值value是以*开头时，则按照*后面的值全模糊匹配。</p>
<p id="p10621449102913"><a name="p10621449102913"></a><a name="p10621449102913"></a>默认值为空。</p>
</td>
</tr>
<tr id="row1633012241220"><td class="cellrowborder" valign="top" width="12.78%" headers="mcps1.2.5.1.1 "><p id="p1933113222124"><a name="p1933113222124"></a><a name="p1933113222124"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p1833110221120"><a name="p1833110221120"></a><a name="p1833110221120"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.600000000000001%" headers="mcps1.2.5.1.3 "><p id="p1533162211129"><a name="p1533162211129"></a><a name="p1533162211129"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59.4%" headers="mcps1.2.5.1.4 "><p id="p113313225126"><a name="p113313225126"></a><a name="p113313225126"></a>zone名称。</p>
<p id="p159771524568"><a name="p159771524568"></a><a name="p159771524568"></a>搜索模式默认为模糊搜索。</p>
</td>
</tr>
<tr id="row1173792401616"><td class="cellrowborder" valign="top" width="12.78%" headers="mcps1.2.5.1.1 "><p id="p6738102411167"><a name="p6738102411167"></a><a name="p6738102411167"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="14.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p973842401614"><a name="p973842401614"></a><a name="p973842401614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.600000000000001%" headers="mcps1.2.5.1.3 "><p id="p1173872481613"><a name="p1173872481613"></a><a name="p1173872481613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59.4%" headers="mcps1.2.5.1.4 "><p id="p08895418160"><a name="p08895418160"></a><a name="p08895418160"></a>资源状态。</p>
<p id="p168892041161615"><a name="p168892041161615"></a><a name="p168892041161615"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
</td>
</tr>
<tr id="row193191414415"><td class="cellrowborder" valign="top" width="12.78%" headers="mcps1.2.5.1.1 "><p id="p183195412449"><a name="p183195412449"></a><a name="p183195412449"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.219999999999999%" headers="mcps1.2.5.1.2 "><p id="p1331912410447"><a name="p1331912410447"></a><a name="p1331912410447"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.600000000000001%" headers="mcps1.2.5.1.3 "><p id="p123191947448"><a name="p123191947448"></a><a name="p123191947448"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59.4%" headers="mcps1.2.5.1.4 "><p id="p1331920410444"><a name="p1331920410444"></a><a name="p1331920410444"></a>域名关联的企业项目ID，长度不超过36个字符。</p>
<p id="p131131925172318"><a name="p131131925172318"></a><a name="p131131925172318"></a>默认值为0。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section44958995161021"></a>

-   请求参数

    无

-   请求样例

    查询域名类型为公网，且资源标签键为key1、值为value1的前10个域名。

    ```
    GET https://{DNS_Endpoint}/v2/zones?type=public&limit=10&offset=0&tags=key1,value1
    ```


## 响应<a name="section40090803161031"></a>

-   要素说明

    **表 2**  响应样例的要素说明

    <a name="table6655637171923"></a>
    <table><thead align="left"><tr id="row12436182171923"><th class="cellrowborder" valign="top" width="18.529999999999998%" id="mcps1.2.4.1.1"><p id="p18040723171923"><a name="p18040723171923"></a><a name="p18040723171923"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.970000000000002%" id="mcps1.2.4.1.2"><p id="p12288867171923"><a name="p12288867171923"></a><a name="p12288867171923"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.5%" id="mcps1.2.4.1.3"><p id="p16021685171923"><a name="p16021685171923"></a><a name="p16021685171923"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1313962617109"><td class="cellrowborder" valign="top" width="18.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p1122192813108"><a name="p1122192813108"></a><a name="p1122192813108"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.970000000000002%" headers="mcps1.2.4.1.2 "><p id="p1222152817106"><a name="p1222152817106"></a><a name="p1222152817106"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.5%" headers="mcps1.2.4.1.3 "><p id="p9225286109"><a name="p9225286109"></a><a name="p9225286109"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p222428171017"><a name="p222428171017"></a><a name="p222428171017"></a>详细信息请参见<a href="#table0172144213344">表5</a>。</p>
    </td>
    </tr>
    <tr id="row33084878171923"><td class="cellrowborder" valign="top" width="18.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p10518479171923"><a name="p10518479171923"></a><a name="p10518479171923"></a>zones</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.970000000000002%" headers="mcps1.2.4.1.2 "><p id="p17816324171923"><a name="p17816324171923"></a><a name="p17816324171923"></a>Array of object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.5%" headers="mcps1.2.4.1.3 "><p id="p64387025171923"><a name="p64387025171923"></a><a name="p64387025171923"></a>zone列表对象，详细内容请参见<a href="#table6348803417233">表3</a>。</p>
    </td>
    </tr>
    <tr id="row45921614175143"><td class="cellrowborder" valign="top" width="18.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p10641344175143"><a name="p10641344175143"></a><a name="p10641344175143"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.970000000000002%" headers="mcps1.2.4.1.2 "><p id="p24643947175143"><a name="p24643947175143"></a><a name="p24643947175143"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.5%" headers="mcps1.2.4.1.3 "><p id="p50002691175143"><a name="p50002691175143"></a><a name="p50002691175143"></a>返回满足过滤条件的资源总数，详细内容请参见<a href="#table52442344175457">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  zones参数说明

    <a name="table6348803417233"></a>
    <table><thead align="left"><tr id="r23fa2da9911a4ee5a769290a0a199439"><th class="cellrowborder" valign="top" width="18.37%" id="mcps1.2.4.1.1"><p id="ab37e0c953c5e4c9f825ae513b4e7be64"><a name="ab37e0c953c5e4c9f825ae513b4e7be64"></a><a name="ab37e0c953c5e4c9f825ae513b4e7be64"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.41%" id="mcps1.2.4.1.2"><p id="acf116b883bc84e0dbdb0aba866af0983"><a name="acf116b883bc84e0dbdb0aba866af0983"></a><a name="acf116b883bc84e0dbdb0aba866af0983"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.22%" id="mcps1.2.4.1.3"><p id="afc0cd2e5779b4d6aad0629b35d87cfe5"><a name="afc0cd2e5779b4d6aad0629b35d87cfe5"></a><a name="afc0cd2e5779b4d6aad0629b35d87cfe5"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r06a7dd0ecc294dc6882fa08829fe0604"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a4932676eab7a4ea09e37b9ad2db58d31"><a name="a4932676eab7a4ea09e37b9ad2db58d31"></a><a name="a4932676eab7a4ea09e37b9ad2db58d31"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="a4239fa13387042118443b35b50304e4a"><a name="a4239fa13387042118443b35b50304e4a"></a><a name="a4239fa13387042118443b35b50304e4a"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="a6d1b608635744cd292ef147bfd8d3920"><a name="a6d1b608635744cd292ef147bfd8d3920"></a><a name="a6d1b608635744cd292ef147bfd8d3920"></a>zone的ID，uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="r9c08eb7520d44ce98644f20f1655f1c1"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="aefad392b710e479597345abba93e82fa"><a name="aefad392b710e479597345abba93e82fa"></a><a name="aefad392b710e479597345abba93e82fa"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="a696a900fa4654809880ea1ce0fc0f561"><a name="a696a900fa4654809880ea1ce0fc0f561"></a><a name="a696a900fa4654809880ea1ce0fc0f561"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="a5f80a18701844c989e2439936c0652a3"><a name="a5f80a18701844c989e2439936c0652a3"></a><a name="a5f80a18701844c989e2439936c0652a3"></a>zone名称。</p>
    </td>
    </tr>
    <tr id="r6b77005ed4224ea0b410678e7912fc97"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="ac6590fa69311427898e8170c48b8fa39"><a name="ac6590fa69311427898e8170c48b8fa39"></a><a name="ac6590fa69311427898e8170c48b8fa39"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="adf1b2bc2172e496289cfff6aa994a331"><a name="adf1b2bc2172e496289cfff6aa994a331"></a><a name="adf1b2bc2172e496289cfff6aa994a331"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="a2341f4ef85b34a8cad2372164c6686eb"><a name="a2341f4ef85b34a8cad2372164c6686eb"></a><a name="a2341f4ef85b34a8cad2372164c6686eb"></a>对zone的描述信息。</p>
    </td>
    </tr>
    <tr id="rfdd59b39416a4adc9a8103df0224e716"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a30a87e7422dd4c5cbf5c8b4bbf2a84d8"><a name="a30a87e7422dd4c5cbf5c8b4bbf2a84d8"></a><a name="a30a87e7422dd4c5cbf5c8b4bbf2a84d8"></a>email</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p336297171039"><a name="zh-cn_topic_0037139748_p336297171039"></a><a name="zh-cn_topic_0037139748_p336297171039"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="a791ad8d88187434094a0eed0a3cbbfb2"><a name="a791ad8d88187434094a0eed0a3cbbfb2"></a><a name="a791ad8d88187434094a0eed0a3cbbfb2"></a>管理该zone的管理员邮箱。</p>
    </td>
    </tr>
    <tr id="r65ed8e5dbe574f5ba73cfb6177c74d51"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a586a45dbdef8419e8fc848941eaa1aa9"><a name="a586a45dbdef8419e8fc848941eaa1aa9"></a><a name="a586a45dbdef8419e8fc848941eaa1aa9"></a>zone_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="a0f2f0d5daa7b46d5b4e611831fd0c4a8"><a name="a0f2f0d5daa7b46d5b4e611831fd0c4a8"></a><a name="a0f2f0d5daa7b46d5b4e611831fd0c4a8"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="a13ac59b267154f24b2d096be4c229e62"><a name="a13ac59b267154f24b2d096be4c229e62"></a><a name="a13ac59b267154f24b2d096be4c229e62"></a>zone类型，公网（public）或者内网（private）。</p>
    </td>
    </tr>
    <tr id="rf50e52f024aa428ca2324bdb3719bb1c"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a8a3f46292b0c4874898c63b7a6f80926"><a name="a8a3f46292b0c4874898c63b7a6f80926"></a><a name="a8a3f46292b0c4874898c63b7a6f80926"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="aafbde4a45c94452aa4ec4e4c0ab151ba"><a name="aafbde4a45c94452aa4ec4e4c0ab151ba"></a><a name="aafbde4a45c94452aa4ec4e4c0ab151ba"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="a10f5e4e2602f4350a2ccfc124a018d34"><a name="a10f5e4e2602f4350a2ccfc124a018d34"></a><a name="a10f5e4e2602f4350a2ccfc124a018d34"></a>该zone下SOA记录中的ttl值。</p>
    <p id="p0662131993410"><a name="p0662131993410"></a><a name="p0662131993410"></a>取值范围：1~2147483647。</p>
    <p id="p7662111973418"><a name="p7662111973418"></a><a name="p7662111973418"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="r6b4647120ecf46eaa33b673e28839d15"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="aebeb87bd362d4a3faacb6ca919e3981e"><a name="aebeb87bd362d4a3faacb6ca919e3981e"></a><a name="aebeb87bd362d4a3faacb6ca919e3981e"></a>serial</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="a9748d8daa2f947f8921f68add4e991c0"><a name="a9748d8daa2f947f8921f68add4e991c0"></a><a name="a9748d8daa2f947f8921f68add4e991c0"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="p1499913459428"><a name="p1499913459428"></a><a name="p1499913459428"></a>该zone下SOA记录中用于标识zone文件变更的序列值，用于主从节点同步。</p>
    <p id="p7524749171039"><a name="p7524749171039"></a><a name="p7524749171039"></a>该参数暂未使用。</p>
    </td>
    </tr>
    <tr id="re8c33e9c430e41e88b42b9ceb94d5803"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="aaf10dc2c1ac64fc5a3da7078cb0596a6"><a name="aaf10dc2c1ac64fc5a3da7078cb0596a6"></a><a name="aaf10dc2c1ac64fc5a3da7078cb0596a6"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="a687065e2ff0d46e98e1b2942fe23bc3a"><a name="a687065e2ff0d46e98e1b2942fe23bc3a"></a><a name="a687065e2ff0d46e98e1b2942fe23bc3a"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="a1bee5fd6826345c1aee2af7b2b331937"><a name="a1bee5fd6826345c1aee2af7b2b331937"></a><a name="a1bee5fd6826345c1aee2af7b2b331937"></a>资源状态。</p>
    <p id="p15991203153020"><a name="p15991203153020"></a><a name="p15991203153020"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="r80c4f22c27124b56b9f9ee0679394c42"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="aeb15dbe32b604c1fb0ecae447c204c29"><a name="aeb15dbe32b604c1fb0ecae447c204c29"></a><a name="aeb15dbe32b604c1fb0ecae447c204c29"></a>record_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="ae5c55f656d2f4ee8985921f3c83f738e"><a name="ae5c55f656d2f4ee8985921f3c83f738e"></a><a name="ae5c55f656d2f4ee8985921f3c83f738e"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="a9cb01b7b03184775b5c98e48b1b3426a"><a name="a9cb01b7b03184775b5c98e48b1b3426a"></a><a name="a9cb01b7b03184775b5c98e48b1b3426a"></a>该zone下的recordset个数。</p>
    </td>
    </tr>
    <tr id="rf994e423aff545899ef9c353685756ff"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a87487f19552d4c12a0ad956bccaa7998"><a name="a87487f19552d4c12a0ad956bccaa7998"></a><a name="a87487f19552d4c12a0ad956bccaa7998"></a>pool_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="adb93a67b81d342d19c3509b6bb845745"><a name="adb93a67b81d342d19c3509b6bb845745"></a><a name="adb93a67b81d342d19c3509b6bb845745"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="aaccbb6eaeed64b7096678ae8a7c87e24"><a name="aaccbb6eaeed64b7096678ae8a7c87e24"></a><a name="aaccbb6eaeed64b7096678ae8a7c87e24"></a>托管该zone的pool，由系统分配。</p>
    </td>
    </tr>
    <tr id="r60fa51885e2d4d01bd7d47db1ff3bfdd"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="afdd30b1a51354b639ce164b115df339e"><a name="afdd30b1a51354b639ce164b115df339e"></a><a name="afdd30b1a51354b639ce164b115df339e"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="a06917a7a64fa4de693aeb5442109be96"><a name="a06917a7a64fa4de693aeb5442109be96"></a><a name="a06917a7a64fa4de693aeb5442109be96"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="p8704812171039"><a name="p8704812171039"></a><a name="p8704812171039"></a>zone所属的项目ID。</p>
    </td>
    </tr>
    <tr id="ra456600e26214cdcbfedd7e42f4a9d73"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a329645c1cf924ea0b3258c9b67f35b59"><a name="a329645c1cf924ea0b3258c9b67f35b59"></a><a name="a329645c1cf924ea0b3258c9b67f35b59"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="a25d2495f1d28446b8e57250347024ecf"><a name="a25d2495f1d28446b8e57250347024ecf"></a><a name="a25d2495f1d28446b8e57250347024ecf"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="a3c499e0e732e4eedb2b900eed39a86eb"><a name="a3c499e0e732e4eedb2b900eed39a86eb"></a><a name="a3c499e0e732e4eedb2b900eed39a86eb"></a>创建时间。</p>
    <p id="p16471913102410"><a name="p16471913102410"></a><a name="p16471913102410"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="rf0243379fed8476db1f06e6d2d0d1479"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="a90b33cdf2e7048d9a2c4dbb5a0021423"><a name="a90b33cdf2e7048d9a2c4dbb5a0021423"></a><a name="a90b33cdf2e7048d9a2c4dbb5a0021423"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="a2f7e47e730f9408ebde639a3e1b65f22"><a name="a2f7e47e730f9408ebde639a3e1b65f22"></a><a name="a2f7e47e730f9408ebde639a3e1b65f22"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="acdf6059b171f4930a800e842b314166f"><a name="acdf6059b171f4930a800e842b314166f"></a><a name="acdf6059b171f4930a800e842b314166f"></a>更新时间。</p>
    <p id="p465420187241"><a name="p465420187241"></a><a name="p465420187241"></a>采用UTC时间格式，格式为：YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="r0eebfd448d94450db6310faee3858418"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037139748_p288749251572"><a name="zh-cn_topic_0037139748_p288749251572"></a><a name="zh-cn_topic_0037139748_p288749251572"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037139748_p571676251572"><a name="zh-cn_topic_0037139748_p571676251572"></a><a name="zh-cn_topic_0037139748_p571676251572"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037139748_p660161572"><a name="zh-cn_topic_0037139748_p660161572"></a><a name="zh-cn_topic_0037139748_p660161572"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p14741433184311"><a name="p14741433184311"></a><a name="p14741433184311"></a>详细信息请参见<a href="#table0172144213344">表5</a>。</p>
    </td>
    </tr>
    <tr id="row56817311274"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p145019941317"><a name="p145019941317"></a><a name="p145019941317"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="p75011918138"><a name="p75011918138"></a><a name="p75011918138"></a>Array of <a href="#table619059185111">tag</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="p1350114961316"><a name="p1350114961316"></a><a name="p1350114961316"></a>资源标签。</p>
    <p id="p111349461418"><a name="p111349461418"></a><a name="p111349461418"></a>取值格式：key1,value1|key2,value2</p>
    <p id="p18134744140"><a name="p18134744140"></a><a name="p18134744140"></a>多个标签之间用"|"分开，每个标签的键值用英文逗号","相隔。</p>
    <p id="p18134204181420"><a name="p18134204181420"></a><a name="p18134204181420"></a>多个标签之间为“与”的关系。</p>
    <p id="p8134749148"><a name="p8134749148"></a><a name="p8134749148"></a>关于资源标签，请参见<a href="#table619059185111">表6 tag对象参数说明</a>。</p>
    <p id="p61341740143"><a name="p61341740143"></a><a name="p61341740143"></a>搜索模式为精确搜索。如果资源标签值value是以*开头时，则按照*后面的值全模糊匹配。</p>
    <p id="p1713404141413"><a name="p1713404141413"></a><a name="p1713404141413"></a>默认值为空。</p>
    </td>
    </tr>
    <tr id="row540810311563"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="p2408231966"><a name="p2408231966"></a><a name="p2408231966"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="p9408103116617"><a name="p9408103116617"></a><a name="p9408103116617"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="p18408153111619"><a name="p18408153111619"></a><a name="p18408153111619"></a>域名关联的企业项目ID，长度不超过36个字符。</p>
    </td>
    </tr>
    <tr id="re2fe47183e18405d92046423a13cc360"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.1 "><p id="aaad74d843b144b02886916b90476b9eb"><a name="aaad74d843b144b02886916b90476b9eb"></a><a name="aaad74d843b144b02886916b90476b9eb"></a>masters</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.41%" headers="mcps1.2.4.1.2 "><p id="ac58ddffcdd4b4db48b9da9a1aa4b94b8"><a name="ac58ddffcdd4b4db48b9da9a1aa4b94b8"></a><a name="ac58ddffcdd4b4db48b9da9a1aa4b94b8"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="a2693d405736c4ed38996b010ac12ed27"><a name="a2693d405736c4ed38996b010ac12ed27"></a><a name="a2693d405736c4ed38996b010ac12ed27"></a>主从模式中，从DNS服务器用以获取DNS信息。</p>
    <p id="p052113815317"><a name="p052113815317"></a><a name="p052113815317"></a>目前暂未使用。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  metadata参数说明

    <a name="table52442344175457"></a>
    <table><thead align="left"><tr id="row58979189175457"><th class="cellrowborder" valign="top" width="18.48184818481848%" id="mcps1.2.4.1.1"><p id="p46156243175457"><a name="p46156243175457"></a><a name="p46156243175457"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.46194619461946%" id="mcps1.2.4.1.2"><p id="p47668234175457"><a name="p47668234175457"></a><a name="p47668234175457"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.05620562056207%" id="mcps1.2.4.1.3"><p id="p35921708175457"><a name="p35921708175457"></a><a name="p35921708175457"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row54859922175457"><td class="cellrowborder" valign="top" width="18.48184818481848%" headers="mcps1.2.4.1.1 "><p id="p14468674175457"><a name="p14468674175457"></a><a name="p14468674175457"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.46194619461946%" headers="mcps1.2.4.1.2 "><p id="p31111955175457"><a name="p31111955175457"></a><a name="p31111955175457"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.05620562056207%" headers="mcps1.2.4.1.3 "><p id="p37040428175457"><a name="p37040428175457"></a><a name="p37040428175457"></a>满足查询条件的资源总数，不受分页（即limit、offset参数）影响。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  links参数说明

    <a name="table0172144213344"></a>
    <table><thead align="left"><tr id="row917304253418"><th class="cellrowborder" valign="top" width="18.391839183918393%" id="mcps1.2.4.1.1"><p id="p101731742153416"><a name="p101731742153416"></a><a name="p101731742153416"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.55195519551955%" id="mcps1.2.4.1.2"><p id="p0174542163418"><a name="p0174542163418"></a><a name="p0174542163418"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.05620562056207%" id="mcps1.2.4.1.3"><p id="p7174194243414"><a name="p7174194243414"></a><a name="p7174194243414"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1917494211345"><td class="cellrowborder" valign="top" width="18.391839183918393%" headers="mcps1.2.4.1.1 "><p id="p13174134215348"><a name="p13174134215348"></a><a name="p13174134215348"></a>self</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.55195519551955%" headers="mcps1.2.4.1.2 "><p id="p181741642173417"><a name="p181741642173417"></a><a name="p181741642173417"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.05620562056207%" headers="mcps1.2.4.1.3 "><p id="p1017434223419"><a name="p1017434223419"></a><a name="p1017434223419"></a>当前资源的链接。</p>
    </td>
    </tr>
    <tr id="row88718634719"><td class="cellrowborder" valign="top" width="18.391839183918393%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.55195519551955%" headers="mcps1.2.4.1.2 "><p id="p19656144517367"><a name="p19656144517367"></a><a name="p19656144517367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.05620562056207%" headers="mcps1.2.4.1.3 "><p id="p76567451365"><a name="p76567451365"></a><a name="p76567451365"></a>下一页资源的链接。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  tag对象说明

    <a name="table619059185111"></a>
    <table><thead align="left"><tr id="row15361836112436"><th class="cellrowborder" valign="top" width="18.2%" id="mcps1.2.4.1.1"><p id="p58707511112436"><a name="p58707511112436"></a><a name="p58707511112436"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.07%" id="mcps1.2.4.1.2"><p id="p42210623112436"><a name="p42210623112436"></a><a name="p42210623112436"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.73%" id="mcps1.2.4.1.3"><p id="p63617265112436"><a name="p63617265112436"></a><a name="p63617265112436"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row35684479112436"><td class="cellrowborder" valign="top" width="18.2%" headers="mcps1.2.4.1.1 "><p id="p13313439112530"><a name="p13313439112530"></a><a name="p13313439112530"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.07%" headers="mcps1.2.4.1.2 "><p id="p35653193112436"><a name="p35653193112436"></a><a name="p35653193112436"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.73%" headers="mcps1.2.4.1.3 "><p id="p011410211144"><a name="p011410211144"></a><a name="p011410211144"></a>键。</p>
    <p id="p12621122816413"><a name="p12621122816413"></a><a name="p12621122816413"></a>最大长度36个unicode字符。 key不能为空。不能包含“=”、“*”、“&lt;”、“&gt;”、“\”、“,”、“|”和“/”，且首尾字符不能为空格。</p>
    </td>
    </tr>
    <tr id="row20048002112436"><td class="cellrowborder" valign="top" width="18.2%" headers="mcps1.2.4.1.1 "><p id="p66095544112533"><a name="p66095544112533"></a><a name="p66095544112533"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.07%" headers="mcps1.2.4.1.2 "><p id="p60123528112436"><a name="p60123528112436"></a><a name="p60123528112436"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.73%" headers="mcps1.2.4.1.3 "><p id="p592417401420"><a name="p592417401420"></a><a name="p592417401420"></a>值。</p>
    <p id="p3383124915419"><a name="p3383124915419"></a><a name="p3383124915419"></a>每个值最大长度43个unicode字符，可以为空字符串。 不能包含“=”、“*”、“&lt;”、“&gt;”、“\”、“,”、“|”和“/”，且首尾字符不能为空格。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "links": {
            "self": "https://Endpoint/v2/zones?type=public&limit=11",
            "next": "https://Endpoint/v2/zones?type=public&limit=11&marker=2c9eb155587194ec01587224c9f90149"
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


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

