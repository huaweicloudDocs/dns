# 查询PTR Record<a name="dns_api_66003"></a>

## 功能介绍<a name="section18389930"></a>

查询单个弹性IP的PTR记录。

## URI<a name="section31291646"></a>

GET /v2/reverse/floatingips/\{region\}:\{floatingip\_id\}

参数说明请参见[表1](#table21421675)。

**表 1**  URI格式的参数说明

<a name="table21421675"></a>
<table><thead align="left"><tr id="rf5eb1b4b32f8403bb0acf9d017b51ee5"><th class="cellrowborder" valign="top" width="22.64%" id="mcps1.2.5.1.1"><p id="a3c7e1e08fe294e3e82e1797588253df5"><a name="a3c7e1e08fe294e3e82e1797588253df5"></a><a name="a3c7e1e08fe294e3e82e1797588253df5"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.37%" id="mcps1.2.5.1.2"><p id="adc5414917a3c400cb8857a02b29eb94d"><a name="adc5414917a3c400cb8857a02b29eb94d"></a><a name="adc5414917a3c400cb8857a02b29eb94d"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.3"><p id="a9ce61a6198d44964bdc496d82601e141"><a name="a9ce61a6198d44964bdc496d82601e141"></a><a name="a9ce61a6198d44964bdc496d82601e141"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.64%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0042318613_p517246718149"><a name="zh-cn_topic_0042318613_p517246718149"></a><a name="zh-cn_topic_0042318613_p517246718149"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="rfa1eb070d71448a9b2fbaa5917068657"><td class="cellrowborder" valign="top" width="22.64%" headers="mcps1.2.5.1.1 "><p id="ae661ce94166a4825a0aad48ed9e3a0e3"><a name="ae661ce94166a4825a0aad48ed9e3a0e3"></a><a name="ae661ce94166a4825a0aad48ed9e3a0e3"></a>region</p>
</td>
<td class="cellrowborder" valign="top" width="17.37%" headers="mcps1.2.5.1.2 "><p id="ac4b80f38e0ef4382be487f39931804d3"><a name="ac4b80f38e0ef4382be487f39931804d3"></a><a name="ac4b80f38e0ef4382be487f39931804d3"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="a0a1bf1099829467e967689705fc84fe5"><a name="a0a1bf1099829467e967689705fc84fe5"></a><a name="a0a1bf1099829467e967689705fc84fe5"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.64%" headers="mcps1.2.5.1.4 "><p id="a939d47bc868d44c290326fb1df4c5e00"><a name="a939d47bc868d44c290326fb1df4c5e00"></a><a name="a939d47bc868d44c290326fb1df4c5e00"></a>租户的区域信息。</p>
<p id="p5433349018149"><a name="p5433349018149"></a><a name="p5433349018149"></a>详细内容请参见<a href="终端节点（Endpoint）.md">终端节点（Endpoint）</a>。</p>
</td>
</tr>
<tr id="r0588e91c222b4483b97fe5b2e56f79bb"><td class="cellrowborder" valign="top" width="22.64%" headers="mcps1.2.5.1.1 "><p id="ac3563e9e05cc422ab54a9d288aa5810c"><a name="ac3563e9e05cc422ab54a9d288aa5810c"></a><a name="ac3563e9e05cc422ab54a9d288aa5810c"></a>floatingip_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.37%" headers="mcps1.2.5.1.2 "><p id="af475fd33d3fc4310b7f5a1f14e1fa9c9"><a name="af475fd33d3fc4310b7f5a1f14e1fa9c9"></a><a name="af475fd33d3fc4310b7f5a1f14e1fa9c9"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="a2fe0b089a6a14db1a241b4d93dc9fd5a"><a name="a2fe0b089a6a14db1a241b4d93dc9fd5a"></a><a name="a2fe0b089a6a14db1a241b4d93dc9fd5a"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.64%" headers="mcps1.2.5.1.4 "><p id="ad2fce4accef8431b86dcaca0bd572a60"><a name="ad2fce4accef8431b86dcaca0bd572a60"></a><a name="ad2fce4accef8431b86dcaca0bd572a60"></a>弹性IP的ID。</p>
<p id="p5553155134916"><a name="p5553155134916"></a><a name="p5553155134916"></a>可以通过网络控制台的弹性公网IP页面获取或者通过<a href="https://support.huaweicloud.com/api-eip/eip_api_0003.html" target="_blank" rel="noopener noreferrer">查询弹性公网IP列表</a>获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section13189358"></a>

-   请求参数

    无

-   请求样例

    查询ID为“c5504932-bf23-4171-b655-b87a6bc59334”的弹性IP的PTR。

    ```
    GET https://{DNS_Endpoint}/v2/reverse/floatingips/region_id:c5504932-bf23-4171-b655-b87a6bc59334
    ```


## 响应<a name="section51595365"></a>

-   参数说明

    **表 2**  响应样例的参数说明

    <a name="table28278595"></a>
    <table><thead align="left"><tr id="rc433fa5ceea44999bda6baae10282bed"><th class="cellrowborder" valign="top" width="18.23%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0042318613_p690539418456"><a name="zh-cn_topic_0042318613_p690539418456"></a><a name="zh-cn_topic_0042318613_p690539418456"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.139999999999997%" id="mcps1.2.4.1.2"><p id="aec3926ab378e4c9fafd96942ae9c2f24"><a name="aec3926ab378e4c9fafd96942ae9c2f24"></a><a name="aec3926ab378e4c9fafd96942ae9c2f24"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.629999999999995%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0042318613_p781187018456"><a name="zh-cn_topic_0042318613_p781187018456"></a><a name="zh-cn_topic_0042318613_p781187018456"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="rf59c1308b662423d9e5c5eb972f057a1"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="af1202b164f13422d896f91d34faf7c44"><a name="af1202b164f13422d896f91d34faf7c44"></a><a name="af1202b164f13422d896f91d34faf7c44"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.139999999999997%" headers="mcps1.2.4.1.2 "><p id="aa0e1ad68e67146a3a89bc538709063e9"><a name="aa0e1ad68e67146a3a89bc538709063e9"></a><a name="aa0e1ad68e67146a3a89bc538709063e9"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="a48e534dd79ef418ab79ff1303a8ff149"><a name="a48e534dd79ef418ab79ff1303a8ff149"></a><a name="a48e534dd79ef418ab79ff1303a8ff149"></a>PTR记录的ID，格式形如{region}:{floatingip_id}。</p>
    </td>
    </tr>
    <tr id="r8de792b7f9bb42a5bbd359fd67c55802"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="affabc5d973dd43ef8f81431cfbba2e4d"><a name="affabc5d973dd43ef8f81431cfbba2e4d"></a><a name="affabc5d973dd43ef8f81431cfbba2e4d"></a>ptrdname</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.139999999999997%" headers="mcps1.2.4.1.2 "><p id="a8d449d79abdf400cacc28050075effe9"><a name="a8d449d79abdf400cacc28050075effe9"></a><a name="a8d449d79abdf400cacc28050075effe9"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="a695a30773b7b4545a348899428360b0c"><a name="a695a30773b7b4545a348899428360b0c"></a><a name="a695a30773b7b4545a348899428360b0c"></a>PTR记录对应的域名。</p>
    </td>
    </tr>
    <tr id="r07959df68aa640f7b2550a4ec13bd321"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="a58edc66abfd94b8d88234ccc87f993ef"><a name="a58edc66abfd94b8d88234ccc87f993ef"></a><a name="a58edc66abfd94b8d88234ccc87f993ef"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.139999999999997%" headers="mcps1.2.4.1.2 "><p id="a585f5fc28a9746e0ae2a07ca866d0979"><a name="a585f5fc28a9746e0ae2a07ca866d0979"></a><a name="a585f5fc28a9746e0ae2a07ca866d0979"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="a26cda8d7c28c484a8555271f1b7c9c18"><a name="a26cda8d7c28c484a8555271f1b7c9c18"></a><a name="a26cda8d7c28c484a8555271f1b7c9c18"></a>对PTR记录的描述。</p>
    </td>
    </tr>
    <tr id="rc07302b7ba7748e2bd3ba03f66d4d046"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="ac280dc3e9e514cb4bb61dc356b75c265"><a name="ac280dc3e9e514cb4bb61dc356b75c265"></a><a name="ac280dc3e9e514cb4bb61dc356b75c265"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.139999999999997%" headers="mcps1.2.4.1.2 "><p id="a2faf54e82d504a619ab8183ab083c6f4"><a name="a2faf54e82d504a619ab8183ab083c6f4"></a><a name="a2faf54e82d504a619ab8183ab083c6f4"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p73714549431"><a name="p73714549431"></a><a name="p73714549431"></a>PTR记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="p1837175484310"><a name="p1837175484310"></a><a name="p1837175484310"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    <p id="a23cf8b6abe1245a294fde1b3cdc68e76"><a name="a23cf8b6abe1245a294fde1b3cdc68e76"></a><a name="a23cf8b6abe1245a294fde1b3cdc68e76"></a>取值范围：</p>
    <p id="abb10491c52064bc0a5fb65a66c645c01"><a name="abb10491c52064bc0a5fb65a66c645c01"></a><a name="abb10491c52064bc0a5fb65a66c645c01"></a>1～2147483647。</p>
    <p id="p1859919134417"><a name="p1859919134417"></a><a name="p1859919134417"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="rb0577738b87a4dafb23d0a1ef4cac7ed"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="a6c80427db35e48689eb4ae318fc8fa30"><a name="a6c80427db35e48689eb4ae318fc8fa30"></a><a name="a6c80427db35e48689eb4ae318fc8fa30"></a>address</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.139999999999997%" headers="mcps1.2.4.1.2 "><p id="aa917e102919f4ac98c625e33f516baee"><a name="aa917e102919f4ac98c625e33f516baee"></a><a name="aa917e102919f4ac98c625e33f516baee"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="a01a51f050f414b669b4a08478ede886e"><a name="a01a51f050f414b669b4a08478ede886e"></a><a name="a01a51f050f414b669b4a08478ede886e"></a>弹性IP的IP地址。</p>
    </td>
    </tr>
    <tr id="r9d3448295e68459db0bade4562e211a5"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="a29ee325b52134a3f847bbee5c91b1da3"><a name="a29ee325b52134a3f847bbee5c91b1da3"></a><a name="a29ee325b52134a3f847bbee5c91b1da3"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.139999999999997%" headers="mcps1.2.4.1.2 "><p id="a0db39a1fe84849a5b1a1e8b334e41e5b"><a name="a0db39a1fe84849a5b1a1e8b334e41e5b"></a><a name="a0db39a1fe84849a5b1a1e8b334e41e5b"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="a133beb6a97ed42bdac622271072840e6"><a name="a133beb6a97ed42bdac622271072840e6"></a><a name="a133beb6a97ed42bdac622271072840e6"></a>资源状态。</p>
    <p id="zh-cn_topic_0042318613_p55966391353"><a name="zh-cn_topic_0042318613_p55966391353"></a><a name="zh-cn_topic_0042318613_p55966391353"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="rb4683cb844214f51ae468943568b4cde"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="a1d911558e18444b3896ace2ed6ccbaec"><a name="a1d911558e18444b3896ace2ed6ccbaec"></a><a name="a1d911558e18444b3896ace2ed6ccbaec"></a>action</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.139999999999997%" headers="mcps1.2.4.1.2 "><p id="ae39f64d2c5af4dae91b509416f77d31d"><a name="ae39f64d2c5af4dae91b509416f77d31d"></a><a name="ae39f64d2c5af4dae91b509416f77d31d"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0042318613_p507362318456"><a name="zh-cn_topic_0042318613_p507362318456"></a><a name="zh-cn_topic_0042318613_p507362318456"></a>对该资源的当前操作。</p>
    <p id="a7560251cd28e4dd9b678da457820ee30"><a name="a7560251cd28e4dd9b678da457820ee30"></a><a name="a7560251cd28e4dd9b678da457820ee30"></a>取值范围：CREATE，UPDATE，DELETE，NONE</p>
    <p id="zh-cn_topic_0042318613_p178601911399"><a name="zh-cn_topic_0042318613_p178601911399"></a><a name="zh-cn_topic_0042318613_p178601911399"></a>CREATE：表示创建，UPDATE：表示更新，DELETE：表示删除，NONE：表示无操作</p>
    </td>
    </tr>
    <tr id="re6d739b3d80f4bcda0e2ad834dc1d66f"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0042318613_p204899518456"><a name="zh-cn_topic_0042318613_p204899518456"></a><a name="zh-cn_topic_0042318613_p204899518456"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.139999999999997%" headers="mcps1.2.4.1.2 "><p id="ad894d21cefa74634a62f6964f84019f6"><a name="ad894d21cefa74634a62f6964f84019f6"></a><a name="ad894d21cefa74634a62f6964f84019f6"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="ab163171b57cd4600a059890e5f4373ce"><a name="ab163171b57cd4600a059890e5f4373ce"></a><a name="ab163171b57cd4600a059890e5f4373ce"></a>指向当前资源或者其他相关资源的链接。</p>
    <p id="a4dc7ac60268d4291a27544e93c236e22"><a name="a4dc7ac60268d4291a27544e93c236e22"></a><a name="a4dc7ac60268d4291a27544e93c236e22"></a>当响应需要分页时，需要包含一个next链接来进行分页。详细信息请参见<a href="#table354521744216">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  links参数说明

    <a name="table354521744216"></a>
    <table><thead align="left"><tr id="row954518179427"><th class="cellrowborder" valign="top" width="18.3018301830183%" id="mcps1.2.4.1.1"><p id="p654513173424"><a name="p654513173424"></a><a name="p654513173424"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.591959195919593%" id="mcps1.2.4.1.2"><p id="p654551714212"><a name="p654551714212"></a><a name="p654551714212"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.10621062106211%" id="mcps1.2.4.1.3"><p id="p1545141717427"><a name="p1545141717427"></a><a name="p1545141717427"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3545101710429"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p115467171428"><a name="p115467171428"></a><a name="p115467171428"></a>self</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.591959195919593%" headers="mcps1.2.4.1.2 "><p id="p254611713427"><a name="p254611713427"></a><a name="p254611713427"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.10621062106211%" headers="mcps1.2.4.1.3 "><p id="p5546171744214"><a name="p5546171744214"></a><a name="p5546171744214"></a>当前资源的链接。</p>
    </td>
    </tr>
    <tr id="row2458163435118"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.591959195919593%" headers="mcps1.2.4.1.2 "><p id="p19656144517367"><a name="p19656144517367"></a><a name="p19656144517367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.10621062106211%" headers="mcps1.2.4.1.3 "><p id="p76567451365"><a name="p76567451365"></a><a name="p76567451365"></a>下一页资源的链接。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "id": "region_id:c5504932-bf23-4171-b655-b87a6bc59334",
        "ptrdname": "www.example.com.",
        "description": "Description for this PTR record",
        "address": "10.154.52.138",
        "action": "CREATE",
        "ttl": 300,
        "status": "ACTIVE",
        "links": {
            "self": "https://Endpoint/v2/reverse/floatingips/region_id:c5504932-bf23-4171-b655-b87a6bc59334"
        }
    }
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

