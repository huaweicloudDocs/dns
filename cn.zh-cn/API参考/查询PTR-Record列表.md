# 查询PTR Record列表<a name="zh-cn_topic_0042318615"></a>

## 功能介绍<a name="section29105235"></a>

查询租户弹性IP的PTR记录列表。

## URI<a name="section60620523"></a>

GET /v2/reverse/floatingips?limit=\{limit\}&marker=\{marker\}&offset=\{offset\}&tags=\{tags\}

参数说明请参见[表1](#table1562846014112)。

**表 1**  URI格式的参数说明

<a name="table1562846014112"></a>
<table><thead align="left"><tr id="r6ac32cd36c6440bd8ac6087ceb16d5cc"><th class="cellrowborder" valign="top" width="16.62166216621662%" id="mcps1.2.5.1.1"><p id="a4e323cd7393046cf818209af891ceb09"><a name="a4e323cd7393046cf818209af891ceb09"></a><a name="a4e323cd7393046cf818209af891ceb09"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.921592159215923%" id="mcps1.2.5.1.2"><p id="a8a575925321445698046900da989bc3f"><a name="a8a575925321445698046900da989bc3f"></a><a name="a8a575925321445698046900da989bc3f"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.01170117011701%" id="mcps1.2.5.1.3"><p id="a059da88b19b84eb8b75f8e366f39b709"><a name="a059da88b19b84eb8b75f8e366f39b709"></a><a name="a059da88b19b84eb8b75f8e366f39b709"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50.44504450445044%" id="mcps1.2.5.1.4"><p id="a10e66b0b45c64f42a71a62a3052a263a"><a name="a10e66b0b45c64f42a71a62a3052a263a"></a><a name="a10e66b0b45c64f42a71a62a3052a263a"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="r6efd36b450494483b222910e404b1e6a"><td class="cellrowborder" valign="top" width="16.62166216621662%" headers="mcps1.2.5.1.1 "><p id="a7f00431d42ae407e9b0e4d81c5938835"><a name="a7f00431d42ae407e9b0e4d81c5938835"></a><a name="a7f00431d42ae407e9b0e4d81c5938835"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="15.921592159215923%" headers="mcps1.2.5.1.2 "><p id="ad6af330a24be43aa9721d334a5175266"><a name="ad6af330a24be43aa9721d334a5175266"></a><a name="ad6af330a24be43aa9721d334a5175266"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.01170117011701%" headers="mcps1.2.5.1.3 "><p id="a6a5ec28098714553b4b375b27253f5a3"><a name="a6a5ec28098714553b4b375b27253f5a3"></a><a name="a6a5ec28098714553b4b375b27253f5a3"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.44504450445044%" headers="mcps1.2.5.1.4 "><p id="a5e11749436c54f85807503bca7950ef0"><a name="a5e11749436c54f85807503bca7950ef0"></a><a name="a5e11749436c54f85807503bca7950ef0"></a>分页查询起始的资源ID，为空时为查询第一页。</p>
<p id="p64815261440"><a name="p64815261440"></a><a name="p64815261440"></a>默认值为空。</p>
</td>
</tr>
<tr id="r4be7a5418c324afd9a5d1bfaccccc5a2"><td class="cellrowborder" valign="top" width="16.62166216621662%" headers="mcps1.2.5.1.1 "><p id="a473baa503056414f89deaa313549266d"><a name="a473baa503056414f89deaa313549266d"></a><a name="a473baa503056414f89deaa313549266d"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="15.921592159215923%" headers="mcps1.2.5.1.2 "><p id="a704b39f2d90b445b96e210fa5803b4be"><a name="a704b39f2d90b445b96e210fa5803b4be"></a><a name="a704b39f2d90b445b96e210fa5803b4be"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.01170117011701%" headers="mcps1.2.5.1.3 "><p id="a883425368cca4e889138f0f3a93c3850"><a name="a883425368cca4e889138f0f3a93c3850"></a><a name="a883425368cca4e889138f0f3a93c3850"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.44504450445044%" headers="mcps1.2.5.1.4 "><p id="p230120311413"><a name="p230120311413"></a><a name="p230120311413"></a>每页返回的资源个数。</p>
<p id="p147131447514"><a name="p147131447514"></a><a name="p147131447514"></a>取值范围：0~500</p>
<p id="p1385813431412"><a name="p1385813431412"></a><a name="p1385813431412"></a>取值一般为10，20，50。默认值为500。</p>
</td>
</tr>
<tr id="row58150604195642"><td class="cellrowborder" valign="top" width="16.62166216621662%" headers="mcps1.2.5.1.1 "><p id="p11536930195644"><a name="p11536930195644"></a><a name="p11536930195644"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="15.921592159215923%" headers="mcps1.2.5.1.2 "><p id="p62076162195644"><a name="p62076162195644"></a><a name="p62076162195644"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.01170117011701%" headers="mcps1.2.5.1.3 "><p id="p62113243195644"><a name="p62113243195644"></a><a name="p62113243195644"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50.44504450445044%" headers="mcps1.2.5.1.4 "><p id="p35951433204916"><a name="p35951433204916"></a><a name="p35951433204916"></a>分页查询起始偏移量，表示从偏移量的下一个资源开始查询。</p>
<p id="p18898143914915"><a name="p18898143914915"></a><a name="p18898143914915"></a>取值范围：0~2147483647</p>
<p id="p13209172234718"><a name="p13209172234718"></a><a name="p13209172234718"></a>默认值为0。</p>
<p id="p167712216335"><a name="p167712216335"></a><a name="p167712216335"></a>当前设置marker不为空时，以marker为分页起始标识。</p>
</td>
</tr>
<tr id="row6180858115857"><td class="cellrowborder" valign="top" width="16.62166216621662%" headers="mcps1.2.5.1.1 "><p id="p6537624212219"><a name="p6537624212219"></a><a name="p6537624212219"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="15.921592159215923%" headers="mcps1.2.5.1.2 "><p id="p6098421112219"><a name="p6098421112219"></a><a name="p6098421112219"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.01170117011701%" headers="mcps1.2.5.1.3 "><p id="p4077405312219"><a name="p4077405312219"></a><a name="p4077405312219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.44504450445044%" headers="mcps1.2.5.1.4 "><p id="p1436398312219"><a name="p1436398312219"></a><a name="p1436398312219"></a>资源标签。</p>
<p id="p6216698912219"><a name="p6216698912219"></a><a name="p6216698912219"></a>取值格式：key1,value1|key2,value2</p>
<p id="p64141841114123"><a name="p64141841114123"></a><a name="p64141841114123"></a>多个标签之间用"|"分开，每个标签的键值用英文逗号","相隔。</p>
<p id="p2263199412219"><a name="p2263199412219"></a><a name="p2263199412219"></a>多个标签之间为“与”的关系。</p>
<p id="p65263192115146"><a name="p65263192115146"></a><a name="p65263192115146"></a>关于资源标签，请参见<a href="添加资源标签.md">添加资源标签</a>。</p>
<p id="p1770514714203"><a name="p1770514714203"></a><a name="p1770514714203"></a>搜索模式为精确搜索。如果资源标签值value是以*开头时，则按照*后面的值全模糊匹配。</p>
<p id="p71284149127"><a name="p71284149127"></a><a name="p71284149127"></a>默认值为空。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section8713795"></a>

-   请求参数

    无

-   请求样例

    查询PTR列表。

    ```
    GET https://{DNS_Endpoint}/v2/reverse/floatingips
    ```


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
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="p58299955181232"><a name="p58299955181232"></a><a name="p58299955181232"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p5040034717923"><a name="p5040034717923"></a><a name="p5040034717923"></a>指向当前资源或者其他相关资源的链接。</p>
    <p id="p5094994217923"><a name="p5094994217923"></a><a name="p5094994217923"></a>当响应需要分页时，需要包含一个next链接来进行分页。详细信息请参见<a href="#table354521744216">表5</a>。</p>
    </td>
    </tr>
    <tr id="row17649295181232"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p20306794181232"><a name="p20306794181232"></a><a name="p20306794181232"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="p34237593181232"><a name="p34237593181232"></a><a name="p34237593181232"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p21781637181232"><a name="p21781637181232"></a><a name="p21781637181232"></a>返回满足过滤条件的资源总数。详细信息请参见<a href="#table16355953155210">表4</a>。</p>
    </td>
    </tr>
    <tr id="row61817005181232"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p41121470181232"><a name="p41121470181232"></a><a name="p41121470181232"></a>floatingips</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="p1974516569913"><a name="p1974516569913"></a><a name="p1974516569913"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="p20334170181232"><a name="p20334170181232"></a><a name="p20334170181232"></a>PTR Record对象列表。详细信息请参见<a href="#table43740677113542">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  floatingips字段说明

    <a name="table43740677113542"></a>
    <table><thead align="left"><tr id="rc433fa5ceea44999bda6baae10282bed"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0042318613_p690539418456"><a name="zh-cn_topic_0042318613_p690539418456"></a><a name="zh-cn_topic_0042318613_p690539418456"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.259999999999998%" id="mcps1.2.4.1.2"><p id="aec3926ab378e4c9fafd96942ae9c2f24"><a name="aec3926ab378e4c9fafd96942ae9c2f24"></a><a name="aec3926ab378e4c9fafd96942ae9c2f24"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.56%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0042318613_p781187018456"><a name="zh-cn_topic_0042318613_p781187018456"></a><a name="zh-cn_topic_0042318613_p781187018456"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="rf59c1308b662423d9e5c5eb972f057a1"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="af1202b164f13422d896f91d34faf7c44"><a name="af1202b164f13422d896f91d34faf7c44"></a><a name="af1202b164f13422d896f91d34faf7c44"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="p27591010151011"><a name="p27591010151011"></a><a name="p27591010151011"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.56%" headers="mcps1.2.4.1.3 "><p id="a48e534dd79ef418ab79ff1303a8ff149"><a name="a48e534dd79ef418ab79ff1303a8ff149"></a><a name="a48e534dd79ef418ab79ff1303a8ff149"></a>PTR记录的ID，格式形如{region}:{floatingip_id}。</p>
    </td>
    </tr>
    <tr id="r8de792b7f9bb42a5bbd359fd67c55802"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="affabc5d973dd43ef8f81431cfbba2e4d"><a name="affabc5d973dd43ef8f81431cfbba2e4d"></a><a name="affabc5d973dd43ef8f81431cfbba2e4d"></a>ptrdname</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="p598126105"><a name="p598126105"></a><a name="p598126105"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.56%" headers="mcps1.2.4.1.3 "><p id="a695a30773b7b4545a348899428360b0c"><a name="a695a30773b7b4545a348899428360b0c"></a><a name="a695a30773b7b4545a348899428360b0c"></a>PTR记录对应的域名。</p>
    </td>
    </tr>
    <tr id="r07959df68aa640f7b2550a4ec13bd321"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="a58edc66abfd94b8d88234ccc87f993ef"><a name="a58edc66abfd94b8d88234ccc87f993ef"></a><a name="a58edc66abfd94b8d88234ccc87f993ef"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="p183479136108"><a name="p183479136108"></a><a name="p183479136108"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.56%" headers="mcps1.2.4.1.3 "><p id="a26cda8d7c28c484a8555271f1b7c9c18"><a name="a26cda8d7c28c484a8555271f1b7c9c18"></a><a name="a26cda8d7c28c484a8555271f1b7c9c18"></a>对PTR记录的描述。</p>
    </td>
    </tr>
    <tr id="rc07302b7ba7748e2bd3ba03f66d4d046"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="ac280dc3e9e514cb4bb61dc356b75c265"><a name="ac280dc3e9e514cb4bb61dc356b75c265"></a><a name="ac280dc3e9e514cb4bb61dc356b75c265"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="a2faf54e82d504a619ab8183ab083c6f4"><a name="a2faf54e82d504a619ab8183ab083c6f4"></a><a name="a2faf54e82d504a619ab8183ab083c6f4"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.56%" headers="mcps1.2.4.1.3 "><p id="p73714549431"><a name="p73714549431"></a><a name="p73714549431"></a>PTR记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="p1837175484310"><a name="p1837175484310"></a><a name="p1837175484310"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    <p id="a3c9384952a064d6da121077d6f1faf0a"><a name="a3c9384952a064d6da121077d6f1faf0a"></a><a name="a3c9384952a064d6da121077d6f1faf0a"></a>取值范围：</p>
    <p id="abb10491c52064bc0a5fb65a66c645c01"><a name="abb10491c52064bc0a5fb65a66c645c01"></a><a name="abb10491c52064bc0a5fb65a66c645c01"></a>1～2147483647。</p>
    <p id="p0873451124411"><a name="p0873451124411"></a><a name="p0873451124411"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="rb0577738b87a4dafb23d0a1ef4cac7ed"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="a6c80427db35e48689eb4ae318fc8fa30"><a name="a6c80427db35e48689eb4ae318fc8fa30"></a><a name="a6c80427db35e48689eb4ae318fc8fa30"></a>address</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="p1922131461018"><a name="p1922131461018"></a><a name="p1922131461018"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.56%" headers="mcps1.2.4.1.3 "><p id="a01a51f050f414b669b4a08478ede886e"><a name="a01a51f050f414b669b4a08478ede886e"></a><a name="a01a51f050f414b669b4a08478ede886e"></a>弹性IP的IP地址。</p>
    </td>
    </tr>
    <tr id="r9d3448295e68459db0bade4562e211a5"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="a29ee325b52134a3f847bbee5c91b1da3"><a name="a29ee325b52134a3f847bbee5c91b1da3"></a><a name="a29ee325b52134a3f847bbee5c91b1da3"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="p86891651016"><a name="p86891651016"></a><a name="p86891651016"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.56%" headers="mcps1.2.4.1.3 "><p id="a133beb6a97ed42bdac622271072840e6"><a name="a133beb6a97ed42bdac622271072840e6"></a><a name="a133beb6a97ed42bdac622271072840e6"></a>资源状态。</p>
    <p id="p4158416129"><a name="p4158416129"></a><a name="p4158416129"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="rb4683cb844214f51ae468943568b4cde"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="a1d911558e18444b3896ace2ed6ccbaec"><a name="a1d911558e18444b3896ace2ed6ccbaec"></a><a name="a1d911558e18444b3896ace2ed6ccbaec"></a>action</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="ae39f64d2c5af4dae91b509416f77d31d"><a name="ae39f64d2c5af4dae91b509416f77d31d"></a><a name="ae39f64d2c5af4dae91b509416f77d31d"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.56%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0042318613_p507362318456"><a name="zh-cn_topic_0042318613_p507362318456"></a><a name="zh-cn_topic_0042318613_p507362318456"></a>对该资源的当前操作。</p>
    <p id="p3570202615112"><a name="p3570202615112"></a><a name="p3570202615112"></a>取值范围：CREATE，UPDATE，DELETE，NONE。</p>
    <p id="p1959511502122"><a name="p1959511502122"></a><a name="p1959511502122"></a>CREATE：表示创建，UPDATE：表示更新，DELETE：表示删除，NONE：表示无操作</p>
    </td>
    </tr>
    <tr id="re6d739b3d80f4bcda0e2ad834dc1d66f"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0042318613_p204899518456"><a name="zh-cn_topic_0042318613_p204899518456"></a><a name="zh-cn_topic_0042318613_p204899518456"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.259999999999998%" headers="mcps1.2.4.1.2 "><p id="ad894d21cefa74634a62f6964f84019f6"><a name="ad894d21cefa74634a62f6964f84019f6"></a><a name="ad894d21cefa74634a62f6964f84019f6"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.56%" headers="mcps1.2.4.1.3 "><p id="ab163171b57cd4600a059890e5f4373ce"><a name="ab163171b57cd4600a059890e5f4373ce"></a><a name="ab163171b57cd4600a059890e5f4373ce"></a>指向当前资源或者其他相关资源的链接。</p>
    <p id="a4dc7ac60268d4291a27544e93c236e22"><a name="a4dc7ac60268d4291a27544e93c236e22"></a><a name="a4dc7ac60268d4291a27544e93c236e22"></a>当响应需要分页时，需要包含一个next链接来进行分页。详细信息请参见<a href="#table354521744216">表5</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  metadata参数说明

    <a name="table16355953155210"></a>
    <table><thead align="left"><tr id="r1ee98e923a7c4bfcaa89e708d3fca79e"><th class="cellrowborder" valign="top" width="18.02180218021802%" id="mcps1.2.4.1.1"><p id="af493c2fde22f44069c2b5ea0467dfe89"><a name="af493c2fde22f44069c2b5ea0467dfe89"></a><a name="af493c2fde22f44069c2b5ea0467dfe89"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.881988198819883%" id="mcps1.2.4.1.2"><p id="a581940a484df4c8294e51f11391a23c8"><a name="a581940a484df4c8294e51f11391a23c8"></a><a name="a581940a484df4c8294e51f11391a23c8"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.09620962096209%" id="mcps1.2.4.1.3"><p id="a0301bbf5a1234ea3a88a104e1b4cff92"><a name="a0301bbf5a1234ea3a88a104e1b4cff92"></a><a name="a0301bbf5a1234ea3a88a104e1b4cff92"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r7cc02a0ecbd24482bca90faa98114b18"><td class="cellrowborder" valign="top" width="18.02180218021802%" headers="mcps1.2.4.1.1 "><p id="a9234858cb2f447539b4b85a307884322"><a name="a9234858cb2f447539b4b85a307884322"></a><a name="a9234858cb2f447539b4b85a307884322"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.881988198819883%" headers="mcps1.2.4.1.2 "><p id="af14a2a2c8f0345f4811bb21dd2a9b667"><a name="af14a2a2c8f0345f4811bb21dd2a9b667"></a><a name="af14a2a2c8f0345f4811bb21dd2a9b667"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.09620962096209%" headers="mcps1.2.4.1.3 "><p id="a39058f9901c84eb9a776ca5cd44ede29"><a name="a39058f9901c84eb9a776ca5cd44ede29"></a><a name="a39058f9901c84eb9a776ca5cd44ede29"></a>满足查询条件的资源总数，不受分页（即limit、offset参数）影响。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  links参数说明

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
    <tr id="row20182104310515"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
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
        "links": {
            "self": "https://Endpoint/v2/reverse/floatingips",
            "next": "https://Endpoint/v2/zones?id=&limit=1&marker=region_id:c5504932-bf23-4171-b655-b87a6bc59334"
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


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

