# 怎样设置弹性云服务器的私网IP的反向解析？<a name="dns_faq_031"></a>

反向域名解析提供通过IP地址查找域名的功能。

通过管理控制台的“域名解析 \> 反向解析”“反向解析”页面可以设置EIP的反向解析。如果要设置ECS服务器私网IP的反向解析，可以通过在创建内网域名之后添加PTR记录集实现。

设置私网IP的反向解析，其域名格式是x.x.x.x.in-addr.arpa。

>![](public_sys-resources/icon-note.gif) **说明：**   
>in-addr.arpa是反向解析的顶级域。  
>例如，私网IP是192.168.1.10，其反向域名格式是10.1.168.192.in-addr.arpa。  
>可以创建内网域名192.in-addr.arpa，然后添加10.1.168.192.in-addr.arpa的PTR记录集来实现设置该私网IP的反向解析记录。  

## 创建内网域名<a name="section75811117181517"></a>

1.  登录管理控制台。
2.  选择“网络 \> 云解析服务”。

    进入云解析服务页面。

3.  在左侧树状导航栏，选择“域名解析 \> 内网域名”。

    进入“内网域名”页面。

4.  单击管理控制台左上角的![](figures/zh-cn_image_0073591874.png)，选择区域和项目。
5.  单击“创建内网域名”，开始创建内网域名。

    **图 1**  创建内网域名<a name="fig13961150155910"></a>  
    ![](figures/创建内网域名-1.png "创建内网域名-1")

6.  根据界面提示配置参数，参数说明如[表1](#table12455154165118)所示。

    **表 1**  创建内网域名参数说明

    <a name="table12455154165118"></a>
    <table><thead align="left"><tr id="row54556485113"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p44551945516"><a name="p44551945516"></a><a name="p44551945516"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p44553411510"><a name="p44553411510"></a><a name="p44553411510"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p10455154125113"><a name="p10455154125113"></a><a name="p10455154125113"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row144553495114"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p645619414517"><a name="p645619414517"></a><a name="p645619414517"></a>域名</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p51968545220"><a name="p51968545220"></a><a name="p51968545220"></a>域名。</p>
    <p id="p151961957522"><a name="p151961957522"></a><a name="p151961957522"></a>反向顶级域in-addr.arpa。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p174562418510"><a name="p174562418510"></a><a name="p174562418510"></a>192.in-addr.arpa</p>
    </td>
    </tr>
    <tr id="row5456845517"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p84561645514"><a name="p84561645514"></a><a name="p84561645514"></a>VPC</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p1645674145115"><a name="p1645674145115"></a><a name="p1645674145115"></a>内网域名要关联的VPC。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p104567425119"><a name="p104567425119"></a><a name="p104567425119"></a>-</p>
    </td>
    </tr>
    <tr id="row145614175118"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p174561745510"><a name="p174561745510"></a><a name="p174561745510"></a>邮箱</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p126950408523"><a name="p126950408523"></a><a name="p126950408523"></a>可选参数。</p>
    <p id="p46952405522"><a name="p46952405522"></a><a name="p46952405522"></a>管理该内网域名的管理员邮箱。建议用户使用保留邮箱“HOSTMASTER@<em id="i2069584005210"><a name="i2069584005210"></a><a name="i2069584005210"></a>域名</em>”作为此管理员邮箱。</p>
    <p id="p1069694012522"><a name="p1069694012522"></a><a name="p1069694012522"></a>更多关于Email的信息，请参见<a href="SOA记录中的Email格式为什么变化了.md">SOA记录中的Email格式为什么变化了？</a></p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p345613435118"><a name="p345613435118"></a><a name="p345613435118"></a>HOSTMASTER@example.com</p>
    </td>
    </tr>
    <tr id="row18748159183818"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p18481122652416"><a name="p18481122652416"></a><a name="p18481122652416"></a>标签</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p18551159141412"><a name="p18551159141412"></a><a name="p18551159141412"></a>可选参数。</p>
    <p id="p523611212291"><a name="p523611212291"></a><a name="p523611212291"></a>域名的标示，包括键和值，每个域名可以创建10个标签。</p>
    <p id="p1690771316155"><a name="p1690771316155"></a><a name="p1690771316155"></a>键和值的命名规则请参见<a href="#dns_faq_031__table114584301390">表2</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p15551259121412"><a name="p15551259121412"></a><a name="p15551259121412"></a>example_key1</p>
    <p id="p15031954131915"><a name="p15031954131915"></a><a name="p15031954131915"></a>example_value1</p>
    </td>
    </tr>
    <tr id="row64563417519"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p545619418517"><a name="p545619418517"></a><a name="p545619418517"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p6836195285214"><a name="p6836195285214"></a><a name="p6836195285214"></a>可选参数。</p>
    <p id="p28378521522"><a name="p28378521522"></a><a name="p28378521522"></a>域名的描述信息。</p>
    <p id="p15838125275220"><a name="p15838125275220"></a><a name="p15838125275220"></a>长度不超过255个字符。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p84561846519"><a name="p84561846519"></a><a name="p84561846519"></a>This is a zone example.</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  标签命名规则

    <a name="table114584301390"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0057777026_zh-cn_topic_0035467699_row72901535141713"><th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p132908358173"><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p132908358173"></a><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p132908358173"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="50.505050505050505%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p1629093517175"><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p1629093517175"></a><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p1629093517175"></a>规则</p>
    </th>
    <th class="cellrowborder" valign="top" width="31.313131313131315%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p32901635141714"><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p32901635141714"></a><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p32901635141714"></a>举例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0057777026_zh-cn_topic_0035467699_row52906354176"><td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p122901235111715"><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p122901235111715"></a><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p122901235111715"></a>键</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.505050505050505%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_ul46253231183"></a><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_ul46253231183"></a><ul id="zh-cn_topic_0057777026_zh-cn_topic_0035467699_ul46253231183"><li>不能为空。</li><li>对于同一资源键值唯一。</li><li>长度不超过36个字符。</li><li>取值为不包含“=”,“*”,“&lt;”,“&gt;”,“\”,“,”,“|”,“/”的所有Unicode字符，且首尾字符不能为空格。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="31.313131313131315%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p12290163511720"><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p12290163511720"></a><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p12290163511720"></a>example_key1</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0057777026_zh-cn_topic_0035467699_row132900355172"><td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p152901635181712"><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p152901635181712"></a><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p152901635181712"></a>值</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.505050505050505%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_ul19648123161815"></a><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_ul19648123161815"></a><ul id="zh-cn_topic_0057777026_zh-cn_topic_0035467699_ul19648123161815"><li>不能为空。</li><li>长度不超过43个字符。</li><li>取值为不包含“=”,“*”,“&lt;”,“&gt;”,“\”,“,”,“|”,“/”的所有Unicode字符，且首尾字符不能为空格。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="31.313131313131315%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p62904352179"><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p62904352179"></a><a name="zh-cn_topic_0057777026_zh-cn_topic_0035467699_p62904352179"></a>example_value1</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  单击“确定”。

    创建完成后，您可以在“内网域名”页面查看新创建的域名信息。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >单击“名称”列的域名名称，可以看到系统已经为您创建了SOA类型和NS类型的记录集。其中，  
    >-   SOA类型的记录集标识了对此域名具有最终解释权的主权威服务器。  
    >-   NS类型的记录集标识了此域名的权威服务器。  


## 添加PTR记录集<a name="section59204303151"></a>

1.  在“内网域名”页面的域名列表中，单击新创建域名的名称。

    系统进入域名解析记录页面。

2.  单击“添加记录集”。

    系统进入“添加记录集”页面。

    **图 2**  添加记录集<a name="fig6986018374"></a>  
    ![](figures/添加记录集-2.png "添加记录集-2")

3.  根据界面提示填写参数配置，参数说明如[表3](#table2068616914271)所示。

    **表 3**  添加PTR类型记录集参数说明

    <a name="table2068616914271"></a>
    <table><thead align="left"><tr id="row14687398277"><th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.4.1.1"><p id="p56871894279"><a name="p56871894279"></a><a name="p56871894279"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.2.4.1.2"><p id="p46871191279"><a name="p46871191279"></a><a name="p46871191279"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p1568749132716"><a name="p1568749132716"></a><a name="p1568749132716"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row46871799274"><td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.4.1.1 "><p id="p368713912271"><a name="p368713912271"></a><a name="p368713912271"></a>主机记录</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.4.1.2 "><p id="p172536599323"><a name="p172536599323"></a><a name="p172536599323"></a>填写反向解析具体的IP地址。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p166871919278"><a name="p166871919278"></a><a name="p166871919278"></a>10.1.168</p>
    <p id="p3645662495544"><a name="p3645662495544"></a><a name="p3645662495544"></a>例如，用户IP地址为192.168.1.10，则反向解析域名的完整格式为10.1.168.192.in-addr.arpa。</p>
    <a name="ul772510438411"></a><a name="ul772510438411"></a><ul id="ul772510438411"><li>若创建的域名为192.in-addr.arpa，则主机记录为10.1.168</li><li>若创建的域名为1.168.192.in-addr.arpa，则主机记录为10</li></ul>
    </td>
    </tr>
    <tr id="row186872093277"><td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.4.1.1 "><p id="p176871792270"><a name="p176871792270"></a><a name="p176871792270"></a>类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.4.1.2 "><p id="p068716910279"><a name="p068716910279"></a><a name="p068716910279"></a>记录集的类型，此处为PTR类型。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p1968821875317"><a name="p1968821875317"></a><a name="p1968821875317"></a>PTR – 将IP地址指向域名</p>
    </td>
    </tr>
    <tr id="row17687395279"><td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.4.1.1 "><p id="p1268849122712"><a name="p1268849122712"></a><a name="p1268849122712"></a>TTL(秒)</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.4.1.2 "><p id="p206881395275"><a name="p206881395275"></a><a name="p206881395275"></a>记录集的有效缓存时间，以秒为单位。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p1068811962718"><a name="p1068811962718"></a><a name="p1068811962718"></a>默认为“5min”，即300s。</p>
    </td>
    </tr>
    <tr id="row176881399271"><td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.4.1.1 "><p id="p166882914277"><a name="p166882914277"></a><a name="p166882914277"></a>值</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.4.1.2 "><p id="p51576321316"><a name="p51576321316"></a><a name="p51576321316"></a>反向解析指向的域名。</p>
    <p id="p715713223114"><a name="p715713223114"></a><a name="p715713223114"></a>仅可输入1个域名。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p36883972711"><a name="p36883972711"></a><a name="p36883972711"></a>mail.example.com</p>
    </td>
    </tr>
    <tr id="row10389125919409"><td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.4.1.1 "><p id="p183901516412"><a name="p183901516412"></a><a name="p183901516412"></a>标签</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.4.1.2 "><p id="p6550184818333"><a name="p6550184818333"></a><a name="p6550184818333"></a>可选参数，当“其他配置”开关打开时显示。记录集的标示，包括键和值，每个记录集可以创建10个标签。</p>
    <p id="p339421184117"><a name="p339421184117"></a><a name="p339421184117"></a>键和值的命名规则请参见<a href="#dns_faq_031__table114584301390">表2</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p9399117417"><a name="p9399117417"></a><a name="p9399117417"></a>example_key1</p>
    <p id="p1140011110414"><a name="p1140011110414"></a><a name="p1140011110414"></a>example_value1</p>
    </td>
    </tr>
    <tr id="row17688109192713"><td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.4.1.1 "><p id="p968899202716"><a name="p968899202716"></a><a name="p968899202716"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.4.1.2 "><p id="p66251337192810"><a name="p66251337192810"></a><a name="p66251337192810"></a>可选配置，对PTR记录集的描述，当“其他配置”开关打开时显示。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p11688159152710"><a name="p11688159152710"></a><a name="p11688159152710"></a>The description of the PTR Record.</p>
    </td>
    </tr>
    </tbody>
    </table>

4.  单击“确定”，完成PTR类型记录集的添加。

