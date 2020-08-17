# Zone管理<a name="dns_api_70002"></a>

**表 1**  Zone管理

<a name="table930910161495"></a>
<table><thead align="left"><tr id="row1015517691"><th class="cellrowborder" valign="top" width="14.500000000000002%" id="mcps1.2.7.1.1"><p id="p0163172093"><a name="p0163172093"></a><a name="p0163172093"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="21.750000000000004%" id="mcps1.2.7.1.2"><p id="p18295111810169"><a name="p18295111810169"></a><a name="p18295111810169"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="15.420000000000003%" id="mcps1.2.7.1.3"><p id="p15509182516274"><a name="p15509182516274"></a><a name="p15509182516274"></a>授权项（Action）</p>
</th>
<th class="cellrowborder" valign="top" width="20.330000000000005%" id="mcps1.2.7.1.4"><p id="p14675557351"><a name="p14675557351"></a><a name="p14675557351"></a>依赖的授权项</p>
</th>
<th class="cellrowborder" valign="top" width="12.15%" id="mcps1.2.7.1.5"><p id="p1838971541713"><a name="p1838971541713"></a><a name="p1838971541713"></a>IAM项目<span>(Project)</span></p>
</th>
<th class="cellrowborder" valign="top" width="15.850000000000003%" id="mcps1.2.7.1.6"><p id="p475572121720"><a name="p475572121720"></a><a name="p475572121720"></a>企业项目<span>(Enterprise Project)</span></p>
</th>
</tr>
</thead>
<tbody><tr id="row816141720910"><td class="cellrowborder" valign="top" width="14.500000000000002%" headers="mcps1.2.7.1.1 "><p id="p816817399"><a name="p816817399"></a><a name="p816817399"></a>创建Zone</p>
</td>
<td class="cellrowborder" valign="top" width="21.750000000000004%" headers="mcps1.2.7.1.2 "><p id="p4295151831614"><a name="p4295151831614"></a><a name="p4295151831614"></a>POST /v2/zones</p>
</td>
<td class="cellrowborder" valign="top" width="15.420000000000003%" headers="mcps1.2.7.1.3 "><p id="p1950911259278"><a name="p1950911259278"></a><a name="p1950911259278"></a>dns:zone:create</p>
</td>
<td class="cellrowborder" valign="top" width="20.330000000000005%" headers="mcps1.2.7.1.4 "><p id="p125091625132717"><a name="p125091625132717"></a><a name="p125091625132717"></a>vpc:*:get*</p>
<p id="p105091825132714"><a name="p105091825132714"></a><a name="p105091825132714"></a>vpc:*:list*</p>
</td>
<td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.5 "><p id="p1523614642915"><a name="p1523614642915"></a><a name="p1523614642915"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.850000000000003%" headers="mcps1.2.7.1.6 "><p id="p1723612615292"><a name="p1723612615292"></a><a name="p1723612615292"></a>×</p>
</td>
</tr>
<tr id="row161618171099"><td class="cellrowborder" valign="top" width="14.500000000000002%" headers="mcps1.2.7.1.1 "><p id="p816217698"><a name="p816217698"></a><a name="p816217698"></a>查询Zone</p>
</td>
<td class="cellrowborder" valign="top" width="21.750000000000004%" headers="mcps1.2.7.1.2 "><p id="p829516185163"><a name="p829516185163"></a><a name="p829516185163"></a>GET /v2/zones/{zone_id}</p>
</td>
<td class="cellrowborder" valign="top" width="15.420000000000003%" headers="mcps1.2.7.1.3 "><p id="p750918259272"><a name="p750918259272"></a><a name="p750918259272"></a>dns:zone:get</p>
</td>
<td class="cellrowborder" valign="top" width="20.330000000000005%" headers="mcps1.2.7.1.4 "><p id="p13695154083516"><a name="p13695154083516"></a><a name="p13695154083516"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.5 "><p id="p822715113282"><a name="p822715113282"></a><a name="p822715113282"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.850000000000003%" headers="mcps1.2.7.1.6 "><p id="p5238135191716"><a name="p5238135191716"></a><a name="p5238135191716"></a>×</p>
</td>
</tr>
<tr id="row2169177920"><td class="cellrowborder" valign="top" width="14.500000000000002%" headers="mcps1.2.7.1.1 "><p id="p5165171595"><a name="p5165171595"></a><a name="p5165171595"></a>查询Zone列表</p>
</td>
<td class="cellrowborder" valign="top" width="21.750000000000004%" headers="mcps1.2.7.1.2 "><p id="p929616182162"><a name="p929616182162"></a><a name="p929616182162"></a>GET /v2/zones</p>
</td>
<td class="cellrowborder" valign="top" width="15.420000000000003%" headers="mcps1.2.7.1.3 "><p id="p115091925132711"><a name="p115091925132711"></a><a name="p115091925132711"></a>dns:zone:list</p>
</td>
<td class="cellrowborder" valign="top" width="20.330000000000005%" headers="mcps1.2.7.1.4 "><p id="p169534063515"><a name="p169534063515"></a><a name="p169534063515"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.5 "><p id="p123772911293"><a name="p123772911293"></a><a name="p123772911293"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.850000000000003%" headers="mcps1.2.7.1.6 "><p id="p737710918291"><a name="p737710918291"></a><a name="p737710918291"></a>×</p>
</td>
</tr>
<tr id="row41610171697"><td class="cellrowborder" valign="top" width="14.500000000000002%" headers="mcps1.2.7.1.1 "><p id="p17169170919"><a name="p17169170919"></a><a name="p17169170919"></a>更新Zone</p>
</td>
<td class="cellrowborder" valign="top" width="21.750000000000004%" headers="mcps1.2.7.1.2 "><p id="p42969184169"><a name="p42969184169"></a><a name="p42969184169"></a>PATCH /v2/zones/{zone_id}</p>
</td>
<td class="cellrowborder" valign="top" width="15.420000000000003%" headers="mcps1.2.7.1.3 "><p id="p850916254277"><a name="p850916254277"></a><a name="p850916254277"></a>dns:zone:update</p>
</td>
<td class="cellrowborder" valign="top" width="20.330000000000005%" headers="mcps1.2.7.1.4 "><p id="p17695104015355"><a name="p17695104015355"></a><a name="p17695104015355"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.5 "><p id="p7564111317292"><a name="p7564111317292"></a><a name="p7564111317292"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.850000000000003%" headers="mcps1.2.7.1.6 "><p id="p1256417137291"><a name="p1256417137291"></a><a name="p1256417137291"></a>×</p>
</td>
</tr>
<tr id="row18832111108"><td class="cellrowborder" valign="top" width="14.500000000000002%" headers="mcps1.2.7.1.1 "><p id="p588416114010"><a name="p588416114010"></a><a name="p588416114010"></a>设置Zone状态</p>
</td>
<td class="cellrowborder" valign="top" width="21.750000000000004%" headers="mcps1.2.7.1.2 "><p id="p4296518121618"><a name="p4296518121618"></a><a name="p4296518121618"></a>PUT /v2/zones/{zone_id}/statuses</p>
</td>
<td class="cellrowborder" valign="top" width="15.420000000000003%" headers="mcps1.2.7.1.3 "><p id="p85106255272"><a name="p85106255272"></a><a name="p85106255272"></a>dns:zone:setStatus</p>
</td>
<td class="cellrowborder" valign="top" width="20.330000000000005%" headers="mcps1.2.7.1.4 "><p id="p9695144003512"><a name="p9695144003512"></a><a name="p9695144003512"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.5 "><p id="p133271714192913"><a name="p133271714192913"></a><a name="p133271714192913"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.850000000000003%" headers="mcps1.2.7.1.6 "><p id="p53276144297"><a name="p53276144297"></a><a name="p53276144297"></a>×</p>
</td>
</tr>
<tr id="row101601713910"><td class="cellrowborder" valign="top" width="14.500000000000002%" headers="mcps1.2.7.1.1 "><p id="p116181713910"><a name="p116181713910"></a><a name="p116181713910"></a>删除Zone</p>
</td>
<td class="cellrowborder" valign="top" width="21.750000000000004%" headers="mcps1.2.7.1.2 "><p id="p1929611810161"><a name="p1929611810161"></a><a name="p1929611810161"></a>DELETE /v2/zones/{zone_id}</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="15.420000000000003%" headers="mcps1.2.7.1.3 "><p id="p7510625102717"><a name="p7510625102717"></a><a name="p7510625102717"></a>dns:zone:delete</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="20.330000000000005%" headers="mcps1.2.7.1.4 "><p id="p1351015258279"><a name="p1351015258279"></a><a name="p1351015258279"></a>ces:remoteChecks:list</p>
<p id="p125101625152717"><a name="p125101625152717"></a><a name="p125101625152717"></a>ces:siteMonitorHealthCheck:get</p>
<p id="p3510122592717"><a name="p3510122592717"></a><a name="p3510122592717"></a>ces:siteMonitorHealthCheck:create</p>
<p id="p145104254272"><a name="p145104254272"></a><a name="p145104254272"></a>ces:siteMonitorRule:delete</p>
<p id="p9510182512273"><a name="p9510182512273"></a><a name="p9510182512273"></a>ces:siteMonitorRule:put</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="12.15%" headers="mcps1.2.7.1.5 "><p id="p7595181542911"><a name="p7595181542911"></a><a name="p7595181542911"></a>√</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="15.850000000000003%" headers="mcps1.2.7.1.6 "><p id="p1459561518299"><a name="p1459561518299"></a><a name="p1459561518299"></a>×</p>
</td>
</tr>
<tr id="row171616171294"><td class="cellrowborder" valign="top" headers="mcps1.2.7.1.1 "><p id="p91618172092"><a name="p91618172092"></a><a name="p91618172092"></a>批量删除Zone</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.7.1.2 "><p id="p1929671819165"><a name="p1929671819165"></a><a name="p1929671819165"></a>DELETE /v2.1/zones</p>
</td>
</tr>
<tr id="row19169178918"><td class="cellrowborder" valign="top" width="14.500000000000002%" headers="mcps1.2.7.1.1 "><p id="p816131712914"><a name="p816131712914"></a><a name="p816131712914"></a>内网Zone关联VPC</p>
</td>
<td class="cellrowborder" valign="top" width="21.750000000000004%" headers="mcps1.2.7.1.2 "><p id="p15296151831613"><a name="p15296151831613"></a><a name="p15296151831613"></a>POST /v2/zones/{zone_id}/associaterouter</p>
</td>
<td class="cellrowborder" valign="top" width="15.420000000000003%" headers="mcps1.2.7.1.3 "><p id="p1651042512279"><a name="p1651042512279"></a><a name="p1651042512279"></a>dns:zone:associaterouter</p>
</td>
<td class="cellrowborder" valign="top" width="20.330000000000005%" headers="mcps1.2.7.1.4 "><p id="p1351092518271"><a name="p1351092518271"></a><a name="p1351092518271"></a>vpc:*:get*</p>
<p id="p1151092532711"><a name="p1151092532711"></a><a name="p1151092532711"></a>vpc:*:list*</p>
</td>
<td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.5 "><p id="p155111917152912"><a name="p155111917152912"></a><a name="p155111917152912"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.850000000000003%" headers="mcps1.2.7.1.6 "><p id="p16511171715299"><a name="p16511171715299"></a><a name="p16511171715299"></a>×</p>
</td>
</tr>
<tr id="row20161177915"><td class="cellrowborder" valign="top" width="14.500000000000002%" headers="mcps1.2.7.1.1 "><p id="p1161817891"><a name="p1161817891"></a><a name="p1161817891"></a>内网Zone解关联VPC</p>
</td>
<td class="cellrowborder" valign="top" width="21.750000000000004%" headers="mcps1.2.7.1.2 "><p id="p529691811616"><a name="p529691811616"></a><a name="p529691811616"></a>POST /v2/zones/{zone_id}/disassociaterouter</p>
</td>
<td class="cellrowborder" valign="top" width="15.420000000000003%" headers="mcps1.2.7.1.3 "><p id="p651082582712"><a name="p651082582712"></a><a name="p651082582712"></a>dns:zone:disassociaterouter</p>
</td>
<td class="cellrowborder" valign="top" width="20.330000000000005%" headers="mcps1.2.7.1.4 "><p id="p751011258279"><a name="p751011258279"></a><a name="p751011258279"></a>vpc:*:get*</p>
<p id="p175101525102711"><a name="p175101525102711"></a><a name="p175101525102711"></a>vpc:*:list*</p>
</td>
<td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.5 "><p id="p150081812298"><a name="p150081812298"></a><a name="p150081812298"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.850000000000003%" headers="mcps1.2.7.1.6 "><p id="p9500151802912"><a name="p9500151802912"></a><a name="p9500151802912"></a>×</p>
</td>
</tr>
<tr id="row6165171498"><td class="cellrowborder" valign="top" width="14.500000000000002%" headers="mcps1.2.7.1.1 "><p id="p171611171897"><a name="p171611171897"></a><a name="p171611171897"></a>创建公网域名找回</p>
</td>
<td class="cellrowborder" valign="top" width="21.750000000000004%" headers="mcps1.2.7.1.2 "><p id="p17296318131620"><a name="p17296318131620"></a><a name="p17296318131620"></a>POST /v2/retrieval</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="15.420000000000003%" headers="mcps1.2.7.1.3 "><p id="p12510172582714"><a name="p12510172582714"></a><a name="p12510172582714"></a>dns:zone:createRetrieval</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="20.330000000000005%" headers="mcps1.2.7.1.4 "><p id="p856155310367"><a name="p856155310367"></a><a name="p856155310367"></a>-</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="12.15%" headers="mcps1.2.7.1.5 "><p id="p5925171922915"><a name="p5925171922915"></a><a name="p5925171922915"></a>√</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="15.850000000000003%" headers="mcps1.2.7.1.6 "><p id="p09252198291"><a name="p09252198291"></a><a name="p09252198291"></a>×</p>
</td>
</tr>
<tr id="row1216181718919"><td class="cellrowborder" valign="top" headers="mcps1.2.7.1.1 "><p id="p1517181719918"><a name="p1517181719918"></a><a name="p1517181719918"></a>请求立即验证公网域名找回</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.7.1.2 "><p id="p132961118191610"><a name="p132961118191610"></a><a name="p132961118191610"></a>POST /v2/retrieval/verification/{id}</p>
</td>
</tr>
<tr id="row5171817995"><td class="cellrowborder" valign="top" width="14.500000000000002%" headers="mcps1.2.7.1.1 "><p id="p1117171717920"><a name="p1117171717920"></a><a name="p1117171717920"></a>查询公网域名找回</p>
</td>
<td class="cellrowborder" valign="top" width="21.750000000000004%" headers="mcps1.2.7.1.2 "><p id="p629711183168"><a name="p629711183168"></a><a name="p629711183168"></a>GET /v2/retrieval</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="15.420000000000003%" headers="mcps1.2.7.1.3 "><p id="p205101725102713"><a name="p205101725102713"></a><a name="p205101725102713"></a>dns:zone:getRetrieval</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="20.330000000000005%" headers="mcps1.2.7.1.4 "><p id="p137915530391"><a name="p137915530391"></a><a name="p137915530391"></a>-</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="12.15%" headers="mcps1.2.7.1.5 "><p id="p548814218294"><a name="p548814218294"></a><a name="p548814218294"></a>√</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="15.850000000000003%" headers="mcps1.2.7.1.6 "><p id="p54881521112910"><a name="p54881521112910"></a><a name="p54881521112910"></a>×</p>
</td>
</tr>
<tr id="row317121716920"><td class="cellrowborder" valign="top" headers="mcps1.2.7.1.1 "><p id="p13171017696"><a name="p13171017696"></a><a name="p13171017696"></a>查询公网域名找回结果</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.7.1.2 "><p id="p1829717186169"><a name="p1829717186169"></a><a name="p1829717186169"></a>GET /v2/retrieval/verification/{id}</p>
</td>
</tr>
<tr id="row1218917893"><td class="cellrowborder" valign="top" width="14.500000000000002%" headers="mcps1.2.7.1.1 "><p id="p61811171393"><a name="p61811171393"></a><a name="p61811171393"></a>导出Zone</p>
</td>
<td class="cellrowborder" valign="top" width="21.750000000000004%" headers="mcps1.2.7.1.2 "><p id="p429701841619"><a name="p429701841619"></a><a name="p429701841619"></a>GET /v2/zones/{zone_id}/export</p>
</td>
<td class="cellrowborder" valign="top" width="15.420000000000003%" headers="mcps1.2.7.1.3 "><p id="p5510122513271"><a name="p5510122513271"></a><a name="p5510122513271"></a>dns:zone:getExport</p>
</td>
<td class="cellrowborder" valign="top" width="20.330000000000005%" headers="mcps1.2.7.1.4 "><p id="p7695164043512"><a name="p7695164043512"></a><a name="p7695164043512"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.5 "><p id="p1591422122912"><a name="p1591422122912"></a><a name="p1591422122912"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.850000000000003%" headers="mcps1.2.7.1.6 "><p id="p2091122218297"><a name="p2091122218297"></a><a name="p2091122218297"></a>×</p>
</td>
</tr>
</tbody>
</table>

