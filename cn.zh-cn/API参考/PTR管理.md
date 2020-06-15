# PTR管理<a name="dns_api_70004"></a>

**表 1**  PTR管理

<a name="table930910161495"></a>
<table><thead align="left"><tr id="row1015517691"><th class="cellrowborder" valign="top" width="14.499999999999996%" id="mcps1.2.7.1.1"><p id="p0163172093"><a name="p0163172093"></a><a name="p0163172093"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="22.249999999999996%" id="mcps1.2.7.1.2"><p id="p18295111810169"><a name="p18295111810169"></a><a name="p18295111810169"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="15.419999999999998%" id="mcps1.2.7.1.3"><p id="p15509182516274"><a name="p15509182516274"></a><a name="p15509182516274"></a>授权项（Action）</p>
</th>
<th class="cellrowborder" valign="top" width="19.899999999999995%" id="mcps1.2.7.1.4"><p id="p675113518427"><a name="p675113518427"></a><a name="p675113518427"></a>依赖的授权项</p>
</th>
<th class="cellrowborder" valign="top" width="12.079999999999998%" id="mcps1.2.7.1.5"><p id="p1838971541713"><a name="p1838971541713"></a><a name="p1838971541713"></a>IAM项目<span>(Project)</span></p>
</th>
<th class="cellrowborder" valign="top" width="15.849999999999998%" id="mcps1.2.7.1.6"><p id="p475572121720"><a name="p475572121720"></a><a name="p475572121720"></a>企业项目<span>(Enterprise Project)</span></p>
</th>
</tr>
</thead>
<tbody><tr id="row12261717890"><td class="cellrowborder" valign="top" width="14.499999999999996%" headers="mcps1.2.7.1.1 "><p id="p1261171898"><a name="p1261171898"></a><a name="p1261171898"></a>设置PTR Record</p>
</td>
<td class="cellrowborder" valign="top" width="22.249999999999996%" headers="mcps1.2.7.1.2 "><p id="p19298418101615"><a name="p19298418101615"></a><a name="p19298418101615"></a>PATCH /v2/reverse/floatingips/{region}:{floatingip_id}</p>
</td>
<td class="cellrowborder" rowspan="4" valign="top" width="15.419999999999998%" headers="mcps1.2.7.1.3 "><p id="p105115258270"><a name="p105115258270"></a><a name="p105115258270"></a>dns:ptr:set</p>
</td>
<td class="cellrowborder" rowspan="4" valign="top" width="19.899999999999995%" headers="mcps1.2.7.1.4 "><p id="p1511425142710"><a name="p1511425142710"></a><a name="p1511425142710"></a>vpc:*:get*</p>
<p id="p15511122511278"><a name="p15511122511278"></a><a name="p15511122511278"></a>vpc:*:list*</p>
</td>
<td class="cellrowborder" rowspan="4" valign="top" width="12.079999999999998%" headers="mcps1.2.7.1.5 "><p id="p14634115734815"><a name="p14634115734815"></a><a name="p14634115734815"></a>√</p>
</td>
<td class="cellrowborder" rowspan="4" valign="top" width="15.849999999999998%" headers="mcps1.2.7.1.6 "><p id="p590919154912"><a name="p590919154912"></a><a name="p590919154912"></a>×</p>
</td>
</tr>
<tr id="row12271817997"><td class="cellrowborder" valign="top" headers="mcps1.2.7.1.1 "><p id="p82731720912"><a name="p82731720912"></a><a name="p82731720912"></a>修改PTR Record</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.7.1.2 "><p id="p1329918186169"><a name="p1329918186169"></a><a name="p1329918186169"></a>PATCH /v2/reverse/floatingips/{region}:{floatingip_id}</p>
</td>
</tr>
<tr id="row1282171998"><td class="cellrowborder" valign="top" headers="mcps1.2.7.1.1 "><p id="p132810171697"><a name="p132810171697"></a><a name="p132810171697"></a>恢复PTR Record默认值</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.7.1.2 "><p id="p929951811165"><a name="p929951811165"></a><a name="p929951811165"></a>PATCH /v2/reverse/floatingips/{region}:{floatingip_id}</p>
</td>
</tr>
<tr id="row3281817894"><td class="cellrowborder" valign="top" headers="mcps1.2.7.1.1 "><p id="p11283171795"><a name="p11283171795"></a><a name="p11283171795"></a>批量恢复PTR Record默认值</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.7.1.2 "><p id="p192991618111611"><a name="p192991618111611"></a><a name="p192991618111611"></a>DELETE /v2.1/reverse/floatingips</p>
</td>
</tr>
<tr id="row1128017892"><td class="cellrowborder" valign="top" width="14.499999999999996%" headers="mcps1.2.7.1.1 "><p id="p13291817092"><a name="p13291817092"></a><a name="p13291817092"></a>查询PTR Record</p>
</td>
<td class="cellrowborder" valign="top" width="22.249999999999996%" headers="mcps1.2.7.1.2 "><p id="p7299618151619"><a name="p7299618151619"></a><a name="p7299618151619"></a>GET /v2/reverse/floatingips/{region}:{floatingip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="15.419999999999998%" headers="mcps1.2.7.1.3 "><p id="p18512182532710"><a name="p18512182532710"></a><a name="p18512182532710"></a>dns:ptr:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.899999999999995%" headers="mcps1.2.7.1.4 "><p id="p10893148124814"><a name="p10893148124814"></a><a name="p10893148124814"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="12.079999999999998%" headers="mcps1.2.7.1.5 "><p id="p1549414491481"><a name="p1549414491481"></a><a name="p1549414491481"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.849999999999998%" headers="mcps1.2.7.1.6 "><p id="p192401255178"><a name="p192401255178"></a><a name="p192401255178"></a>×</p>
</td>
</tr>
<tr id="row829317297"><td class="cellrowborder" valign="top" width="14.499999999999996%" headers="mcps1.2.7.1.1 "><p id="p14297179912"><a name="p14297179912"></a><a name="p14297179912"></a>查询PTR Record列表</p>
</td>
<td class="cellrowborder" valign="top" width="22.249999999999996%" headers="mcps1.2.7.1.2 "><p id="p9299171815161"><a name="p9299171815161"></a><a name="p9299171815161"></a>GET /v2/reverse/floatingips</p>
</td>
<td class="cellrowborder" valign="top" width="15.419999999999998%" headers="mcps1.2.7.1.3 "><p id="p5512112532718"><a name="p5512112532718"></a><a name="p5512112532718"></a>dns:ptr:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.899999999999995%" headers="mcps1.2.7.1.4 "><p id="p2893280489"><a name="p2893280489"></a><a name="p2893280489"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="12.079999999999998%" headers="mcps1.2.7.1.5 "><p id="p11494749164818"><a name="p11494749164818"></a><a name="p11494749164818"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.849999999999998%" headers="mcps1.2.7.1.6 "><p id="p2240115111712"><a name="p2240115111712"></a><a name="p2240115111712"></a>×</p>
</td>
</tr>
</tbody>
</table>

