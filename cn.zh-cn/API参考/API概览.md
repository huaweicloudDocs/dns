# API概览<a name="zh-cn_topic_0132421999"></a>

云解析服务提供自研的REST接口。

通过使用云解析服务的接口，您可以完整的使用云解析服务的所有功能，包括对公网域名、内网域名、记录集等资源的创建、查询、修改和删除。

云解析服务提供的具体API如[表1](#table138131522381)所示。

**表 1**  接口说明

<a name="table138131522381"></a>
<table><thead align="left"><tr id="row1781315293816"><th class="cellrowborder" valign="top" width="36.9%" id="mcps1.2.3.1.1"><p id="p1981355253811"><a name="p1981355253811"></a><a name="p1981355253811"></a>子类型</p>
</th>
<th class="cellrowborder" valign="top" width="63.1%" id="mcps1.2.3.1.2"><p id="p281315263819"><a name="p281315263819"></a><a name="p281315263819"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row9813152113817"><td class="cellrowborder" valign="top" width="36.9%" headers="mcps1.2.3.1.1 "><p id="p16813152123819"><a name="p16813152123819"></a><a name="p16813152123819"></a>版本管理</p>
</td>
<td class="cellrowborder" valign="top" width="63.1%" headers="mcps1.2.3.1.2 "><p id="p10814552153819"><a name="p10814552153819"></a><a name="p10814552153819"></a>DNS API的版本查询接口，支持查询所有API或者指定API的版本号。</p>
</td>
</tr>
<tr id="row11814185263819"><td class="cellrowborder" valign="top" width="36.9%" headers="mcps1.2.3.1.1 "><p id="p1681485293812"><a name="p1681485293812"></a><a name="p1681485293812"></a>公网Zone管理</p>
</td>
<td class="cellrowborder" valign="top" width="63.1%" headers="mcps1.2.3.1.2 "><p id="p13814145233816"><a name="p13814145233816"></a><a name="p13814145233816"></a>DNS API的公网域名管理接口，实现对公网域名的创建、删除、修改以及查询。</p>
</td>
</tr>
<tr id="row164093101809"><td class="cellrowborder" valign="top" width="36.9%" headers="mcps1.2.3.1.1 "><p id="p19409121016019"><a name="p19409121016019"></a><a name="p19409121016019"></a>内网Zone管理</p>
</td>
<td class="cellrowborder" valign="top" width="63.1%" headers="mcps1.2.3.1.2 "><p id="p2410151015017"><a name="p2410151015017"></a><a name="p2410151015017"></a>DNS API的内网域名管理接口，实现对内网域名的创建、删除、修改以及查询。</p>
</td>
</tr>
<tr id="row128140521381"><td class="cellrowborder" valign="top" width="36.9%" headers="mcps1.2.3.1.1 "><p id="p17814452203813"><a name="p17814452203813"></a><a name="p17814452203813"></a>Record Set管理</p>
</td>
<td class="cellrowborder" valign="top" width="63.1%" headers="mcps1.2.3.1.2 "><p id="p19814115273814"><a name="p19814115273814"></a><a name="p19814115273814"></a>DNS API的记录集管理接口，实现为公网域名和内网域名创建、删除、修改以及查询解析记录。</p>
</td>
</tr>
<tr id="row08141952193817"><td class="cellrowborder" valign="top" width="36.9%" headers="mcps1.2.3.1.1 "><p id="p781614529385"><a name="p781614529385"></a><a name="p781614529385"></a>Record Set多线路管理</p>
</td>
<td class="cellrowborder" valign="top" width="63.1%" headers="mcps1.2.3.1.2 "><p id="p198161452183815"><a name="p198161452183815"></a><a name="p198161452183815"></a>DNS API的多线路解析管理接口，实现为公网域名创建、删除、修改以及查询多线路解析的解析记录。</p>
</td>
</tr>
<tr id="row19816752163815"><td class="cellrowborder" valign="top" width="36.9%" headers="mcps1.2.3.1.1 "><p id="p3816185212381"><a name="p3816185212381"></a><a name="p3816185212381"></a>PTR Record管理</p>
</td>
<td class="cellrowborder" valign="top" width="63.1%" headers="mcps1.2.3.1.2 "><p id="p14816105210387"><a name="p14816105210387"></a><a name="p14816105210387"></a>DNS API的反向解析管理接口，实现创建、删除、修改以及查询弹性IP到域名的反向解析记录。</p>
</td>
</tr>
<tr id="row181655210387"><td class="cellrowborder" valign="top" width="36.9%" headers="mcps1.2.3.1.1 "><p id="p17816185210388"><a name="p17816185210388"></a><a name="p17816185210388"></a>TAG管理</p>
</td>
<td class="cellrowborder" valign="top" width="63.1%" headers="mcps1.2.3.1.2 "><p id="p7816135283812"><a name="p7816135283812"></a><a name="p7816135283812"></a>DNS API的标签管理接口，实现为指定实例创建、删除、修改以及查询标签，同时还支持为指定实例批量创建或删除标签。</p>
</td>
</tr>
<tr id="row3277163535313"><td class="cellrowborder" valign="top" width="36.9%" headers="mcps1.2.3.1.1 "><p id="p19278835105313"><a name="p19278835105313"></a><a name="p19278835105313"></a>自定义线路管理</p>
</td>
<td class="cellrowborder" valign="top" width="63.1%" headers="mcps1.2.3.1.2 "><p id="p1127815352539"><a name="p1127815352539"></a><a name="p1127815352539"></a>DNS API的自定义线路管理接口，实现自定义线路的创建、删除、更新及查询。</p>
</td>
</tr>
<tr id="row1023081012503"><td class="cellrowborder" valign="top" width="36.9%" headers="mcps1.2.3.1.1 "><p id="p6231191025016"><a name="p6231191025016"></a><a name="p6231191025016"></a>名称服务器管理</p>
</td>
<td class="cellrowborder" valign="top" width="63.1%" headers="mcps1.2.3.1.2 "><p id="p9231910145013"><a name="p9231910145013"></a><a name="p9231910145013"></a>DNS API的名称服务器管理接口，实现名称服务器的查询。</p>
</td>
</tr>
</tbody>
</table>

## 版本管理接口<a name="section174483361620"></a>

版本管理接口，用于查询所有DNS API版本的接口和查询指定DNS API版本的接口。

**表 2**  版本管理接口

<a name="table1280213192913"></a>
<table><thead align="left"><tr id="row102811313142913"><th class="cellrowborder" valign="top" width="34.42%" id="mcps1.2.3.1.1"><p id="p42815133294"><a name="p42815133294"></a><a name="p42815133294"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="65.58%" id="mcps1.2.3.1.2"><p id="p102810131296"><a name="p102810131296"></a><a name="p102810131296"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row528181312912"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p19281913112915"><a name="p19281913112915"></a><a name="p19281913112915"></a><a href="查询版本号列表.md">查询版本号列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p4281813102913"><a name="p4281813102913"></a><a name="p4281813102913"></a>查询所有DNS API接口的版本。</p>
</td>
</tr>
<tr id="row1028118132292"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p7281111316299"><a name="p7281111316299"></a><a name="p7281111316299"></a><a href="查询版本号.md">查询版本号</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p6281101316297"><a name="p6281101316297"></a><a name="p6281101316297"></a>查询指定DNS API接口的版本。</p>
</td>
</tr>
</tbody>
</table>

## 公网Zone管理接口<a name="section848205510315"></a>

公网Zone管理接口，用于创建、查询、删除以及修改公网Zone。

**表 3**  公网Zone管理接口

<a name="table94835516312"></a>
<table><thead align="left"><tr id="row64817556315"><th class="cellrowborder" valign="top" width="34.42%" id="mcps1.2.3.1.1"><p id="p1148195513110"><a name="p1148195513110"></a><a name="p1148195513110"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="65.58%" id="mcps1.2.3.1.2"><p id="p948195593118"><a name="p948195593118"></a><a name="p948195593118"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row249955183118"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p154995514313"><a name="p154995514313"></a><a name="p154995514313"></a><a href="创建公网Zone.md">创建公网Zone</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p449855173119"><a name="p449855173119"></a><a name="p449855173119"></a>创建单个公网Zone。</p>
</td>
</tr>
<tr id="row449655193114"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p1349355123119"><a name="p1349355123119"></a><a name="p1349355123119"></a><a href="查询公网Zone.md">查询公网Zone</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p1049195533115"><a name="p1049195533115"></a><a name="p1049195533115"></a>查询单个公网Zone。</p>
</td>
</tr>
<tr id="row8355374321"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p133551470325"><a name="p133551470325"></a><a name="p133551470325"></a><a href="查询公网Zone列表.md">查询公网Zone列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p1735516743220"><a name="p1735516743220"></a><a name="p1735516743220"></a>查询公网Zone列表。</p>
</td>
</tr>
<tr id="row1335613793214"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p11356107113220"><a name="p11356107113220"></a><a name="p11356107113220"></a><a href="查询公网Zone的名称服务器.md">查询公网Zone的名称服务器</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p1235617717322"><a name="p1235617717322"></a><a name="p1235617717322"></a>查询单个公网Zone的名称服务器。</p>
</td>
</tr>
<tr id="row8700718173216"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p1670041814326"><a name="p1670041814326"></a><a name="p1670041814326"></a><a href="删除公网Zone.md">删除公网Zone</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p137011718103214"><a name="p137011718103214"></a><a name="p137011718103214"></a>删除单个公网Zone。</p>
</td>
</tr>
<tr id="row723519211320"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p162356215320"><a name="p162356215320"></a><a name="p162356215320"></a><a href="修改公网Zone.md">修改公网Zone</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p122352213328"><a name="p122352213328"></a><a name="p122352213328"></a>修改单个公网Zone。</p>
</td>
</tr>
<tr id="row141681115249"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p2169121122410"><a name="p2169121122410"></a><a name="p2169121122410"></a><a href="设置Zone状态.md">设置Zone状态</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p5169121182417"><a name="p5169121182417"></a><a name="p5169121182417"></a>设置单个公网Zone状态。</p>
</td>
</tr>
</tbody>
</table>

## 内网Zone管理接口<a name="section1913415455371"></a>

内网Zone管理接口，用于创建、查询、删除以及修改内网Zone。

**表 4**  内网Zone管理接口

<a name="table9134145183719"></a>
<table><thead align="left"><tr id="row1513424516378"><th class="cellrowborder" valign="top" width="34.42%" id="mcps1.2.3.1.1"><p id="p1313474518372"><a name="p1313474518372"></a><a name="p1313474518372"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="65.58%" id="mcps1.2.3.1.2"><p id="p813517459376"><a name="p813517459376"></a><a name="p813517459376"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row9135164512370"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p131351645193714"><a name="p131351645193714"></a><a name="p131351645193714"></a><a href="创建内网Zone.md">创建内网Zone</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p1613513455376"><a name="p1613513455376"></a><a name="p1613513455376"></a>查询单个内网Zone。</p>
</td>
</tr>
<tr id="row1013524543711"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p201351456375"><a name="p201351456375"></a><a name="p201351456375"></a><a href="内网Zone关联VPC.md">内网Zone关联VPC</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p1013524503710"><a name="p1013524503710"></a><a name="p1013524503710"></a>为内网Zone关联VPC。</p>
</td>
</tr>
<tr id="row8135345173719"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p513564523716"><a name="p513564523716"></a><a name="p513564523716"></a><a href="内网Zone解关联VPC.md">内网Zone解关联VPC</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p613517457370"><a name="p613517457370"></a><a name="p613517457370"></a>为内网Zone解关联VPC。</p>
</td>
</tr>
<tr id="row313513454374"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p413544593714"><a name="p413544593714"></a><a name="p413544593714"></a><a href="查询内网Zone.md">查询内网Zone</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p6135645153720"><a name="p6135645153720"></a><a name="p6135645153720"></a>查询单个内网Zone。</p>
</td>
</tr>
<tr id="row101357455375"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p11135144515377"><a name="p11135144515377"></a><a name="p11135144515377"></a><a href="查询内网Zone列表.md">查询内网Zone列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p1813564543715"><a name="p1813564543715"></a><a name="p1813564543715"></a>查询内网Zone列表。</p>
</td>
</tr>
<tr id="row1762618110394"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p862616113390"><a name="p862616113390"></a><a name="p862616113390"></a><a href="查询内网Zone的名称服务器.md">查询内网Zone的名称服务器</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p26263111390"><a name="p26263111390"></a><a name="p26263111390"></a>查询内网Zone的名称服务器。</p>
</td>
</tr>
<tr id="row1762671193912"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p196264110395"><a name="p196264110395"></a><a name="p196264110395"></a><a href="删除内网Zone.md">删除内网Zone</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p7952113458"><a name="p7952113458"></a><a name="p7952113458"></a>删除单个内网Zone。</p>
</td>
</tr>
<tr id="row11626717397"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p1662691193914"><a name="p1662691193914"></a><a name="p1662691193914"></a><a href="修改内网Zone.md">修改内网Zone</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p201011211455"><a name="p201011211455"></a><a name="p201011211455"></a>修改单个内网Zone。</p>
</td>
</tr>
</tbody>
</table>

## Record Set管理接口<a name="section8115537144512"></a>

Record Set管理接口，用于创建、查询、删除以及修改Record Set。

**表 5**  Record Set管理接口

<a name="table1116193714453"></a>
<table><thead align="left"><tr id="row511618375453"><th class="cellrowborder" valign="top" width="34.42%" id="mcps1.2.3.1.1"><p id="p9116837124518"><a name="p9116837124518"></a><a name="p9116837124518"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="65.58%" id="mcps1.2.3.1.2"><p id="p1611653784517"><a name="p1611653784517"></a><a name="p1611653784517"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row21161137164513"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p1411615373452"><a name="p1411615373452"></a><a name="p1411615373452"></a><a href="创建Record-Set.md">创建Record Set</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p2116143717458"><a name="p2116143717458"></a><a name="p2116143717458"></a>创建单个Record Set。</p>
</td>
</tr>
<tr id="row511653717451"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p211618375452"><a name="p211618375452"></a><a name="p211618375452"></a><a href="查询Record-Set.md">查询Record Set</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p151166376456"><a name="p151166376456"></a><a name="p151166376456"></a>查询单个Record Set。</p>
</td>
</tr>
<tr id="row20116133710459"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p124919516471"><a name="p124919516471"></a><a name="p124919516471"></a><a href="查询Record-Set列表.md">查询Record Set列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p18116203715454"><a name="p18116203715454"></a><a name="p18116203715454"></a>查询租户Record Set资源列表。</p>
</td>
</tr>
<tr id="row31171537164519"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p134892051473"><a name="p134892051473"></a><a name="p134892051473"></a><a href="查询单个Zone下Record-Set列表.md">查询单个Zone下Record Set列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p41171437194513"><a name="p41171437194513"></a><a name="p41171437194513"></a>查询单个Zone的Record Set列表。</p>
</td>
</tr>
<tr id="row181171837134519"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p1748895154714"><a name="p1748895154714"></a><a name="p1748895154714"></a><a href="删除Record-Set.md">删除Record Set</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p51171537204515"><a name="p51171537204515"></a><a name="p51171537204515"></a>删除单个Record Set。</p>
</td>
</tr>
<tr id="row411743764519"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p648718584711"><a name="p648718584711"></a><a name="p648718584711"></a><a href="修改Record-Set.md">修改Record Set</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p1211712372452"><a name="p1211712372452"></a><a name="p1211712372452"></a>修改单个Record Set。</p>
</td>
</tr>
</tbody>
</table>

## Record Set多线路管理接口<a name="section7487124385817"></a>

Record Set多线路管理接口，用于在多线路解析中创建、查询、删除以及修改Record Set。

**表 6**  Record Set多线路管理接口

<a name="table16489743145819"></a>
<table><thead align="left"><tr id="row849113437588"><th class="cellrowborder" valign="top" width="34.42%" id="mcps1.2.3.1.1"><p id="p1149114317589"><a name="p1149114317589"></a><a name="p1149114317589"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="65.58%" id="mcps1.2.3.1.2"><p id="p13491184345816"><a name="p13491184345816"></a><a name="p13491184345816"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1949174315581"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p169024112593"><a name="p169024112593"></a><a name="p169024112593"></a><a href="创建Record-Set-多线路.md">创建Record Set</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p657563415120"><a name="p657563415120"></a><a name="p657563415120"></a>创建单个Record Set。</p>
</td>
</tr>
<tr id="row11491114365816"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p790171165914"><a name="p790171165914"></a><a name="p790171165914"></a><a href="查询Record-Set-多线路.md">查询Record Set</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p35759346112"><a name="p35759346112"></a><a name="p35759346112"></a>查询单个Record Set。</p>
</td>
</tr>
<tr id="row17492343125817"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p1610851597"><a name="p1610851597"></a><a name="p1610851597"></a><a href="查询Record-Set列表-多线路.md">查询Record Set列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p205751341813"><a name="p205751341813"></a><a name="p205751341813"></a>查询租户Record Set资源列表。</p>
</td>
</tr>
<tr id="row184922043135819"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p5608359597"><a name="p5608359597"></a><a name="p5608359597"></a><a href="查询单个Zone下Record-Set列表-多线路.md">查询单个Zone下Record Set列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p19575143415112"><a name="p19575143415112"></a><a name="p19575143415112"></a>查询单个Zone的Record Set列表。</p>
</td>
</tr>
<tr id="row9492114395818"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p13605145155913"><a name="p13605145155913"></a><a name="p13605145155913"></a><a href="删除Record-Set-多线路.md">删除Record Set</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p165755341315"><a name="p165755341315"></a><a name="p165755341315"></a>删除单个Record Set。</p>
</td>
</tr>
<tr id="row15492043145815"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p146021253599"><a name="p146021253599"></a><a name="p146021253599"></a><a href="修改Record-Set-多线路.md">修改Record Set</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p557514341816"><a name="p557514341816"></a><a name="p557514341816"></a>修改单个Record Set。</p>
</td>
</tr>
<tr id="row78141416599"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p45991556591"><a name="p45991556591"></a><a name="p45991556591"></a><a href="设置Record-Set状态.md">设置Record Set状态</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p459714565913"><a name="p459714565913"></a><a name="p459714565913"></a>设置Record Set状态，包括启用或暂停解析。</p>
</td>
</tr>
</tbody>
</table>

## PTR Record管理接口<a name="section599018465414"></a>

PTR Record管理接口，用于为弹性IP设置反向解析，包括设置、查询以及修改Record Set，并支持将弹性IP的PTR Record恢复为默认值。

**表 7**  PTR Record管理接口

<a name="table29913461649"></a>
<table><thead align="left"><tr id="row099118461142"><th class="cellrowborder" valign="top" width="34.42%" id="mcps1.2.3.1.1"><p id="p99918467411"><a name="p99918467411"></a><a name="p99918467411"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="65.58%" id="mcps1.2.3.1.2"><p id="p179916466411"><a name="p179916466411"></a><a name="p179916466411"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row09911246346"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p209303431754"><a name="p209303431754"></a><a name="p209303431754"></a><a href="设置PTR-Record.md">设置PTR Record</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p0991124615411"><a name="p0991124615411"></a><a name="p0991124615411"></a>设置弹性IP的PTR Record。</p>
</td>
</tr>
<tr id="row1799218469413"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p33510196613"><a name="p33510196613"></a><a name="p33510196613"></a><a href="查询PTR-Record.md">查询PTR Record</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p18992194612416"><a name="p18992194612416"></a><a name="p18992194612416"></a>查询单个弹性IP的PTR Record。</p>
</td>
</tr>
<tr id="row99923461547"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p59295431451"><a name="p59295431451"></a><a name="p59295431451"></a><a href="查询PTR-Record列表.md">查询PTR Record列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p20992184618420"><a name="p20992184618420"></a><a name="p20992184618420"></a>查询租户弹性IP的PTR Record列表。</p>
</td>
</tr>
<tr id="row999218466419"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p14928843752"><a name="p14928843752"></a><a name="p14928843752"></a><a href="恢复PTR-Record默认值.md">恢复PTR Record默认值</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p999212467416"><a name="p999212467416"></a><a name="p999212467416"></a>将弹性IP的PTR Record恢复为默认值。</p>
</td>
</tr>
<tr id="row109921046548"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p592716430516"><a name="p592716430516"></a><a name="p592716430516"></a><a href="修改PTR-Record.md">修改PTR Record</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p999244617412"><a name="p999244617412"></a><a name="p999244617412"></a>修改弹性IP的PTR Record。</p>
</td>
</tr>
</tbody>
</table>

## TAG管理接口<a name="section15133512201219"></a>

TAG管理接口，用于为资源或实例添加、删除以及查询标签。

**表 8**  TAG管理接口

<a name="table13133191214123"></a>
<table><thead align="left"><tr id="row111337125123"><th class="cellrowborder" valign="top" width="34.42%" id="mcps1.2.3.1.1"><p id="p6133131210120"><a name="p6133131210120"></a><a name="p6133131210120"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="65.58%" id="mcps1.2.3.1.2"><p id="p4134161291216"><a name="p4134161291216"></a><a name="p4134161291216"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row41341012121210"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p122231621413"><a name="p122231621413"></a><a name="p122231621413"></a><a href="添加资源标签.md">添加资源标签</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0101702788_p3230987105511"><a name="zh-cn_topic_0101702788_p3230987105511"></a><a name="zh-cn_topic_0101702788_p3230987105511"></a>为指定实例添加标签。一个资源上最多有10个标签。</p>
</td>
</tr>
<tr id="row121342128126"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p1122119164143"><a name="p1122119164143"></a><a name="p1122119164143"></a><a href="删除资源标签.md">删除资源标签</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p1313471221217"><a name="p1313471221217"></a><a name="p1313471221217"></a>删除资源标签。</p>
</td>
</tr>
<tr id="row8134111216129"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p7221131611412"><a name="p7221131611412"></a><a name="p7221131611412"></a><a href="批量添加删除资源标签.md">批量添加删除资源标签</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0094510675_p3230987105511"><a name="zh-cn_topic_0094510675_p3230987105511"></a><a name="zh-cn_topic_0094510675_p3230987105511"></a>为指定实例批量添加或删除标签。</p>
</td>
</tr>
<tr id="row16134112111212"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p1722011611410"><a name="p1722011611410"></a><a name="p1722011611410"></a><a href="查询资源标签.md">查询资源标签</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p10134111219124"><a name="p10134111219124"></a><a name="p10134111219124"></a>查询指定实例的标签信息。</p>
</td>
</tr>
<tr id="row181352129121"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p919918166145"><a name="p919918166145"></a><a name="p919918166145"></a><a href="查询项目标签.md">查询项目标签</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p1313511125127"><a name="p1313511125127"></a><a name="p1313511125127"></a>查询指定实例类型的所有标签集合。</p>
</td>
</tr>
<tr id="row164429111147"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p17599817201513"><a name="p17599817201513"></a><a name="p17599817201513"></a><a href="查询资源实例.md">查询资源实例</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0123490185_p782982518031"><a name="zh-cn_topic_0123490185_p782982518031"></a><a name="zh-cn_topic_0123490185_p782982518031"></a>使用标签查询资源实例。资源实例按照创建时间倒序。</p>
</td>
</tr>
</tbody>
</table>

## 自定义线路管理接口<a name="section15811379181"></a>

自定义线路管理接口，用于创建、删除、更新以及查询自定义线路。

**表 9**  自定义线路管理接口

<a name="table1481113713184"></a>
<table><thead align="left"><tr id="row5821537121813"><th class="cellrowborder" valign="top" width="34.42%" id="mcps1.2.3.1.1"><p id="p1082103717187"><a name="p1082103717187"></a><a name="p1082103717187"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="65.58%" id="mcps1.2.3.1.2"><p id="p082437161820"><a name="p082437161820"></a><a name="p082437161820"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row20821137171812"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p672211568188"><a name="p672211568188"></a><a name="p672211568188"></a><a href="创建自定义线路.md">创建自定义线路</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p982123771816"><a name="p982123771816"></a><a name="p982123771816"></a>创建单个自定义线路。</p>
</td>
</tr>
<tr id="row782203717189"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p12721165613187"><a name="p12721165613187"></a><a name="p12721165613187"></a><a href="删除自定义线路.md">删除自定义线路</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p6829372189"><a name="p6829372189"></a><a name="p6829372189"></a>删除单个自定义线路。</p>
</td>
</tr>
<tr id="row382113717186"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p171915671817"><a name="p171915671817"></a><a name="p171915671817"></a><a href="更新自定义线路.md">更新自定义线路</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p983437101815"><a name="p983437101815"></a><a name="p983437101815"></a>更新单个自定义线路。</p>
</td>
</tr>
<tr id="row14831378181"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p16717105671810"><a name="p16717105671810"></a><a name="p16717105671810"></a><a href="查询自定义线路.md">查询自定义线路</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p18383791811"><a name="p18383791811"></a><a name="p18383791811"></a>查询自定义线路。</p>
</td>
</tr>
</tbody>
</table>

## 名称服务器管理接口<a name="section117821133165120"></a>

名称服务器管理接口，用于查询名称服务器列表。

**表 10**  名称服务器管理接口

<a name="table1678212331519"></a>
<table><thead align="left"><tr id="row11783123318519"><th class="cellrowborder" valign="top" width="34.42%" id="mcps1.2.3.1.1"><p id="p57831233165113"><a name="p57831233165113"></a><a name="p57831233165113"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="65.58%" id="mcps1.2.3.1.2"><p id="p17783183355111"><a name="p17783183355111"></a><a name="p17783183355111"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5783143311515"><td class="cellrowborder" valign="top" width="34.42%" headers="mcps1.2.3.1.1 "><p id="p4783163345116"><a name="p4783163345116"></a><a name="p4783163345116"></a><a href="查询名称服务器列表.md">查询名称服务器列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="65.58%" headers="mcps1.2.3.1.2 "><p id="p77831733105112"><a name="p77831733105112"></a><a name="p77831733105112"></a>查询名称服务器列表。</p>
</td>
</tr>
</tbody>
</table>

