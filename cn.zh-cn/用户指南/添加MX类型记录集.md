# 添加MX类型记录集<a name="dns_usermanual_0011"></a>

## 操作场景<a name="section187281084528"></a>

当您想要指定域名对应的邮件服务器时，可以通过为域名增加MX类型记录集实现。

可以用于配置邮箱解析。

更多关于记录集类型的介绍，请参见[记录集类型及配置规则](记录集类型及配置规则.md)。

## 约束与限制<a name="section10284161715528"></a>

已经部署邮箱服务器，并通过邮箱服务商获取邮箱的域名地址。

## 操作步骤<a name="section6412174644120"></a>

1.  登录管理控制台。
2.  将鼠标悬浮于页面左侧的“![](figures/service-list.jpg)”，在服务列表中，选择“网络  \> 云解析服务”。

    进入“云解析”页面。


1.  在左侧树状导航栏，选择“公网域名”或者“内网域名”。

    进入域名列表页面。

2.  （可选）如果选择“内网解析”，请单击管理控制台左上角的![](figures/icon-region.png)，选择区域和项目。
3.  在待添加记录集的域名所在行，单击“名称”列的域名名称。
4.  单击“添加记录集”。

    进入“添加记录集”页面。


1.  设置记录集参数，如[表1](#td3830bff2b1749ca977ebf2237a18cd8)所示。

    **表 1**  添加MX类型记录集参数说明

    <a name="td3830bff2b1749ca977ebf2237a18cd8"></a>
    <table><thead align="left"><tr id="row40985647123146"><th class="cellrowborder" valign="top" width="19.05%" id="mcps1.2.4.1.1"><p id="p31503124123146"><a name="p31503124123146"></a><a name="p31503124123146"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.620000000000005%" id="mcps1.2.4.1.2"><p id="p1616237123146"><a name="p1616237123146"></a><a name="p1616237123146"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33%" id="mcps1.2.4.1.3"><p id="p63806371123146"><a name="p63806371123146"></a><a name="p63806371123146"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row933533123146"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.1 "><p id="p8507331123146"><a name="p8507331123146"></a><a name="p8507331123146"></a>主机记录</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.620000000000005%" headers="mcps1.2.4.1.2 "><p id="p498991411924"><a name="p498991411924"></a><a name="p498991411924"></a>解析域名的前缀。</p>
    <p id="p4490923311924"><a name="p4490923311924"></a><a name="p4490923311924"></a>例如创建的域名为“example.com”，其“主机记录”设置包括：</p>
    <a name="ul62101617105015"></a><a name="ul62101617105015"></a><ul id="ul62101617105015"><li>www：用于网站解析，表示解析的域名为“www.example.com”。</li><li>空：用于网站解析，表示解析的域名为“example.com”。<p id="dns_usermanual_0007_p210152475518"><a name="dns_usermanual_0007_p210152475518"></a><a name="dns_usermanual_0007_p210152475518"></a>主机记录置为空，还可用于为空头域名“@”添加解析。</p>
    </li><li>abc：用于子域名解析，表示解析的域名为“example.com”的子域名“abc.example.com”。</li><li>mail：用于邮箱解析，表示解析的域名为“mail.example.com”。</li><li>*：用于泛解析，表示解析的域名为“*.example.com”，匹配“example.com”的所有子域名。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p1195486695028"><a name="p1195486695028"></a><a name="p1195486695028"></a>置空</p>
    </td>
    </tr>
    <tr id="row26983954123146"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.1 "><p id="p38216656123146"><a name="p38216656123146"></a><a name="p38216656123146"></a>类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.620000000000005%" headers="mcps1.2.4.1.2 "><p id="p8541435123146"><a name="p8541435123146"></a><a name="p8541435123146"></a>记录集的类型，此处为MX类型。</p>
    <p id="p8911154710176"><a name="p8911154710176"></a><a name="p8911154710176"></a>添加记录集时，如果提示解析记录集已经存在，说明待添加的记录集与已有的记录集存在限制关系或者冲突。</p>
    <p id="p091321341812"><a name="p091321341812"></a><a name="p091321341812"></a>详细内容请参见<a href="https://support.huaweicloud.com/dns_faq/dns_faq_016.html" target="_blank" rel="noopener noreferrer">为什么会提示解析记录集已经存在？</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p204561425134318"><a name="p204561425134318"></a><a name="p204561425134318"></a>MX – 将域名指向邮件服务器地址</p>
    </td>
    </tr>
    <tr id="row94915310153"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.1 "><p id="p1880719311392"><a name="p1880719311392"></a><a name="p1880719311392"></a>别名</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.620000000000005%" headers="mcps1.2.4.1.2 "><p id="p1480715314392"><a name="p1480715314392"></a><a name="p1480715314392"></a>用于是否将此记录集关联至云服务资源实例。</p>
    <a name="ul780813115548"></a><a name="ul780813115548"></a><ul id="ul780813115548"><li>是：为此记录集关联云服务资源实例，详细说明请参见<a href="设置别名解析.md">设置别名解析</a>。</li><li>否：不为此记录集关联云服务资源实例。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p58071353915"><a name="p58071353915"></a><a name="p58071353915"></a>否</p>
    </td>
    </tr>
    <tr id="row12886103714516"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.1 "><p id="p48862371953"><a name="p48862371953"></a><a name="p48862371953"></a>别名记录</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.620000000000005%" headers="mcps1.2.4.1.2 "><p id="p203236165311"><a name="p203236165311"></a><a name="p203236165311"></a>仅当“别名”设置为“是”时出现。</p>
    <p id="p19832241155311"><a name="p19832241155311"></a><a name="p19832241155311"></a>用于设置记录集关联的华为云服务资源实例。</p>
    <p id="p2756195865318"><a name="p2756195865318"></a><a name="p2756195865318"></a>记录集支持关联的华为云服务资源实例包括：云速建站、Web应用防火墙。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p68865371253"><a name="p68865371253"></a><a name="p68865371253"></a>-</p>
    </td>
    </tr>
    <tr id="row3823189820853"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.1 "><p id="p4690566311450"><a name="p4690566311450"></a><a name="p4690566311450"></a>线路类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.620000000000005%" headers="mcps1.2.4.1.2 "><p id="p578885213504"><a name="p578885213504"></a><a name="p578885213504"></a>解析的线路类型用于DNS服务器在解析域名时，根据访问者的来源，返回对应的服务器IP地址。</p>
    <p id="p1632317531489"><a name="p1632317531489"></a><a name="p1632317531489"></a>默认值为“全网默认”。</p>
    <p id="p432365316811"><a name="p432365316811"></a><a name="p432365316811"></a>仅支持为公网域名的记录集配置此参数。</p>
    <a name="ul867142417117"></a><a name="ul867142417117"></a><ul id="ul867142417117"><li>全网默认：默认线路类型，当未根据访问者来源设置解析线路时，系统会返回默认解析结果。</li><li>运营商线路解析：根据访问者所在运营商，设置解析线路，详细内容请参见<a href="配置运营商线路解析.md">配置运营商线路解析</a>。</li><li>地域解析：根据访问者所在地域，设置解析线路，详细内容请参见<a href="配置地域解析.md">配置地域线路解析</a>。</li><li>自定义线路：根据访问者所属IP网段，设置解析线路，详细内容请参见<a href="配置自定义线路解析.md">配置自定义线路解析</a>。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p5391976911450"><a name="p5391976911450"></a><a name="p5391976911450"></a>全网默认</p>
    </td>
    </tr>
    <tr id="row52690765123146"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.1 "><p id="p40093542123146"><a name="p40093542123146"></a><a name="p40093542123146"></a>TTL(秒)</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.620000000000005%" headers="mcps1.2.4.1.2 "><p id="p5888275712739"><a name="p5888275712739"></a><a name="p5888275712739"></a>解析记录在本地DNS服务器的缓存时间，以秒为单位。</p>
    <p id="p103873299529"><a name="p103873299529"></a><a name="p103873299529"></a>默认值为“300秒”。取值范围为：300~2147483647</p>
    <p id="p7737113020523"><a name="p7737113020523"></a><a name="p7737113020523"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    <p id="p12104133155216"><a name="p12104133155216"></a><a name="p12104133155216"></a>更多TTL相关内容请参见<a href="https://support.huaweicloud.com/dns_faq/dns_faq_013.html" target="_blank" rel="noopener noreferrer">什么是TTL值？</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p477403312739"><a name="p477403312739"></a><a name="p477403312739"></a>5分钟，即300s。</p>
    </td>
    </tr>
    <tr id="row17058403123146"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.1 "><p id="p39553441123146"><a name="p39553441123146"></a><a name="p39553441123146"></a>值</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.620000000000005%" headers="mcps1.2.4.1.2 "><p id="p395310183518"><a name="p395310183518"></a><a name="p395310183518"></a>填写邮箱服务器地址。</p>
    <p id="p19845113674112"><a name="p19845113674112"></a><a name="p19845113674112"></a>最多可以输入50个不重复地址，多个地址之间以换行符分隔。</p>
    <p id="p7599103820417"><a name="p7599103820417"></a><a name="p7599103820417"></a>填写格式：[优先级] [邮箱服务器域名地址]</p>
    <div class="p" id="p937434154111"><a name="p937434154111"></a><a name="p937434154111"></a>配置规则：<a name="ul78353231045"></a><a name="ul78353231045"></a><ul id="ul78353231045"><li>优先级：用来指定邮箱服务器接收邮件优先顺序，数值越小优先级越高。</li><li>邮箱服务器域名地址：邮箱服务商提供的域名地址。</li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="a298c2074edd64bd694c2796cc0f4d207"><a name="a298c2074edd64bd694c2796cc0f4d207"></a><a name="a298c2074edd64bd694c2796cc0f4d207"></a>10 mailserver.example.com.</p>
    </td>
    </tr>
    <tr id="row1032385319303"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.1 "><p id="p3643254173012"><a name="p3643254173012"></a><a name="p3643254173012"></a>权重</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.620000000000005%" headers="mcps1.2.4.1.2 "><p id="p13661098305"><a name="p13661098305"></a><a name="p13661098305"></a>可选参数，返回解析记录的权重比例。默认值为1，取值范围：0~1000。</p>
    <p id="p87229173020"><a name="p87229173020"></a><a name="p87229173020"></a>仅支持为公网域名的记录集配置此参数。</p>
    <p id="p147789173018"><a name="p147789173018"></a><a name="p147789173018"></a>当域名在同一解析线路中有多条相同类型的解析记录时，可以通过“权重”设置解析记录的响应比例。详细内容请参见<a href="配置权重解析.md">配置权重解析</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p7666115417309"><a name="p7666115417309"></a><a name="p7666115417309"></a>1</p>
    </td>
    </tr>
    <tr id="row17185193111276"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.1 "><p id="p10406539102715"><a name="p10406539102715"></a><a name="p10406539102715"></a>标签</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.620000000000005%" headers="mcps1.2.4.1.2 "><p id="p1414134716167"><a name="p1414134716167"></a><a name="p1414134716167"></a>可选参数，当“其他配置”开关打开时显示。</p>
    <p id="p531243991715"><a name="p531243991715"></a><a name="p531243991715"></a>记录集的标识，包括键和值，每个记录集可以创建10个标签。</p>
    <p id="p74162039142714"><a name="p74162039142714"></a><a name="p74162039142714"></a>键和值的命名规则请参见<a href="#table191971158112315">表2</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p7423139192714"><a name="p7423139192714"></a><a name="p7423139192714"></a>example_key1</p>
    <p id="p1428103913279"><a name="p1428103913279"></a><a name="p1428103913279"></a>example_value1</p>
    </td>
    </tr>
    <tr id="row31966209133453"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.2.4.1.1 "><p id="p3764367133458"><a name="p3764367133458"></a><a name="p3764367133458"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.620000000000005%" headers="mcps1.2.4.1.2 "><p id="p2441229193412"><a name="p2441229193412"></a><a name="p2441229193412"></a>可选参数，对域名的描述，当“其他配置”开关打开时显示。</p>
    <p id="p17140145133253"><a name="p17140145133253"></a><a name="p17140145133253"></a>长度不超过255个字符。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p17597507133458"><a name="p17597507133458"></a><a name="p17597507133458"></a>The description of the hostname.</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  标签命名规则

    <a name="table191971158112315"></a>
    <table><thead align="left"><tr id="dns_usermanual_0007_r4f5fd2fecc60424eb20075f35572eeb0"><th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.2.4.1.1"><p id="dns_usermanual_0007_zh-cn_topic_0035467699_p132908358173"><a name="dns_usermanual_0007_zh-cn_topic_0035467699_p132908358173"></a><a name="dns_usermanual_0007_zh-cn_topic_0035467699_p132908358173"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="50.505050505050505%" id="mcps1.2.4.1.2"><p id="dns_usermanual_0007_aa34a0c0cbae34a23b63e1882cf4a2c91"><a name="dns_usermanual_0007_aa34a0c0cbae34a23b63e1882cf4a2c91"></a><a name="dns_usermanual_0007_aa34a0c0cbae34a23b63e1882cf4a2c91"></a>规则</p>
    </th>
    <th class="cellrowborder" valign="top" width="31.313131313131315%" id="mcps1.2.4.1.3"><p id="dns_usermanual_0007_aece629313e384a698796b7aff7821561"><a name="dns_usermanual_0007_aece629313e384a698796b7aff7821561"></a><a name="dns_usermanual_0007_aece629313e384a698796b7aff7821561"></a>举例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="dns_usermanual_0007_rbb2718429c5141319dde3ac939f97ba9"><td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.2.4.1.1 "><p id="dns_usermanual_0007_ae8044150f5804b42bd8632ccced6b72a"><a name="dns_usermanual_0007_ae8044150f5804b42bd8632ccced6b72a"></a><a name="dns_usermanual_0007_ae8044150f5804b42bd8632ccced6b72a"></a>键</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.505050505050505%" headers="mcps1.2.4.1.2 "><a name="dns_usermanual_0007_zh-cn_topic_0035467699_ul46253231183"></a><a name="dns_usermanual_0007_zh-cn_topic_0035467699_ul46253231183"></a><ul id="dns_usermanual_0007_zh-cn_topic_0035467699_ul46253231183"><li>不能为空。</li><li>对于同一资源键值唯一。</li><li>长度不超过36个字符。</li><li>取值为不包含“=”、“*”、“&lt;”、“&gt;”、“\”、“,”、“|”和“/”的所有Unicode字符，且首尾字符不能为空格。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="31.313131313131315%" headers="mcps1.2.4.1.3 "><p id="dns_usermanual_0007_a6535efd5b28a446992be7db56bdbca33"><a name="dns_usermanual_0007_a6535efd5b28a446992be7db56bdbca33"></a><a name="dns_usermanual_0007_a6535efd5b28a446992be7db56bdbca33"></a>example_key1</p>
    </td>
    </tr>
    <tr id="dns_usermanual_0007_r89eaf5034c26447c8057d051da26301c"><td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.2.4.1.1 "><p id="dns_usermanual_0007_afc435752da464fffb58242f1410f227f"><a name="dns_usermanual_0007_afc435752da464fffb58242f1410f227f"></a><a name="dns_usermanual_0007_afc435752da464fffb58242f1410f227f"></a>值</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.505050505050505%" headers="mcps1.2.4.1.2 "><a name="dns_usermanual_0007_u388a9174749341a8a916b0093d32bc13"></a><a name="dns_usermanual_0007_u388a9174749341a8a916b0093d32bc13"></a><ul id="dns_usermanual_0007_u388a9174749341a8a916b0093d32bc13"><li>不能为空。</li><li>长度不超过43个字符。</li><li>取值为不包含“=”、“*”、“&lt;”、“&gt;”、“\”、“,”、“|”和“/”的所有Unicode字符，且首尾字符不能为空格。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="31.313131313131315%" headers="mcps1.2.4.1.3 "><p id="dns_usermanual_0007_zh-cn_topic_0035467699_p62904352179"><a name="dns_usermanual_0007_zh-cn_topic_0035467699_p62904352179"></a><a name="dns_usermanual_0007_zh-cn_topic_0035467699_p62904352179"></a>example_value1</p>
    </td>
    </tr>
    </tbody>
    </table>

2.  单击“确定”。
3.  返回“解析记录”页面。

    添加完成后，您可以在域名对应的记录集列表中查看已添加的记录集。当记录集的状态显示为“正常”时，表示记录集添加成功。


## 相关操作<a name="section18984203717105"></a>

更多关于MX类型记录集的配置指导，请参考[配置邮箱解析](https://support.huaweicloud.com/qs-dns/dns_qs_0004.html)。

