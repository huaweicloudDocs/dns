# 增加AAAA类型记录集<a name="dns_usermanual_0008"></a>

## 操作场景<a name="section187281084528"></a>

当您想要直接使用域名访问网站、Web应用程序或者云服务器时，可以通过为域名增加AAAA类型记录集实现。

更多关于记录集类型的介绍，请参见[记录集类型及配置规则](记录集类型及配置规则.md)。

## 约束与限制<a name="section10284161715528"></a>

已经完成网站或云服务器的搭建，并获取IPv6格式的IP地址。

## 操作步骤<a name="section6412174644120"></a>

1.  登录管理控制台。
2.  将鼠标悬浮于页面左侧的“![](figures/service-list.jpg)”，在服务列表中，选择“网络  \> 云解析服务”。

    进入“云解析”页面。



1.  在左侧树状导航栏，选择“域名解析 \> 公网解析”或者“域名解析 \> 内网解析”。

    进入域名列表页面。

2.  （可选）如果选择“内网解析”，请单击管理控制台左上角的![](figures/icon-region.png)，选择区域和项目。
3.  在待添加记录集的域名所在行，单击“名称”列的域名名称。
4.  单击“添加记录集”。

    进入“添加记录集”页面。

5.  设置记录集参数，如[表1](#table3171006112739)所示。

    **表 1**  添加AAAA类型记录集参数说明

    <a name="table3171006112739"></a>
    <table><thead align="left"><tr id="row3069844212739"><th class="cellrowborder" valign="top" width="20.549999999999997%" id="mcps1.2.4.1.1"><p id="p2387414512739"><a name="p2387414512739"></a><a name="p2387414512739"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.12%" id="mcps1.2.4.1.2"><p id="p5475757412739"><a name="p5475757412739"></a><a name="p5475757412739"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33%" id="mcps1.2.4.1.3"><p id="p617852412739"><a name="p617852412739"></a><a name="p617852412739"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2712386512739"><td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.4.1.1 "><p id="p57077793115735"><a name="p57077793115735"></a><a name="p57077793115735"></a>主机记录</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.12%" headers="mcps1.2.4.1.2 "><p id="p498991411924"><a name="p498991411924"></a><a name="p498991411924"></a>解析域名的前缀。</p>
    <p id="p4490923311924"><a name="p4490923311924"></a><a name="p4490923311924"></a>例如创建的域名为“example.com”，其“主机记录”设置包括：</p>
    <a name="ul62101617105015"></a><a name="ul62101617105015"></a><ul id="ul62101617105015"><li>www：用于网站解析，表示解析的域名为“www.example.com”。</li><li>空：用于网站解析，表示解析的域名为“example.com”。<p id="dns_usermanual_0007_p210152475518"><a name="dns_usermanual_0007_p210152475518"></a><a name="dns_usermanual_0007_p210152475518"></a>主机记录置为空，还可用于为空头域名“@”添加解析。</p>
    </li><li>abc：用于子域名解析，表示解析的域名为“example.com”的子域名“abc.example.com”。</li><li>mail：用于邮箱解析，表示解析的域名为“mail.example.com”。</li><li>*：用于泛解析，表示解析的域名为“*.example.com”，匹配“example.com”的所有子域名。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p28898697122810"><a name="p28898697122810"></a><a name="p28898697122810"></a>www</p>
    </td>
    </tr>
    <tr id="row3782375412739"><td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.4.1.1 "><p id="p3932606412739"><a name="p3932606412739"></a><a name="p3932606412739"></a>类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.12%" headers="mcps1.2.4.1.2 "><p id="p3129459512739"><a name="p3129459512739"></a><a name="p3129459512739"></a>记录集的类型，此处为AAAA类型。</p>
    <p id="p8911154710176"><a name="p8911154710176"></a><a name="p8911154710176"></a>添加记录集时，如果提示解析记录集已经存在，说明待添加的记录集与已有的记录集存在限制关系或者冲突。</p>
    <p id="p091321341812"><a name="p091321341812"></a><a name="p091321341812"></a>详细内容请参见<a href="https://support.huaweicloud.com/dns_faq/dns_faq_016.html" target="_blank" rel="noopener noreferrer">为什么会提示解析记录集已经存在？</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p1943755514110"><a name="p1943755514110"></a><a name="p1943755514110"></a>AAAA – 将域名指向IPv6地址</p>
    </td>
    </tr>
    <tr id="row1452911241411"><td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.4.1.1 "><p id="p1880719311392"><a name="p1880719311392"></a><a name="p1880719311392"></a>别名</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.12%" headers="mcps1.2.4.1.2 "><p id="p1480715314392"><a name="p1480715314392"></a><a name="p1480715314392"></a>用于是否将此记录集关联至云服务资源实例。</p>
    <a name="ul780813115548"></a><a name="ul780813115548"></a><ul id="ul780813115548"><li>是：为此记录集关联云服务资源实例，详细说明请参见<a href="设置别名解析.md">设置记录集别名</a>。</li><li>否：不为此记录集关联云服务资源实例。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p58071353915"><a name="p58071353915"></a><a name="p58071353915"></a>否</p>
    </td>
    </tr>
    <tr id="row821636165310"><td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.4.1.1 "><p id="p432036175314"><a name="p432036175314"></a><a name="p432036175314"></a>别名记录</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.12%" headers="mcps1.2.4.1.2 "><p id="p203236165311"><a name="p203236165311"></a><a name="p203236165311"></a>仅当“别名”设置为“是”时出现。</p>
    <p id="p19832241155311"><a name="p19832241155311"></a><a name="p19832241155311"></a>用于设置记录集关联的华为云服务资源实例。</p>
    <p id="p2756195865318"><a name="p2756195865318"></a><a name="p2756195865318"></a>记录集支持关联的华为云服务资源实例包括：云速建站、Web应用防火墙。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p173103612534"><a name="p173103612534"></a><a name="p173103612534"></a>-</p>
    </td>
    </tr>
    <tr id="row3156703320747"><td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.4.1.1 "><p id="p4690566311450"><a name="p4690566311450"></a><a name="p4690566311450"></a>线路类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.12%" headers="mcps1.2.4.1.2 "><p id="p578885213504"><a name="p578885213504"></a><a name="p578885213504"></a>解析的线路类型用于DNS服务器在解析域名时，根据访问者的来源，返回对应的服务器IP地址。</p>
    <p id="p6627318120337"><a name="p6627318120337"></a><a name="p6627318120337"></a>默认值为“全网默认”。</p>
    <p id="p52031852192217"><a name="p52031852192217"></a><a name="p52031852192217"></a>仅支持为公网域名的记录集配置此参数。</p>
    <a name="ul867142417117"></a><a name="ul867142417117"></a><ul id="ul867142417117"><li>全网默认：默认线路类型，当未根据访问者来源设置解析线路时，系统会返回默认解析结果。</li><li>运营商线路解析：根据访问者所在运营商，设置解析线路，详细内容请参见<a href="配置运营商线路解析.md">配置运营商线路解析</a>。</li><li>地域解析：根据访问者所在地域，设置解析线路，详细内容请参见<a href="配置地域解析.md">配置地域线路解析</a>。</li><li>自定义线路：根据访问者所属IP网段，设置解析线路，详细内容请参见<a href="配置自定义线路解析.md">配置自定义线路解析</a>。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p5391976911450"><a name="p5391976911450"></a><a name="p5391976911450"></a>全网默认</p>
    </td>
    </tr>
    <tr id="row5115242612739"><td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.4.1.1 "><p id="p486947012739"><a name="p486947012739"></a><a name="p486947012739"></a>TTL(秒)</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.12%" headers="mcps1.2.4.1.2 "><p id="p5888275712739"><a name="p5888275712739"></a><a name="p5888275712739"></a>解析记录在本地DNS服务器的缓存时间，以秒为单位。</p>
    <p id="p103873299529"><a name="p103873299529"></a><a name="p103873299529"></a>默认值为“300秒”。取值范围为：1~2147483647</p>
    <p id="p7737113020523"><a name="p7737113020523"></a><a name="p7737113020523"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    <p id="p12104133155216"><a name="p12104133155216"></a><a name="p12104133155216"></a>更多TTL相关内容请参见<a href="https://support.huaweicloud.com/dns_faq/dns_faq_013.html" target="_blank" rel="noopener noreferrer">什么是TTL值？</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p477403312739"><a name="p477403312739"></a><a name="p477403312739"></a>5分钟，即300s。</p>
    </td>
    </tr>
    <tr id="row3916732112739"><td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.4.1.1 "><p id="p5771865512739"><a name="p5771865512739"></a><a name="p5771865512739"></a>值</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.12%" headers="mcps1.2.4.1.2 "><p id="p4469944512739"><a name="p4469944512739"></a><a name="p4469944512739"></a>域名对应的IPv6地址。</p>
    <p id="p16575194113336"><a name="p16575194113336"></a><a name="p16575194113336"></a>最多可以输入50个不重复地址，多个地址之间以换行符分隔。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p6593540212739"><a name="p6593540212739"></a><a name="p6593540212739"></a>ff03:0db8:85a3:0:0:8a2e:0370:7334</p>
    </td>
    </tr>
    <tr id="row1510111843017"><td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.4.1.1 "><p id="p16578933012"><a name="p16578933012"></a><a name="p16578933012"></a>权重</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.12%" headers="mcps1.2.4.1.2 "><p id="p13661098305"><a name="p13661098305"></a><a name="p13661098305"></a>可选参数，返回解析记录的权重比例。默认值为1，取值范围：0~1000。</p>
    <p id="p87229173020"><a name="p87229173020"></a><a name="p87229173020"></a>仅支持为公网域名的记录集配置此参数。</p>
    <p id="p147789173018"><a name="p147789173018"></a><a name="p147789173018"></a>当域名在同一解析线路中有多条相同类型的解析记录时，可以通过“权重”设置解析记录的响应比例。详细内容请参见<a href="配置权重解析.md">配置权重解析</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p139169183018"><a name="p139169183018"></a><a name="p139169183018"></a>1</p>
    </td>
    </tr>
    <tr id="row158111406234"><td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.4.1.1 "><p id="p174971657162412"><a name="p174971657162412"></a><a name="p174971657162412"></a>标签</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.12%" headers="mcps1.2.4.1.2 "><p id="p1414134716167"><a name="p1414134716167"></a><a name="p1414134716167"></a>可选参数，当“其他配置”开关打开时显示。</p>
    <p id="p127620395420"><a name="p127620395420"></a><a name="p127620395420"></a>记录集的标识，包括键和值，每个记录集可以创建10个标签。</p>
    <p id="p7512155710249"><a name="p7512155710249"></a><a name="p7512155710249"></a>键和值的命名规则请参见<a href="#table191971158112315">表2</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p19522657162412"><a name="p19522657162412"></a><a name="p19522657162412"></a>example_key1</p>
    <p id="p05253572248"><a name="p05253572248"></a><a name="p05253572248"></a>example_value1</p>
    </td>
    </tr>
    <tr id="row5602640133247"><td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.4.1.1 "><p id="p48629108133253"><a name="p48629108133253"></a><a name="p48629108133253"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.12%" headers="mcps1.2.4.1.2 "><p id="p2441229193412"><a name="p2441229193412"></a><a name="p2441229193412"></a>可选参数，对域名的描述，当“其他配置”开关打开时显示。</p>
    <p id="p17140145133253"><a name="p17140145133253"></a><a name="p17140145133253"></a>长度不超过255个字符。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p46174475133253"><a name="p46174475133253"></a><a name="p46174475133253"></a>The description of the hostname.</p>
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

6.  单击“确定”。
7.  返回“解析记录”页面。

    添加完成后，您可以在域名对应的记录集列表中查看已添加的记录集。当记录集的状态显示为“正常”时，表示记录集添加成功。


