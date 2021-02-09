# 增加A类型记录集<a name="dns_usermanual_0007"></a>

## 操作场景<a name="section187281084528"></a>

当您想要直接使用域名访问网站、Web应用程序或者云服务器时，可以通过为域名增加A类型记录集实现。

更多关于记录集类型的介绍，请参见[记录集类型及配置规则](记录集类型及配置规则.md)。

## 约束与限制<a name="section10284161715528"></a>

已经完成网站或云服务器的搭建，并获取IPv4格式的IP地址。

## 操作步骤<a name="section3649104165212"></a>

1.  登录管理控制台。
2.  将鼠标悬浮于页面左侧的“![](figures/service-list.jpg)”，在服务列表中，选择“网络 \> 云解析服务”。

    进入“云解析”页面。


1.  在左侧树状导航栏，选择“域名解析 \> 公网解析”或者“域名解析 \> 内网解析”。

    进入域名列表页面。

2.  （可选）如果选择“内网解析”，请单击管理控制台左上角的![](figures/icon-region.png)，选择区域和项目。
3.  在待添加记录集的域名所在行，单击“名称”列的域名名称。
4.  单击“添加记录集”。

    进入“添加记录集”页面。

5.  设置记录集参数，如[表1](#table219785892310)所示。

    **表 1**  A类型记录集参数说明

    <a name="table219785892310"></a>
    <table><thead align="left"><tr id="row01931258112316"><th class="cellrowborder" valign="top" width="20.599999999999998%" id="mcps1.2.4.1.1"><p id="p0193658172318"><a name="p0193658172318"></a><a name="p0193658172318"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.01%" id="mcps1.2.4.1.2"><p id="p119395892316"><a name="p119395892316"></a><a name="p119395892316"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.39%" id="mcps1.2.4.1.3"><p id="p1419385816231"><a name="p1419385816231"></a><a name="p1419385816231"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row191931585230"><td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.4.1.1 "><p id="p18193155813234"><a name="p18193155813234"></a><a name="p18193155813234"></a>主机记录</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="p1193205814232"><a name="p1193205814232"></a><a name="p1193205814232"></a>解析域名的前缀。</p>
    <p id="p9491202813279"><a name="p9491202813279"></a><a name="p9491202813279"></a>例如创建的域名为“example.com”，其“主机记录”设置包括：</p>
    <a name="ul74911928142713"></a><a name="ul74911928142713"></a><ul id="ul74911928142713"><li>www：用于网站解析，表示解析的域名为“www.example.com”</li><li>空：用于网站解析，表示解析的域名为“example.com”</li><li>abc：用于子域名解析，表示解析的域名为“example.com”的子域名“abc.example.com”</li><li>mail：用于邮箱解析，表示解析的域名为“mail.example.com”</li><li>*：用于泛解析，表示解析的域名为“*.example.com”，匹配“example.com”的所有子域名。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.39%" headers="mcps1.2.4.1.3 "><p id="p181931058152317"><a name="p181931058152317"></a><a name="p181931058152317"></a>www</p>
    </td>
    </tr>
    <tr id="row1195175852312"><td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.4.1.1 "><p id="p1019517585235"><a name="p1019517585235"></a><a name="p1019517585235"></a>类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="p9195175822316"><a name="p9195175822316"></a><a name="p9195175822316"></a>记录集的类型，此处为A类型。</p>
    <p id="p8911154710176"><a name="p8911154710176"></a><a name="p8911154710176"></a>添加记录集时，如果提示解析记录集已经存在，说明待添加的记录集与已有的记录集存在限制关系或者冲突。</p>
    <p id="p091321341812"><a name="p091321341812"></a><a name="p091321341812"></a>详细内容请参见<a href="https://support.huaweicloud.com/dns_faq/dns_faq_016.html" target="_blank" rel="noopener noreferrer">为什么会提示解析记录集已经存在？</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.39%" headers="mcps1.2.4.1.3 "><p id="p181951958152315"><a name="p181951958152315"></a><a name="p181951958152315"></a>A – 将域名指向IPv4地址</p>
    </td>
    </tr>
    <tr id="row1049915211129"><td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.4.1.1 "><p id="p1880719311392"><a name="p1880719311392"></a><a name="p1880719311392"></a>别名</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="p1480715314392"><a name="p1480715314392"></a><a name="p1480715314392"></a>用于是否将此记录集关联至云服务资源实例。</p>
    <a name="ul780813115548"></a><a name="ul780813115548"></a><ul id="ul780813115548"><li>是：为此记录集关联云服务资源实例，详细说明请参见<a href="设置别名解析.md">设置记录集别名</a>。</li><li>否：不为此记录集关联云服务资源实例。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.39%" headers="mcps1.2.4.1.3 "><p id="p58071353915"><a name="p58071353915"></a><a name="p58071353915"></a>否</p>
    </td>
    </tr>
    <tr id="row197161021520"><td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.4.1.1 "><p id="p297271014152"><a name="p297271014152"></a><a name="p297271014152"></a>别名记录</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="p116117444409"><a name="p116117444409"></a><a name="p116117444409"></a>仅当“别名”设置为“是”时出现。</p>
    <p id="p2852542122614"><a name="p2852542122614"></a><a name="p2852542122614"></a>用于设置记录集关联的华为云服务资源实例。</p>
    <p id="p154382013182916"><a name="p154382013182916"></a><a name="p154382013182916"></a>记录集支持关联的华为云服务资源实例包括：云速建站、Web应用防火墙。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.39%" headers="mcps1.2.4.1.3 "><p id="p12972610131518"><a name="p12972610131518"></a><a name="p12972610131518"></a>-</p>
    </td>
    </tr>
    <tr id="row9195205842311"><td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.4.1.1 "><p id="p4690566311450"><a name="p4690566311450"></a><a name="p4690566311450"></a>线路类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="p63311110111714"><a name="p63311110111714"></a><a name="p63311110111714"></a>解析的线路类型用于DNS服务器在解析域名时，根据访问者的来源，返回对应的服务器IP地址。</p>
    <p id="p6627318120337"><a name="p6627318120337"></a><a name="p6627318120337"></a>默认值为“全网默认”。</p>
    <p id="p1552914404228"><a name="p1552914404228"></a><a name="p1552914404228"></a>仅支持为公网域名的记录集配置此参数。</p>
    <a name="ul867142417117"></a><a name="ul867142417117"></a><ul id="ul867142417117"><li>全网默认：默认线路类型，当未根据访问者来源设置解析线路时，系统会返回默认解析结果。</li><li>运营商线路解析：根据访问者所在运营商，设置解析线路，详细内容请参见<a href="配置运营商线路解析.md">配置运营商线路解析</a>。</li><li>地域解析：根据访问者所在地域，设置解析线路，详细内容请参见<a href="配置地域解析.md">配置地域线路解析</a>。</li><li>自定义线路：根据访问者所属IP网段，设置解析线路，详细内容请参见<a href="配置自定义线路解析.md">配置自定义线路解析</a>。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="33.39%" headers="mcps1.2.4.1.3 "><p id="p5391976911450"><a name="p5391976911450"></a><a name="p5391976911450"></a>全网默认</p>
    </td>
    </tr>
    <tr id="row7195185892312"><td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.4.1.1 "><p id="p5195185822318"><a name="p5195185822318"></a><a name="p5195185822318"></a>TTL(秒)</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="p01951585234"><a name="p01951585234"></a><a name="p01951585234"></a>解析记录在本地DNS服务器的缓存时间，以秒为单位。</p>
    <p id="p14211201373218"><a name="p14211201373218"></a><a name="p14211201373218"></a>默认值为“300秒”。取值范围为：1~2147483647</p>
    <p id="p2225120103717"><a name="p2225120103717"></a><a name="p2225120103717"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    <p id="p128523426263"><a name="p128523426263"></a><a name="p128523426263"></a>更多TTL相关内容请参见<a href="https://support.huaweicloud.com/dns_faq/dns_faq_013.html" target="_blank" rel="noopener noreferrer">什么是TTL值？</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.39%" headers="mcps1.2.4.1.3 "><p id="p16195115816233"><a name="p16195115816233"></a><a name="p16195115816233"></a>5分钟，即300s。</p>
    </td>
    </tr>
    <tr id="row17195105813235"><td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.4.1.1 "><p id="p319514581239"><a name="p319514581239"></a><a name="p319514581239"></a>值</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="p191823152340"><a name="p191823152340"></a><a name="p191823152340"></a>域名对应的IPv4地址。</p>
    <p id="p16575194113336"><a name="p16575194113336"></a><a name="p16575194113336"></a>最多可以输入50个不重复地址，多个地址之间以换行符分隔。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.39%" headers="mcps1.2.4.1.3 "><p id="p7195358102310"><a name="p7195358102310"></a><a name="p7195358102310"></a>192.168.12.2</p>
    <p id="p1195658142314"><a name="p1195658142314"></a><a name="p1195658142314"></a>192.168.12.3</p>
    </td>
    </tr>
    <tr id="row19985141952618"><td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.4.1.1 "><p id="p20661202842620"><a name="p20661202842620"></a><a name="p20661202842620"></a>权重</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="p667042892619"><a name="p667042892619"></a><a name="p667042892619"></a>可选参数，返回解析记录的权重比例。默认值为1，取值范围：0~1000。</p>
    <p id="p1960963902610"><a name="p1960963902610"></a><a name="p1960963902610"></a>仅支持为公网域名的记录集配置此参数。</p>
    <p id="p1681102817262"><a name="p1681102817262"></a><a name="p1681102817262"></a>当域名在同一解析线路中有多条相同类型的解析记录时，可以通过“权重”设置解析记录的响应比例。详细内容请参见<a href="配置权重解析.md">配置权重解析</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.39%" headers="mcps1.2.4.1.3 "><p id="p468810282264"><a name="p468810282264"></a><a name="p468810282264"></a>1</p>
    </td>
    </tr>
    <tr id="row1319511584234"><td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.4.1.1 "><p id="p131952588235"><a name="p131952588235"></a><a name="p131952588235"></a>标签</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="p421116377381"><a name="p421116377381"></a><a name="p421116377381"></a>可选参数，当“其他配置”开关打开时显示。</p>
    <p id="p127620395420"><a name="p127620395420"></a><a name="p127620395420"></a>记录集的标识，包括键和值，每个记录集可以创建10个标签。</p>
    <p id="p111951858102315"><a name="p111951858102315"></a><a name="p111951858102315"></a>键和值的命名规则请参见<a href="#table191971158112315">表2</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.39%" headers="mcps1.2.4.1.3 "><p id="p91953585235"><a name="p91953585235"></a><a name="p91953585235"></a>example_key1</p>
    <p id="p1195358102312"><a name="p1195358102312"></a><a name="p1195358102312"></a>example_value1</p>
    </td>
    </tr>
    <tr id="row8195185872311"><td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.4.1.1 "><p id="p6195145862318"><a name="p6195145862318"></a><a name="p6195145862318"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.01%" headers="mcps1.2.4.1.2 "><p id="p66251337192810"><a name="p66251337192810"></a><a name="p66251337192810"></a>可选参数，对域名的描述，当“其他配置”开关打开时显示。</p>
    <p id="p17140145133253"><a name="p17140145133253"></a><a name="p17140145133253"></a>长度不超过255个字符。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.39%" headers="mcps1.2.4.1.3 "><p id="p6195125819231"><a name="p6195125819231"></a><a name="p6195125819231"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  标签命名规则

    <a name="table191971158112315"></a>
    <table><thead align="left"><tr id="r4f5fd2fecc60424eb20075f35572eeb0"><th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0035467699_p132908358173"><a name="zh-cn_topic_0035467699_p132908358173"></a><a name="zh-cn_topic_0035467699_p132908358173"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="50.505050505050505%" id="mcps1.2.4.1.2"><p id="aa34a0c0cbae34a23b63e1882cf4a2c91"><a name="aa34a0c0cbae34a23b63e1882cf4a2c91"></a><a name="aa34a0c0cbae34a23b63e1882cf4a2c91"></a>规则</p>
    </th>
    <th class="cellrowborder" valign="top" width="31.313131313131315%" id="mcps1.2.4.1.3"><p id="aece629313e384a698796b7aff7821561"><a name="aece629313e384a698796b7aff7821561"></a><a name="aece629313e384a698796b7aff7821561"></a>举例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="rbb2718429c5141319dde3ac939f97ba9"><td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.2.4.1.1 "><p id="ae8044150f5804b42bd8632ccced6b72a"><a name="ae8044150f5804b42bd8632ccced6b72a"></a><a name="ae8044150f5804b42bd8632ccced6b72a"></a>键</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.505050505050505%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0035467699_ul46253231183"></a><a name="zh-cn_topic_0035467699_ul46253231183"></a><ul id="zh-cn_topic_0035467699_ul46253231183"><li>不能为空。</li><li>对于同一资源键值唯一。</li><li>长度不超过36个字符。</li><li>取值为不包含“=”、“*”、“&lt;”、“&gt;”、“\”、“,”、“|”和“/”的所有Unicode字符，且首尾字符不能为空格。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="31.313131313131315%" headers="mcps1.2.4.1.3 "><p id="a6535efd5b28a446992be7db56bdbca33"><a name="a6535efd5b28a446992be7db56bdbca33"></a><a name="a6535efd5b28a446992be7db56bdbca33"></a>example_key1</p>
    </td>
    </tr>
    <tr id="r89eaf5034c26447c8057d051da26301c"><td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.2.4.1.1 "><p id="afc435752da464fffb58242f1410f227f"><a name="afc435752da464fffb58242f1410f227f"></a><a name="afc435752da464fffb58242f1410f227f"></a>值</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.505050505050505%" headers="mcps1.2.4.1.2 "><a name="u388a9174749341a8a916b0093d32bc13"></a><a name="u388a9174749341a8a916b0093d32bc13"></a><ul id="u388a9174749341a8a916b0093d32bc13"><li>不能为空。</li><li>长度不超过43个字符。</li><li>取值为不包含“=”、“*”、“&lt;”、“&gt;”、“\”、“,”、“|”和“/”的所有Unicode字符，且首尾字符不能为空格。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="31.313131313131315%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0035467699_p62904352179"><a name="zh-cn_topic_0035467699_p62904352179"></a><a name="zh-cn_topic_0035467699_p62904352179"></a>example_value1</p>
    </td>
    </tr>
    </tbody>
    </table>

6.  单击“确定”。
7.  返回“解析记录”页面。

    添加完成后，您可以在域名对应的记录集列表中查看已添加的记录集。当记录集的状态显示为“正常”时，表示记录集添加成功。


## 相关操作<a name="section1485913521716"></a>

更多关于A类型记录集的配置指导，请参考：

-   [配置网站解析（华为云注册域名）](https://support.huaweicloud.com/qs-dns/dns_qs_0002.html)
-   [配置网站解析（第三方注册域名）](https://support.huaweicloud.com/qs-dns/zh-cn_topic_0035467699.html)

