# 查询PTR Record列表<a name="ZH-CN_TOPIC_0042318615"></a>

## 功能介绍<a name="section29105235"></a>

查询租户弹性IP的PTR记录列表。

## URI<a name="section60620523"></a>

GET /v2/reverse/floatingips?limit=\{limit\}&marker=\{marker\}&offset=\{offset\}&tags=\{tags\}

参数说明请参见[表1](#table1562846014112)。

**表 1**  URI格式的参数说明

<a name="table1562846014112"></a>
<table><thead align="left"><tr id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_row24110047"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p6756797"><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p6756797"></a><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p6756797"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p10429724"><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p10429724"></a><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p10429724"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14141414141414%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p39501348"><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p39501348"></a><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p39501348"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p45492604"><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p45492604"></a><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p45492604"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_row61022284"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p43857981"><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p43857981"></a><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p43857981"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p62835574"><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p62835574"></a><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p62835574"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p56516768"><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p56516768"></a><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p56516768"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p14455523"><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p14455523"></a><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p14455523"></a>分页查询起始的资源ID，为空时为查询第一页。</p>
</td>
</tr>
<tr id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_row62990845"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p1984791"><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p1984791"></a><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p1984791"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p26550365"><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p26550365"></a><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p26550365"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p3095993"><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p3095993"></a><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p3095993"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_ul18169499193915"></a><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_ul18169499193915"></a><ul id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_ul18169499193915"><li>取值范围：0~500<p id="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p61821521193933"><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p61821521193933"></a><a name="zh-cn_topic_0037134402_zh-cn_topic_0037129969_p61821521193933"></a>取值一般为10，20，50</p>
</li><li>功能说明：每页返回的资源个数。</li></ul>
</td>
</tr>
<tr id="row58150604195642"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p11536930195644"><a name="p11536930195644"></a><a name="p11536930195644"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p62076162195644"><a name="p62076162195644"></a><a name="p62076162195644"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p62113243195644"><a name="p62113243195644"></a><a name="p62113243195644"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="ul65116756195644"></a><a name="ul65116756195644"></a><ul id="ul65116756195644"><li>取值范围：0~2147483647</li><li>分页查询起始页码，起始值为0。当前设置marker不为空时，以marker为分页起始标识。</li></ul>
</td>
</tr>
<tr id="row6180858115857"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.5.1.1 "><p id="p6537624212219"><a name="p6537624212219"></a><a name="p6537624212219"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.5.1.2 "><p id="p6098421112219"><a name="p6098421112219"></a><a name="p6098421112219"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p4077405312219"><a name="p4077405312219"></a><a name="p4077405312219"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p1436398312219"><a name="p1436398312219"></a><a name="p1436398312219"></a>资源标签。</p>
<p id="p6216698912219"><a name="p6216698912219"></a><a name="p6216698912219"></a>取值格式：key1,value1|key2,value2</p>
<p id="p64141841114123"><a name="p64141841114123"></a><a name="p64141841114123"></a>多个标签之间用"|"分开，每个标签的键值用英文逗号","相隔。</p>
<p id="p2263199412219"><a name="p2263199412219"></a><a name="p2263199412219"></a>多个标签之间为“与”的关系。</p>
<p id="p65263192115146"><a name="p65263192115146"></a><a name="p65263192115146"></a>关于资源标签，请参见<a href="添加资源标签.md">添加资源标签</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section8713795"></a>

无

## 响应<a name="section11315292"></a>

-   要素说明

    **表 2**  响应样例的要素说明

    <a name="table13410777181232"></a>
    <table><thead align="left"><tr id="row8598877181232"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="p25420464181232"><a name="p25420464181232"></a><a name="p25420464181232"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.189999999999998%" id="mcps1.2.4.1.2"><p id="p45791683181232"><a name="p45791683181232"></a><a name="p45791683181232"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.629999999999995%" id="mcps1.2.4.1.3"><p id="p18138814181232"><a name="p18138814181232"></a><a name="p18138814181232"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row59957834181232"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p24746382181232"><a name="p24746382181232"></a><a name="p24746382181232"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="p58299955181232"><a name="p58299955181232"></a><a name="p58299955181232"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p5040034717923"><a name="p5040034717923"></a><a name="p5040034717923"></a>指向当前资源或者其他相关资源的链接。</p>
    <p id="p5094994217923"><a name="p5094994217923"></a><a name="p5094994217923"></a>当响应需要分页时，需要包含一个next链接来进行分页。</p>
    </td>
    </tr>
    <tr id="row17649295181232"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p20306794181232"><a name="p20306794181232"></a><a name="p20306794181232"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="p34237593181232"><a name="p34237593181232"></a><a name="p34237593181232"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p21781637181232"><a name="p21781637181232"></a><a name="p21781637181232"></a>返回满足过滤条件的资源总数。</p>
    </td>
    </tr>
    <tr id="row61817005181232"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p41121470181232"><a name="p41121470181232"></a><a name="p41121470181232"></a>floatingips</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="p42504768181232"><a name="p42504768181232"></a><a name="p42504768181232"></a>列表对象</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p20334170181232"><a name="p20334170181232"></a><a name="p20334170181232"></a>PTR Record对象列表。</p>
    </td>
    </tr>
    </tbody>
    </table>

    其中，floatingips的字段说明请参见[表3](#table43740677113542)，metadata字段说明请参见[表4](#table16355953155210)。 

    **表 3**  floatingips字段说明

    <a name="table43740677113542"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0042318613_row5725206118456"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0042318613_p690539418456"><a name="zh-cn_topic_0042318613_p690539418456"></a><a name="zh-cn_topic_0042318613_p690539418456"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.189999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0042318613_p2246606418456"><a name="zh-cn_topic_0042318613_p2246606418456"></a><a name="zh-cn_topic_0042318613_p2246606418456"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.629999999999995%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0042318613_p781187018456"><a name="zh-cn_topic_0042318613_p781187018456"></a><a name="zh-cn_topic_0042318613_p781187018456"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0042318613_row2878170018456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0042318613_p4961636318456"><a name="zh-cn_topic_0042318613_p4961636318456"></a><a name="zh-cn_topic_0042318613_p4961636318456"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0042318613_p5950245818456"><a name="zh-cn_topic_0042318613_p5950245818456"></a><a name="zh-cn_topic_0042318613_p5950245818456"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0042318613_p5496981818456"><a name="zh-cn_topic_0042318613_p5496981818456"></a><a name="zh-cn_topic_0042318613_p5496981818456"></a>PTR记录的ID，格式形如{region}:{floatingip_id}。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0042318613_row3274940018456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0042318613_p3545576918456"><a name="zh-cn_topic_0042318613_p3545576918456"></a><a name="zh-cn_topic_0042318613_p3545576918456"></a>ptrdname</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0042318613_p5334507918456"><a name="zh-cn_topic_0042318613_p5334507918456"></a><a name="zh-cn_topic_0042318613_p5334507918456"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0042318613_p2598415318456"><a name="zh-cn_topic_0042318613_p2598415318456"></a><a name="zh-cn_topic_0042318613_p2598415318456"></a>PTR记录对应的域名。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0042318613_row3253079218456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0042318613_p1774845918456"><a name="zh-cn_topic_0042318613_p1774845918456"></a><a name="zh-cn_topic_0042318613_p1774845918456"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0042318613_p2833911218456"><a name="zh-cn_topic_0042318613_p2833911218456"></a><a name="zh-cn_topic_0042318613_p2833911218456"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0042318613_p1376672518456"><a name="zh-cn_topic_0042318613_p1376672518456"></a><a name="zh-cn_topic_0042318613_p1376672518456"></a>对PTR记录的描述。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0042318613_row5679166318456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0042318613_p3672198418456"><a name="zh-cn_topic_0042318613_p3672198418456"></a><a name="zh-cn_topic_0042318613_p3672198418456"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0042318613_p2169069318456"><a name="zh-cn_topic_0042318613_p2169069318456"></a><a name="zh-cn_topic_0042318613_p2169069318456"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0042318613_p1211568618456"><a name="zh-cn_topic_0042318613_p1211568618456"></a><a name="zh-cn_topic_0042318613_p1211568618456"></a>PTR记录的有效缓存时间，以秒为单位，默认值为300s。</p>
    <p id="zh-cn_topic_0042318613_p4184654118456"><a name="zh-cn_topic_0042318613_p4184654118456"></a><a name="zh-cn_topic_0042318613_p4184654118456"></a>取值范围：</p>
    <p id="zh-cn_topic_0042318613_p4107454918456"><a name="zh-cn_topic_0042318613_p4107454918456"></a><a name="zh-cn_topic_0042318613_p4107454918456"></a>300～2147483647。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0042318613_row3412662318456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0042318613_p1279309418456"><a name="zh-cn_topic_0042318613_p1279309418456"></a><a name="zh-cn_topic_0042318613_p1279309418456"></a>address</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0042318613_p2960772218456"><a name="zh-cn_topic_0042318613_p2960772218456"></a><a name="zh-cn_topic_0042318613_p2960772218456"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0042318613_p4941528218456"><a name="zh-cn_topic_0042318613_p4941528218456"></a><a name="zh-cn_topic_0042318613_p4941528218456"></a>弹性IP的IP地址。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0042318613_row4208435918456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0042318613_p5338995318456"><a name="zh-cn_topic_0042318613_p5338995318456"></a><a name="zh-cn_topic_0042318613_p5338995318456"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0042318613_p2961896418456"><a name="zh-cn_topic_0042318613_p2961896418456"></a><a name="zh-cn_topic_0042318613_p2961896418456"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0042318613_p5032586318456"><a name="zh-cn_topic_0042318613_p5032586318456"></a><a name="zh-cn_topic_0042318613_p5032586318456"></a>资源状态。</p>
    <p id="p1427831035118"><a name="p1427831035118"></a><a name="p1427831035118"></a>取值范围：PENDING_CREATE，ACTIVE，PENDING_DELETE，PENDING_UPDATE，ERROR 。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0042318613_row4986307418456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0042318613_p1237719818456"><a name="zh-cn_topic_0042318613_p1237719818456"></a><a name="zh-cn_topic_0042318613_p1237719818456"></a>action</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0042318613_p6302897818456"><a name="zh-cn_topic_0042318613_p6302897818456"></a><a name="zh-cn_topic_0042318613_p6302897818456"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0042318613_p507362318456"><a name="zh-cn_topic_0042318613_p507362318456"></a><a name="zh-cn_topic_0042318613_p507362318456"></a>对该资源的当前操作。</p>
    <p id="p3570202615112"><a name="p3570202615112"></a><a name="p3570202615112"></a>取值范围：CREATE，UPDATE，DELETE。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0042318613_row831034118456"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0042318613_p204899518456"><a name="zh-cn_topic_0042318613_p204899518456"></a><a name="zh-cn_topic_0042318613_p204899518456"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0042318613_p3175087318456"><a name="zh-cn_topic_0042318613_p3175087318456"></a><a name="zh-cn_topic_0042318613_p3175087318456"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0042318613_p2168392018456"><a name="zh-cn_topic_0042318613_p2168392018456"></a><a name="zh-cn_topic_0042318613_p2168392018456"></a>指向当前资源或者其他相关资源的链接。</p>
    <p id="zh-cn_topic_0042318613_p6093755518456"><a name="zh-cn_topic_0042318613_p6093755518456"></a><a name="zh-cn_topic_0042318613_p6093755518456"></a>当响应需要分页时，需要包含一个next链接来进行分页。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  metadata参数说明

    <a name="table16355953155210"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0037134402_row58979189175457"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0037134402_p46156243175457"><a name="zh-cn_topic_0037134402_p46156243175457"></a><a name="zh-cn_topic_0037134402_p46156243175457"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0037134402_p47668234175457"><a name="zh-cn_topic_0037134402_p47668234175457"></a><a name="zh-cn_topic_0037134402_p47668234175457"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0037134402_p35921708175457"><a name="zh-cn_topic_0037134402_p35921708175457"></a><a name="zh-cn_topic_0037134402_p35921708175457"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0037134402_row54859922175457"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134402_p14468674175457"><a name="zh-cn_topic_0037134402_p14468674175457"></a><a name="zh-cn_topic_0037134402_p14468674175457"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134402_p31111955175457"><a name="zh-cn_topic_0037134402_p31111955175457"></a><a name="zh-cn_topic_0037134402_p31111955175457"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134402_p37040428175457"><a name="zh-cn_topic_0037134402_p37040428175457"></a><a name="zh-cn_topic_0037134402_p37040428175457"></a>资源总数</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "links": {
            "self": "https://Endpoint/v2/reverse/floatingips"
        },
        "metadata": {
            "total_count": 1
        },
        "floatingips": [
            {
                "id": "region_id:c5504932-bf23-4171-b655-b87a6bc59334",
                "ptrdname": "www.example.com.",
                "description": "Description for this PTR record",
                "address": "10.154.52.138",
                "action": "NONE",
                "ttl": 300,
                "status": "ACTIVE",
                "links": {
                    "self": "https://Endpoint/v2/reverse/floatingips/region_id:c5504932-bf23-4171-b655-b87a6bc59334"
                }
            }
        ]
    }
    ```


## 返回值<a name="section34728767"></a>

请参考[通用请求返回值](通用请求返回值.md)。

