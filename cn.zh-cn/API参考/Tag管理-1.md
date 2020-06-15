# Tag管理<a name="dns_api_70005"></a>

**表 1**  Tag管理

<a name="table930910161495"></a>
<table><thead align="left"><tr id="row1015517691"><th class="cellrowborder" valign="top" width="14.78%" id="mcps1.2.7.1.1"><p id="p0163172093"><a name="p0163172093"></a><a name="p0163172093"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="21.959999999999997%" id="mcps1.2.7.1.2"><p id="p18295111810169"><a name="p18295111810169"></a><a name="p18295111810169"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="15.35%" id="mcps1.2.7.1.3"><p id="p15509182516274"><a name="p15509182516274"></a><a name="p15509182516274"></a>授权项（Action）</p>
</th>
<th class="cellrowborder" valign="top" width="19.900000000000002%" id="mcps1.2.7.1.4"><p id="p94009499502"><a name="p94009499502"></a><a name="p94009499502"></a>依赖的授权项</p>
</th>
<th class="cellrowborder" valign="top" width="11.940000000000001%" id="mcps1.2.7.1.5"><p id="p1838971541713"><a name="p1838971541713"></a><a name="p1838971541713"></a>IAM项目</p>
<p id="p93891815181714"><a name="p93891815181714"></a><a name="p93891815181714"></a><span>(Project)</span></p>
</th>
<th class="cellrowborder" valign="top" width="16.07%" id="mcps1.2.7.1.6"><p id="p475572121720"><a name="p475572121720"></a><a name="p475572121720"></a>企业项目<span>(Enterprise Project)</span></p>
</th>
</tr>
</thead>
<tbody><tr id="row10301317997"><td class="cellrowborder" valign="top" width="14.78%" headers="mcps1.2.7.1.1 "><p id="p193014171397"><a name="p193014171397"></a><a name="p193014171397"></a>添加资源标签</p>
</td>
<td class="cellrowborder" valign="top" width="21.959999999999997%" headers="mcps1.2.7.1.2 "><p id="p4299131871615"><a name="p4299131871615"></a><a name="p4299131871615"></a>POST /v2/{project_id}/{resource_type}/{resource_id}/tags</p>
</td>
<td class="cellrowborder" rowspan="3" valign="top" width="15.35%" headers="mcps1.2.7.1.3 "><p id="p55122025112715"><a name="p55122025112715"></a><a name="p55122025112715"></a>dns:tag:set</p>
</td>
<td class="cellrowborder" rowspan="3" valign="top" width="19.900000000000002%" headers="mcps1.2.7.1.4 "><p id="p859344013514"><a name="p859344013514"></a><a name="p859344013514"></a>-</p>
</td>
<td class="cellrowborder" rowspan="3" valign="top" width="11.940000000000001%" headers="mcps1.2.7.1.5 "><p id="p17588650165114"><a name="p17588650165114"></a><a name="p17588650165114"></a>√</p>
</td>
<td class="cellrowborder" rowspan="3" valign="top" width="16.07%" headers="mcps1.2.7.1.6 "><p id="p982365825119"><a name="p982365825119"></a><a name="p982365825119"></a>×</p>
</td>
</tr>
<tr id="row831517395"><td class="cellrowborder" valign="top" headers="mcps1.2.7.1.1 "><p id="p11316173913"><a name="p11316173913"></a><a name="p11316173913"></a>批量添加删除资源标签</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.7.1.2 "><p id="p1029951818161"><a name="p1029951818161"></a><a name="p1029951818161"></a>POST /v2/{project_id}/{resource_type}/{resource_id}/tags/action</p>
</td>
</tr>
<tr id="row11311417194"><td class="cellrowborder" valign="top" headers="mcps1.2.7.1.1 "><p id="p53111720913"><a name="p53111720913"></a><a name="p53111720913"></a>删除资源标签</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.7.1.2 "><p id="p12299201861615"><a name="p12299201861615"></a><a name="p12299201861615"></a>DELETE /v2/{project_id}/{resource_type}/{resource_id}/tags/{key}</p>
</td>
</tr>
<tr id="row2313177914"><td class="cellrowborder" valign="top" width="14.78%" headers="mcps1.2.7.1.1 "><p id="p18311317497"><a name="p18311317497"></a><a name="p18311317497"></a>查询资源标签</p>
</td>
<td class="cellrowborder" valign="top" width="21.959999999999997%" headers="mcps1.2.7.1.2 "><p id="p1299101818163"><a name="p1299101818163"></a><a name="p1299101818163"></a>GET /v2/{project_id}/{resource_type}/{resource_id}/tags</p>
</td>
<td class="cellrowborder" rowspan="3" valign="top" width="15.35%" headers="mcps1.2.7.1.3 "><p id="p851262522715"><a name="p851262522715"></a><a name="p851262522715"></a>dns:tag:get</p>
</td>
<td class="cellrowborder" rowspan="3" valign="top" width="19.900000000000002%" headers="mcps1.2.7.1.4 "><p id="p13584123615116"><a name="p13584123615116"></a><a name="p13584123615116"></a>-</p>
</td>
<td class="cellrowborder" rowspan="3" valign="top" width="11.940000000000001%" headers="mcps1.2.7.1.5 "><p id="p174151953175116"><a name="p174151953175116"></a><a name="p174151953175116"></a>√</p>
</td>
<td class="cellrowborder" rowspan="3" valign="top" width="16.07%" headers="mcps1.2.7.1.6 "><p id="p7341756205115"><a name="p7341756205115"></a><a name="p7341756205115"></a>×</p>
</td>
</tr>
<tr id="row173219171992"><td class="cellrowborder" valign="top" headers="mcps1.2.7.1.1 "><p id="p123221712917"><a name="p123221712917"></a><a name="p123221712917"></a>查询项目标签</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.7.1.2 "><p id="p5299718171612"><a name="p5299718171612"></a><a name="p5299718171612"></a>GET /v2/{project_id}/{resource_type}/tags</p>
</td>
</tr>
<tr id="row17323171397"><td class="cellrowborder" valign="top" headers="mcps1.2.7.1.1 "><p id="p173210171594"><a name="p173210171594"></a><a name="p173210171594"></a>查询资源实例</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.7.1.2 "><p id="p19299618171612"><a name="p19299618171612"></a><a name="p19299618171612"></a>POST /v2/{project_id}/{resource_type}/resource_instances/action</p>
</td>
</tr>
</tbody>
</table>

