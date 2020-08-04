# 增加PTR类型记录集<a name="dns_usermanual_0015"></a>

## 操作场景<a name="section187281084528"></a>

当您想要通过私网IP地址反向解析对应的内网域名时，可以通过PTR类型记录集实现。

更多关于记录集类型的介绍，请参见[解析管理简介](解析管理简介.md)。

## 约束与限制<a name="section10284161715528"></a>

-   仅支持为内网域名添加PTR类型记录集。
-   仅支持为顶级域是in-addr.arpa的内网域名添加PTR记录。

    对于公网域名，添加PTR记录的方法请参见[创建反向解析](创建反向解析.md)。


## 操作步骤<a name="section46571720104919"></a>

1.  登录管理控制台。
2.  选择“网络 \> 云解析服务”。

    进入“云解析”页面。



1.  在左侧树状导航栏，选择“域名解析 \> 内网解析”。

    进入“内网域名”页面。

2.  单击管理控制台左上角的![](figures/icon-region.png)，选择区域和项目。
3.  在待添加记录集的域名所在行，单击“名称”列的域名名称。
4.  单击“添加记录集”。

    进入“添加记录集”页面。


1.  设置记录集参数，如[表1](#table6260239895544)所示。

    **表 1**  添加PTR类型记录集参数说明

    <a name="table6260239895544"></a>
    <table><thead align="left"><tr id="row897191795544"><th class="cellrowborder" valign="top" width="18.86%" id="mcps1.2.4.1.1"><p id="p5563669295544"><a name="p5563669295544"></a><a name="p5563669295544"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.81%" id="mcps1.2.4.1.2"><p id="p1027823295544"><a name="p1027823295544"></a><a name="p1027823295544"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33%" id="mcps1.2.4.1.3"><p id="p2723046495544"><a name="p2723046495544"></a><a name="p2723046495544"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row5818398995544"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p1528265495544"><a name="p1528265495544"></a><a name="p1528265495544"></a>主机记录</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p2993546095544"><a name="p2993546095544"></a><a name="p2993546095544"></a>填写反向解析记录的名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p1150727695544"><a name="p1150727695544"></a><a name="p1150727695544"></a>10.1.168</p>
    <p id="p3645662495544"><a name="p3645662495544"></a><a name="p3645662495544"></a>例如，用户IP地址为192.168.1.10，则反向解析域名的完整格式为10.1.168.192.in-addr.arpa。</p>
    <a name="ul772510438411"></a><a name="ul772510438411"></a><ul id="ul772510438411"><li>若创建的域名为192.in-addr.arpa，则主机记录为10.1.168</li><li>若创建的域名为1.168.192.in-addr.arpa，则主机记录为10</li></ul>
    </td>
    </tr>
    <tr id="row5967416095544"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p176882195544"><a name="p176882195544"></a><a name="p176882195544"></a>类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p905683595544"><a name="p905683595544"></a><a name="p905683595544"></a>记录集的类型，此处为PTR类型。</p>
    <p id="p8911154710176"><a name="p8911154710176"></a><a name="p8911154710176"></a>添加记录集时，如果提示解析记录集已经存在，说明待添加的记录集与已有的记录集存在限制关系或者冲突。</p>
    <p id="p091321341812"><a name="p091321341812"></a><a name="p091321341812"></a>详细内容请参见<a href="https://support.huaweicloud.com/dns_faq/dns_faq_016.html" target="_blank" rel="noopener noreferrer">为什么会提示解析记录集已经存在？</a></p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p17976737164517"><a name="p17976737164517"></a><a name="p17976737164517"></a>PTR – 将IP地址指向域名</p>
    </td>
    </tr>
    <tr id="row2576416995544"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p652296395544"><a name="p652296395544"></a><a name="p652296395544"></a>TTL(秒)</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p5888275712739"><a name="p5888275712739"></a><a name="p5888275712739"></a>解析记录在本地DNS服务器的缓存时间，以秒为单位。</p>
    <p id="p103873299529"><a name="p103873299529"></a><a name="p103873299529"></a>默认值为“300秒”。取值范围为：1~2147483647</p>
    <p id="p7737113020523"><a name="p7737113020523"></a><a name="p7737113020523"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    <p id="p12104133155216"><a name="p12104133155216"></a><a name="p12104133155216"></a>更多TTL相关内容请参见<a href="https://support.huaweicloud.com/dns_faq/dns_faq_013.html" target="_blank" rel="noopener noreferrer">什么是TTL值？</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p477403312739"><a name="p477403312739"></a><a name="p477403312739"></a>5分钟，即300s。</p>
    </td>
    </tr>
    <tr id="row3669394995544"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p1941991095544"><a name="p1941991095544"></a><a name="p1941991095544"></a>值</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p2950884795544"><a name="p2950884795544"></a><a name="p2950884795544"></a>填写私网IP地址对应的内网域名，只能填写一个域名。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p4833148395544"><a name="p4833148395544"></a><a name="p4833148395544"></a>host.example.com.</p>
    </td>
    </tr>
    <tr id="row257814332309"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p125271425301"><a name="p125271425301"></a><a name="p125271425301"></a>标签</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p1414134716167"><a name="p1414134716167"></a><a name="p1414134716167"></a>可选参数，当“其他配置”开关打开时显示。</p>
    <p id="p98832015181812"><a name="p98832015181812"></a><a name="p98832015181812"></a>记录集的标识，包括键和值，每个记录集可以创建10个标签。</p>
    <p id="p1353994283013"><a name="p1353994283013"></a><a name="p1353994283013"></a>键和值的命名规则请参见<a href="#table191971158112315">表2</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p165498428308"><a name="p165498428308"></a><a name="p165498428308"></a>example_key1</p>
    <p id="p14553184210305"><a name="p14553184210305"></a><a name="p14553184210305"></a>example_value1</p>
    </td>
    </tr>
    <tr id="row3233016395544"><td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.4.1.1 "><p id="p149754295544"><a name="p149754295544"></a><a name="p149754295544"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.81%" headers="mcps1.2.4.1.2 "><p id="p2441229193412"><a name="p2441229193412"></a><a name="p2441229193412"></a>可选参数，对域名的描述，当“其他配置”开关打开时显示。</p>
    <p id="p17140145133253"><a name="p17140145133253"></a><a name="p17140145133253"></a>长度不超过255个字符。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.3 "><p id="p2748282695544"><a name="p2748282695544"></a><a name="p2748282695544"></a>The description of PTR record.</p>
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

2.  单击“确定”。
3.  返回“解析记录”页面。

    添加完成后，您可以在域名对应的记录集列表中查看已添加的记录集。当记录集的状态显示为“正常”时，表示记录集添加成功。


## 相关操作<a name="section18984203717105"></a>

更多关于PTR类型记录集的配置指导，请参考[怎样设置弹性云服务器的私网IP的反向解析？](https://support.huaweicloud.com/dns_faq/dns_faq_031.html)。

