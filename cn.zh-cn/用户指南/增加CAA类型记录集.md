# 增加CAA类型记录集<a name="dns_usermanual_0014"></a>

## 操作场景<a name="section187281084528"></a>

当您想要指定为域名颁发HTTPS证书的授权CA机构时，可以通过为域名增加CAA类型记录集实现。

用于防止HTTPS证书错误签发。

更多关于记录集类型的介绍，请参见[记录集管理简介](记录集管理简介.md)。

## 约束与限制<a name="section10284161715528"></a>

仅支持为公网域名添加CAA类型记录集。

## 操作步骤<a name="section6412174644120"></a>

1.  登录管理控制台。
2.  选择“网络 \> 云解析服务”。

    进入“云解析”页面。


1.  在左侧树状导航栏，选择“域名解析 \> 公网解析”。

    进入“公网域名”页面。

2.  在待添加记录集的域名所在行，单击“名称”列的域名名称。
3.  单击“添加记录集”。

    进入“添加记录集”页面。


1.  设置记录集参数，如[表1](#table676063732817)所示。

    **表 1**  添加CAA类型记录集参数说明

    <a name="table676063732817"></a>
    <table><thead align="left"><tr id="row5778037182810"><th class="cellrowborder" valign="top" width="18.86%" id="mcps1.2.4.1.1"><p id="p7782133732811"><a name="p7782133732811"></a><a name="p7782133732811"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.81%" id="mcps1.2.4.1.2"><p id="p12788153715287"><a name="p12788153715287"></a><a name="p12788153715287"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33%" id="mcps1.2.4.1.3"><p id="p15792153719289"><a name="p15792153719289"></a><a name="p15792153719289"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row207951137172810"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p8798203752820"><a name="p8798203752820"></a><a name="p8798203752820"></a>主机记录</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p498991411924"><a name="p498991411924"></a><a name="p498991411924"></a>解析域名的前缀。</p>
    <p id="p4490923311924"><a name="p4490923311924"></a><a name="p4490923311924"></a>例如创建的域名为“example.com”，其“主机记录”设置包括：</p>
    <a name="ul62101617105015"></a><a name="ul62101617105015"></a><ul id="ul62101617105015"><li>www：用于网站解析，表示解析的域名为“www.example.com”</li><li>空：用于网站解析，表示解析的域名为“example.com”</li><li>abc：用于子域名解析，表示解析的域名为“example.com”的子域名“abc.example.com”</li><li>mail：用于邮箱解析，表示解析的域名为“mail.example.com”</li><li>*：用于泛解析，表示解析的域名为“*.example.com”，匹配“example.com”的所有子域名。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p78160372285"><a name="p78160372285"></a><a name="p78160372285"></a>置空</p>
    </td>
    </tr>
    <tr id="row13819837192816"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p982663713288"><a name="p982663713288"></a><a name="p982663713288"></a>类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p1383173742816"><a name="p1383173742816"></a><a name="p1383173742816"></a>记录集的类型，此处为CAA类型。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p7622132712445"><a name="p7622132712445"></a><a name="p7622132712445"></a>CAA – CA证书颁发机构授权校验</p>
    </td>
    </tr>
    <tr id="row9580163061611"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p1880719311392"><a name="p1880719311392"></a><a name="p1880719311392"></a>别名</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p1480715314392"><a name="p1480715314392"></a><a name="p1480715314392"></a>用于是否将此记录集关联至云服务资源实例。</p>
    <a name="ul780813115548"></a><a name="ul780813115548"></a><ul id="ul780813115548"><li>是：为此记录集关联云服务资源实例，详细说明请参见<a href="设置别名解析.md">设置记录集别名</a>。</li><li>否：不为此记录集关联云服务资源实例。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p58071353915"><a name="p58071353915"></a><a name="p58071353915"></a>否</p>
    </td>
    </tr>
    <tr id="row1332364317614"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p113238434611"><a name="p113238434611"></a><a name="p113238434611"></a>别名记录</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p203236165311"><a name="p203236165311"></a><a name="p203236165311"></a>仅当“别名”设置为“是”时出现。</p>
    <p id="p19832241155311"><a name="p19832241155311"></a><a name="p19832241155311"></a>用于设置记录集关联的华为云服务资源实例。</p>
    <p id="p2756195865318"><a name="p2756195865318"></a><a name="p2756195865318"></a>记录集支持关联的华为云服务资源实例包括：云速建站、Web应用防火墙。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p103241743264"><a name="p103241743264"></a><a name="p103241743264"></a>-</p>
    </td>
    </tr>
    <tr id="row183993742813"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p4690566311450"><a name="p4690566311450"></a><a name="p4690566311450"></a>线路类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p578885213504"><a name="p578885213504"></a><a name="p578885213504"></a>解析的线路类型用于DNS服务器在解析域名时，根据访问者的来源，返回对应的服务器IP地址。</p>
    <p id="p339175518918"><a name="p339175518918"></a><a name="p339175518918"></a>默认值为“全网默认”。</p>
    <p id="p1439145513918"><a name="p1439145513918"></a><a name="p1439145513918"></a>仅支持为公网域名的记录集配置此参数。</p>
    <a name="ul867142417117"></a><a name="ul867142417117"></a><ul id="ul867142417117"><li>全网默认：默认线路类型，当未根据访问者来源设置解析线路时，系统会返回默认解析结果。</li><li>运营商线路解析：根据访问者所在运营商，设置解析线路，详细内容请参见<a href="配置运营商线路解析.md">配置运营商线路解析</a>。</li><li>地域解析：根据访问者所在地域，设置解析线路，详细内容请参见<a href="配置地域解析.md">配置地域线路解析</a>。</li><li>自定义线路：根据访问者所属IP网段，设置解析线路，详细内容请参见<a href="配置自定义线路解析.md">配置自定义线路解析</a>。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p5391976911450"><a name="p5391976911450"></a><a name="p5391976911450"></a>全网默认</p>
    </td>
    </tr>
    <tr id="row3866173712813"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p9874163714287"><a name="p9874163714287"></a><a name="p9874163714287"></a>TTL(秒)</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p5888275712739"><a name="p5888275712739"></a><a name="p5888275712739"></a>解析记录在本地DNS服务器的缓存时间，以秒为单位。</p>
    <p id="p103873299529"><a name="p103873299529"></a><a name="p103873299529"></a>默认值为“300秒”。取值范围为：1~2147483647</p>
    <p id="p7737113020523"><a name="p7737113020523"></a><a name="p7737113020523"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    <p id="p12104133155216"><a name="p12104133155216"></a><a name="p12104133155216"></a>更多TTL相关内容请参见<a href="https://support.huaweicloud.com/dns_faq/dns_faq_013.html" target="_blank" rel="noopener noreferrer">什么是TTL值？</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p477403312739"><a name="p477403312739"></a><a name="p477403312739"></a>5分钟，即300s。</p>
    </td>
    </tr>
    <tr id="row9887737162813"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p689116371284"><a name="p689116371284"></a><a name="p689116371284"></a>值</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p19128114815389"><a name="p19128114815389"></a><a name="p19128114815389"></a>指定要授权的证书颁发机构，使其可以给域名或者子域名颁发证书。</p>
    <p id="p1372302745912"><a name="p1372302745912"></a><a name="p1372302745912"></a>最多可以输入50个不重复记录，多个记录之间以换行符分隔。</p>
    <p id="p82361147105913"><a name="p82361147105913"></a><a name="p82361147105913"></a>填写格式：[flag] [tag] [value]</p>
    <p id="p19865152383612"><a name="p19865152383612"></a><a name="p19865152383612"></a>配置规则：</p>
    <a name="ul4929101919515"></a><a name="ul4929101919515"></a><ul id="ul4929101919515"><li>flag：认证机构限制标志，定义为0~255无符号整型。常用取值为0。</li><li>tag：仅支持大小写字母和数字0~9，长度1~15，常用取值：<a name="dns_usermanual_0035_ul359754482613"></a><a name="dns_usermanual_0035_ul359754482613"></a><ul id="dns_usermanual_0035_ul359754482613"><li>issue：授权任何类型的域名证书</li><li>issuewild：授权通配符域名证书</li><li>iodef：指定违规申请证书通知策略</li></ul>
    </li><li>value：域名或用于违规通知的电子邮箱或Web地址。其值取决于[tag]的值，必须加双引号。取值范围：字符串（仅包含字母、数字、空格、-#*?&amp;_~=:;.@+^/!%），最长255字符。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p9310164811125"><a name="p9310164811125"></a><a name="p9310164811125"></a>0 issue "ca.abc.com"</p>
    <p id="p183101948161220"><a name="p183101948161220"></a><a name="p183101948161220"></a>0 issuewild "ca.def.com"</p>
    <p id="p831014831214"><a name="p831014831214"></a><a name="p831014831214"></a>0 iodef "mailto:admin@domain.com"</p>
    <p id="p143101248181211"><a name="p143101248181211"></a><a name="p143101248181211"></a>0 iodef "http:// domain.com/log/"</p>
    </td>
    </tr>
    <tr id="row343133417319"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p17871634153119"><a name="p17871634153119"></a><a name="p17871634153119"></a>权重</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p13661098305"><a name="p13661098305"></a><a name="p13661098305"></a>可选参数，解析记录的权重。默认值为1，取值范围：0~100。</p>
    <p id="p87229173020"><a name="p87229173020"></a><a name="p87229173020"></a>仅支持为公网域名的记录集配置此参数。</p>
    <p id="p147789173018"><a name="p147789173018"></a><a name="p147789173018"></a>当域名有多条某一类型的解析记录时，根据权重数值选择解析记录，权重数值越高，优先级越高。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p28903345318"><a name="p28903345318"></a><a name="p28903345318"></a>1</p>
    </td>
    </tr>
    <tr id="row1844134819292"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p1481158112914"><a name="p1481158112914"></a><a name="p1481158112914"></a>标签</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p1414134716167"><a name="p1414134716167"></a><a name="p1414134716167"></a>可选参数，当“其他配置”开关打开时显示。</p>
    <p id="p1347513731813"><a name="p1347513731813"></a><a name="p1347513731813"></a>记录集的标识，包括键和值，每个记录集可以创建10个标签。</p>
    <p id="p1849145832914"><a name="p1849145832914"></a><a name="p1849145832914"></a>键和值的命名规则请参见<a href="#table191971158112315">表2</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p205017586294"><a name="p205017586294"></a><a name="p205017586294"></a>example_key1</p>
    <p id="p11507158172920"><a name="p11507158172920"></a><a name="p11507158172920"></a>example_value1</p>
    </td>
    </tr>
    <tr id="row179379378281"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p094143782818"><a name="p094143782818"></a><a name="p094143782818"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p2441229193412"><a name="p2441229193412"></a><a name="p2441229193412"></a>可选参数，对域名的描述，当“其他配置”开关打开时显示。</p>
    <p id="p17140145133253"><a name="p17140145133253"></a><a name="p17140145133253"></a>长度不超过255个字符。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p8951437162817"><a name="p8951437162817"></a><a name="p8951437162817"></a>The description of the hostname.</p>
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
    <td class="cellrowborder" valign="top" width="50.505050505050505%" headers="mcps1.2.4.1.2 "><a name="dns_usermanual_0007_zh-cn_topic_0035467699_ul46253231183"></a><a name="dns_usermanual_0007_zh-cn_topic_0035467699_ul46253231183"></a><ul id="dns_usermanual_0007_zh-cn_topic_0035467699_ul46253231183"><li>不能为空。</li><li>对于同一资源键值唯一。</li><li>长度不超过36个字符。</li><li>取值为不包含“=”,“*”,“&lt;”,“&gt;”,“\”,“,”,“|”,“/”的所有Unicode字符，且首尾字符不能为空格。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="31.313131313131315%" headers="mcps1.2.4.1.3 "><p id="dns_usermanual_0007_a6535efd5b28a446992be7db56bdbca33"><a name="dns_usermanual_0007_a6535efd5b28a446992be7db56bdbca33"></a><a name="dns_usermanual_0007_a6535efd5b28a446992be7db56bdbca33"></a>example_key1</p>
    </td>
    </tr>
    <tr id="dns_usermanual_0007_r89eaf5034c26447c8057d051da26301c"><td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.2.4.1.1 "><p id="dns_usermanual_0007_afc435752da464fffb58242f1410f227f"><a name="dns_usermanual_0007_afc435752da464fffb58242f1410f227f"></a><a name="dns_usermanual_0007_afc435752da464fffb58242f1410f227f"></a>值</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.505050505050505%" headers="mcps1.2.4.1.2 "><a name="dns_usermanual_0007_u388a9174749341a8a916b0093d32bc13"></a><a name="dns_usermanual_0007_u388a9174749341a8a916b0093d32bc13"></a><ul id="dns_usermanual_0007_u388a9174749341a8a916b0093d32bc13"><li>不能为空。</li><li>长度不超过43个字符。</li><li>取值为不包含“=”,“*”,“&lt;”,“&gt;”,“\”,“,”,“|”,“/”的所有Unicode字符，且首尾字符不能为空格。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="31.313131313131315%" headers="mcps1.2.4.1.3 "><p id="dns_usermanual_0007_zh-cn_topic_0035467699_p62904352179"><a name="dns_usermanual_0007_zh-cn_topic_0035467699_p62904352179"></a><a name="dns_usermanual_0007_zh-cn_topic_0035467699_p62904352179"></a>example_value1</p>
    </td>
    </tr>
    </tbody>
    </table>

2.  单击“确定”，完成记录集的添加。

    您可以在域名对应的记录集列表中查看添加的记录集。当记录集的状态显示为“正常”时，表示记录集添加成功。


## 相关操作<a name="section18984203717105"></a>

更多关于CAA类型记录集的配置指导，请参考[设置CAA记录防止错误颁发HTTPS证书](https://support.huaweicloud.com/bestpractice-dns/zh-cn_topic_0107333199.html)。

