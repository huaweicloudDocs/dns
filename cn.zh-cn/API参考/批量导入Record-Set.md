# 批量导入Record Set<a name="ZH-CN_TOPIC_0130149199"></a>

## 功能介绍<a name="section18389930"></a>

上传导入文件，实现批量导入Record Set。

最大支持导入500条记录，超出部分不进行导入。

## URI<a name="section31291646"></a>

POST /v2/zones/\{zone\_id\}/import/recordsets

参数说明请参见[表1](#table21421675)。

**表 1**  URI格式的参数说明

<a name="table21421675"></a>
<table><thead align="left"><tr id="row9119245"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p461342"><a name="p461342"></a><a name="p461342"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p37368736"><a name="p37368736"></a><a name="p37368736"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p6968762"><a name="p6968762"></a><a name="p6968762"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row27598869"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p20915929"><a name="p20915929"></a><a name="p20915929"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p16468652"><a name="p16468652"></a><a name="p16468652"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p58892473"><a name="p58892473"></a><a name="p58892473"></a>所属zone的ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section13189358"></a>

-   参数说明

    **表 2**  请求消息头

    <a name="zh-cn_topic_0020536996_table2598811411913"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0020536996_row3248625511913"><th class="cellrowborder" valign="top" width="23.119999999999997%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0020536996_p6015991611913"><a name="zh-cn_topic_0020536996_p6015991611913"></a><a name="zh-cn_topic_0020536996_p6015991611913"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="11.27%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0020536996_p4111502811913"><a name="zh-cn_topic_0020536996_p4111502811913"></a><a name="zh-cn_topic_0020536996_p4111502811913"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.830000000000002%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0020536996_p4198298511913"><a name="zh-cn_topic_0020536996_p4198298511913"></a><a name="zh-cn_topic_0020536996_p4198298511913"></a>取值</p>
    </th>
    <th class="cellrowborder" valign="top" width="34.78%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0020536996_p4517861011913"><a name="zh-cn_topic_0020536996_p4517861011913"></a><a name="zh-cn_topic_0020536996_p4517861011913"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0020536996_row54513894165638"><td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020536996_p53549319165638"><a name="zh-cn_topic_0020536996_p53549319165638"></a><a name="zh-cn_topic_0020536996_p53549319165638"></a>Content-Type</p>
    </td>
    <td class="cellrowborder" valign="top" width="11.27%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0020536996_p42527621165638"><a name="zh-cn_topic_0020536996_p42527621165638"></a><a name="zh-cn_topic_0020536996_p42527621165638"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.830000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020536996_p22185287165638"><a name="zh-cn_topic_0020536996_p22185287165638"></a><a name="zh-cn_topic_0020536996_p22185287165638"></a>multipart/form-data</p>
    </td>
    <td class="cellrowborder" valign="top" width="34.78%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0020536996_p52177846165638"><a name="zh-cn_topic_0020536996_p52177846165638"></a><a name="zh-cn_topic_0020536996_p52177846165638"></a>发送的实体的MIME类型。此处为固定取值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020536996_row60029080165425"><td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0020536996_p30517305165425"><a name="zh-cn_topic_0020536996_p30517305165425"></a><a name="zh-cn_topic_0020536996_p30517305165425"></a>X-Auth-Token</p>
    </td>
    <td class="cellrowborder" valign="top" width="11.27%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0020536996_p23288801103741"><a name="zh-cn_topic_0020536996_p23288801103741"></a><a name="zh-cn_topic_0020536996_p23288801103741"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.830000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0020536996_p2488420216568"><a name="zh-cn_topic_0020536996_p2488420216568"></a><a name="zh-cn_topic_0020536996_p2488420216568"></a>用户获取的Token</p>
    </td>
    <td class="cellrowborder" valign="top" width="34.78%" headers="mcps1.2.5.1.4 "><p id="p47014103330"><a name="p47014103330"></a><a name="p47014103330"></a>用户Token。</p>
    </td>
    </tr>
    <tr id="row13918112451211"><td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.2.5.1.1 "><p id="p6918724161213"><a name="p6918724161213"></a><a name="p6918724161213"></a>X-Language</p>
    </td>
    <td class="cellrowborder" valign="top" width="11.27%" headers="mcps1.2.5.1.2 "><p id="p391832411218"><a name="p391832411218"></a><a name="p391832411218"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.830000000000002%" headers="mcps1.2.5.1.3 "><p id="p1391852481215"><a name="p1391852481215"></a><a name="p1391852481215"></a>zh-cn</p>
    </td>
    <td class="cellrowborder" valign="top" width="34.78%" headers="mcps1.2.5.1.4 "><p id="p807379194116"><a name="p807379194116"></a><a name="p807379194116"></a>导入模板所属语言。</p>
    <p id="p56820233173129"><a name="p56820233173129"></a><a name="p56820233173129"></a>取值范围：zh-cn（中文），en-us（英文）</p>
    <p id="p9551172105013"><a name="p9551172105013"></a><a name="p9551172105013"></a>默认为zh-cn。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  请求样例的Content-Disposition参数说明

    <a name="table3720408817742"></a>
    <table><thead align="left"><tr id="row6225671717742"><th class="cellrowborder" valign="top" id="mcps1.2.5.1.1"><p id="p12400633104015"><a name="p12400633104015"></a><a name="p12400633104015"></a>名称</p>
    </th>
    <th class="cellrowborder" colspan="2" valign="top" id="mcps1.2.5.1.2"><p id="p2395486519272"><a name="p2395486519272"></a><a name="p2395486519272"></a>取值</p>
    </th>
    <th class="cellrowborder" valign="top" id="mcps1.2.5.1.3"><p id="p5956810717742"><a name="p5956810717742"></a><a name="p5956810717742"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1329410717742"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p204001933194014"><a name="p204001933194014"></a><a name="p204001933194014"></a>Content-Disposition</p>
    </td>
    <td class="cellrowborder" colspan="2" valign="top" headers="mcps1.2.5.1.2 "><p id="p360216817742"><a name="p360216817742"></a><a name="p360216817742"></a>Content-Disposition: form-data; name="uploadfile"; filename="template.xlsx"</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><a name="ul87612054204116"></a><a name="ul87612054204116"></a><ul id="ul87612054204116"><li>form-data：固定取值。</li><li>name="uploadfile"，固定取值。</li><li>filename="template.xlsx"，设置为上传的文件名。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    -  请求消息头

    ```
    X-Auth-Token: token
    Content-Type: multipart/form-data; boundary=----WebKitFormBoundaryePkpFF7tjBAqx29L
    ```

    -  请求体

    ```
    ------WebKitFormBoundaryePkpFF7tjBAqx29L
    Content-Disposition: form-data; name="uploadfile"; filename="template.xlsx"
    Content-Type: application/x-object
    
    ... contents of file goes here ...
    ------WebKitFormBoundaryePkpFF7tjBAqx29L--
    ```


## 响应<a name="section51595365"></a>

-   参数说明

    **表 4**  响应样例的参数说明

    <a name="table28278595"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0037134404_row52466955175323"><th class="cellrowborder" valign="top" width="27.889999999999997%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0037134404_p2769858175323"><a name="zh-cn_topic_0037134404_p2769858175323"></a><a name="zh-cn_topic_0037134404_p2769858175323"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0037134404_p46296309175323"><a name="zh-cn_topic_0037134404_p46296309175323"></a><a name="zh-cn_topic_0037134404_p46296309175323"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.3%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0037134404_p62697904175323"><a name="zh-cn_topic_0037134404_p62697904175323"></a><a name="zh-cn_topic_0037134404_p62697904175323"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0037134404_row47909891175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p64112397175323"><a name="zh-cn_topic_0037134404_p64112397175323"></a><a name="zh-cn_topic_0037134404_p64112397175323"></a>task_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p1660870175323"><a name="zh-cn_topic_0037134404_p1660870175323"></a><a name="zh-cn_topic_0037134404_p1660870175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p1249204175323"><a name="zh-cn_topic_0037134404_p1249204175323"></a><a name="zh-cn_topic_0037134404_p1249204175323"></a>任务ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
      "task_id": "4011afa265b58e7a0165c12fde025c9c"
    }
    ```


## 返回值<a name="section61705107"></a>

请参考[通用请求返回值](通用请求返回值.md)。

