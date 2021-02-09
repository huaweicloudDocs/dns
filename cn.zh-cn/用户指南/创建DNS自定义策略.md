# 创建DNS自定义策略<a name="dns_usermanual_0051"></a>

如果系统策略不满足授权要求，您可以创建自定义策略，并通过给用户组授予自定义策略来进行精细的访问控制，自定义策略是对系统策略的扩展和补充。

目前华为云支持以下两种方式创建自定义策略：

-   可视化视图：通过可视化视图创建自定义策略，无需了解JSON语法，按可视化视图导航栏选择云服务、操作、资源、条件等策略内容，可自动生成策略。
-   JSON视图：通过JSON视图创建自定义策略，可以在选择策略模板后，根据具体需求编辑策略内容；也可以直接在编辑框内编写JSON格式的策略内容。

如下以定制一个用户仅能修改DNS Zone的策略为例。分别采用可视化视图和JSON视图的配置方式创建自定义策略 。

具体创建步骤请参见：[创建自定义策略](https://support.huaweicloud.com/usermanual-iam/iam_01_0605.html)。本章为您介绍常用的DNS自定义策略样例。

## 可视化视图配置自定义策略<a name="section812210111810"></a>

1.  登录管理控制台。
2.  在控制台页面，将鼠标移动至右上方的账号名，在下拉列表中选择“统一身份认证”。
3.  在“统一身认证服务”页面左侧导航栏中，选择“权限”。
4.  在“权限”页面，单击右上方的“创建自定义策略”。

    进入“创建自定义策略”页面。

5.  输入“策略名称”。
6.  选择“作用范围”，即自定义策略的生效范围，根据服务的部署区域选择。服务部署区域，请参考[系统权限](https://support.huaweicloud.com/permissions/policy_list.html?product=dns)。

    -   全局级服务：系统权限中该服务的“所属区域”为“全局区域”，表示该服务为全局级服务。创建全局级服务的自定义策略时，作用范围选择“全局级服务”。给用户组授予该自定义策略时，需要在全局区域中进行。
    -   项目级服务：系统权限中该服务的“所属区域”为“除全局区域外其他区域”，表示该服务为项目级服务。创建项目级服务的自定义策略时，作用范围选择“项目级服务”。给用户组授予该自定义策略时，需要在除全局区域外其他区域中进行。

    因DNS是区域级项目，此处选择“项目级服务”。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果一个自定义策略中包含多个服务的授权语句，这些服务必须是同一属性，即都是全局级服务或者项目级服务。如果需要同时设置全局服务和项目级服务的自定义策略，请创建两条自定义策略，“作用范围”分别为“全局级服务”以及“项目级服务”。

7.  “策略配置方式”选择“可视化视图”。
8.  在“策略内容”下配置自定义策略。
    1.  选择“允许”或“拒绝”。
    2.  选择“云服务”。

        >![](public_sys-resources/icon-note.gif) **说明：** 
        >此处只能选择一个云服务，如需配置多个云服务的自定义策略，请在完成此条配置后，单击“添加权限”，创建多个服务的授权语句；或使用[JSON视图配置自定义策略](#section1627013490104)。

    3.  选择“操作”，根据需求勾选产品权限。
    4.  （可选）选择资源类型，如选择“特定类型”可以点击“通过资源路径指定”来指定需要授权的资源。
    5.  （可选）添加条件，单击“添加条件”，选择“条件键”，选择“运算符”，根据运算符类型填写相应的值。

        **表 1**  条件参数

        <a name="table138821346182817"></a>
        <table><thead align="left"><tr id="row588374612288"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p388319467284"><a name="p388319467284"></a><a name="p388319467284"></a>名称</p>
        </th>
        <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p1888312469289"><a name="p1888312469289"></a><a name="p1888312469289"></a>说明</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="row788315468289"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p138835462286"><a name="p138835462286"></a><a name="p138835462286"></a>条件值</p>
        </td>
        <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p18363236163117"><a name="p18363236163117"></a><a name="p18363236163117"></a>条件键表示策略语句的Condition元素中的键值。分为全局条件键和服务级条件键。</p>
        <a name="ul06811849123115"></a><a name="ul06811849123115"></a><ul id="ul06811849123115"><li>全局级条件键：前缀为“g:”，适用于所有操作，如<a href="#table183017270387">表2</a>所示。</li><li>服务级条件键：前缀为服务缩写，如“dns:”，仅适用于对应服务的操作。</li></ul>
        </td>
        </tr>
        <tr id="row138831946192811"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p5883946132817"><a name="p5883946132817"></a><a name="p5883946132817"></a>运算符</p>
        </td>
        <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p188314662813"><a name="p188314662813"></a><a name="p188314662813"></a>与条件键一起使用，构成完整的条件判断语句。</p>
        </td>
        </tr>
        <tr id="row4883114615283"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p128831746122810"><a name="p128831746122810"></a><a name="p128831746122810"></a>值</p>
        </td>
        <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p788410461285"><a name="p788410461285"></a><a name="p788410461285"></a>与条件键和运算符一起使用，当运算符需要某个关键字时，需要输入关键字的值，构成完整的条件判断语句。</p>
        </td>
        </tr>
        </tbody>
        </table>

        **表 2**  全局级请求条件

        <a name="table183017270387"></a>
        <table><thead align="left"><tr id="row230217277389"><th class="cellrowborder" valign="top" width="19.36193619361936%" id="mcps1.2.4.1.1"><p id="p18304162712388"><a name="p18304162712388"></a><a name="p18304162712388"></a>全局条件键</p>
        </th>
        <th class="cellrowborder" valign="top" width="17.27172717271727%" id="mcps1.2.4.1.2"><p id="p23042027133816"><a name="p23042027133816"></a><a name="p23042027133816"></a>条件类型</p>
        </th>
        <th class="cellrowborder" valign="top" width="63.366336633663366%" id="mcps1.2.4.1.3"><p id="p1530413278381"><a name="p1530413278381"></a><a name="p1530413278381"></a>说明</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="row10811143213814"><td class="cellrowborder" valign="top" width="19.36193619361936%" headers="mcps1.2.4.1.1 "><p id="p188121832133815"><a name="p188121832133815"></a><a name="p188121832133815"></a>g:CurrentTime</p>
        </td>
        <td class="cellrowborder" valign="top" width="17.27172717271727%" headers="mcps1.2.4.1.2 "><p id="p1881273210386"><a name="p1881273210386"></a><a name="p1881273210386"></a>时间</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.366336633663366%" headers="mcps1.2.4.1.3 "><p id="p1881283213384"><a name="p1881283213384"></a><a name="p1881283213384"></a>接收到鉴权请求的时间。以ISO 8601格式表示，例如：2012-11-11T23:59:59Z。</p>
        </td>
        </tr>
        <tr id="row17304627193814"><td class="cellrowborder" valign="top" width="19.36193619361936%" headers="mcps1.2.4.1.1 "><p id="p1048694683918"><a name="p1048694683918"></a><a name="p1048694683918"></a>g:DomainName</p>
        </td>
        <td class="cellrowborder" valign="top" width="17.27172717271727%" headers="mcps1.2.4.1.2 "><p id="p430432718388"><a name="p430432718388"></a><a name="p430432718388"></a>字符串</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.366336633663366%" headers="mcps1.2.4.1.3 "><p id="p14304227113819"><a name="p14304227113819"></a><a name="p14304227113819"></a>账号名称。</p>
        </td>
        </tr>
        <tr id="row930413271386"><td class="cellrowborder" valign="top" width="19.36193619361936%" headers="mcps1.2.4.1.1 "><p id="p1430462773810"><a name="p1430462773810"></a><a name="p1430462773810"></a>g:MFAPresent</p>
        </td>
        <td class="cellrowborder" valign="top" width="17.27172717271727%" headers="mcps1.2.4.1.2 "><p id="p2304327103810"><a name="p2304327103810"></a><a name="p2304327103810"></a>布尔值</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.366336633663366%" headers="mcps1.2.4.1.3 "><p id="p10304627123817"><a name="p10304627123817"></a><a name="p10304627123817"></a>是否使用MFA多因素认证方式获取Token。</p>
        </td>
        </tr>
        <tr id="row113066273384"><td class="cellrowborder" valign="top" width="19.36193619361936%" headers="mcps1.2.4.1.1 "><p id="p11307727193817"><a name="p11307727193817"></a><a name="p11307727193817"></a>g:MFAAge</p>
        </td>
        <td class="cellrowborder" valign="top" width="17.27172717271727%" headers="mcps1.2.4.1.2 "><p id="p163071427113815"><a name="p163071427113815"></a><a name="p163071427113815"></a>数值</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.366336633663366%" headers="mcps1.2.4.1.3 "><p id="p133077274389"><a name="p133077274389"></a><a name="p133077274389"></a>通过MFA多因素认证方式获取的Token的生效时间。该条件需要和g:MFAPresent一起使用。</p>
        </td>
        </tr>
        <tr id="row173089274389"><td class="cellrowborder" valign="top" width="19.36193619361936%" headers="mcps1.2.4.1.1 "><p id="p1930862733812"><a name="p1930862733812"></a><a name="p1930862733812"></a>g:ProjectName</p>
        </td>
        <td class="cellrowborder" valign="top" width="17.27172717271727%" headers="mcps1.2.4.1.2 "><p id="p18308182723812"><a name="p18308182723812"></a><a name="p18308182723812"></a>字符串</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.366336633663366%" headers="mcps1.2.4.1.3 "><p id="p530892753815"><a name="p530892753815"></a><a name="p530892753815"></a>项目名称。</p>
        </td>
        </tr>
        <tr id="row430842719383"><td class="cellrowborder" valign="top" width="19.36193619361936%" headers="mcps1.2.4.1.1 "><p id="p1430872717382"><a name="p1430872717382"></a><a name="p1430872717382"></a>g:ServiceName</p>
        </td>
        <td class="cellrowborder" valign="top" width="17.27172717271727%" headers="mcps1.2.4.1.2 "><p id="p3308122773811"><a name="p3308122773811"></a><a name="p3308122773811"></a>字符串</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.366336633663366%" headers="mcps1.2.4.1.3 "><p id="p163081627143811"><a name="p163081627143811"></a><a name="p163081627143811"></a>服务名称。</p>
        </td>
        </tr>
        <tr id="row530832712381"><td class="cellrowborder" valign="top" width="19.36193619361936%" headers="mcps1.2.4.1.1 "><p id="p1730811270387"><a name="p1730811270387"></a><a name="p1730811270387"></a>g:UserId</p>
        </td>
        <td class="cellrowborder" valign="top" width="17.27172717271727%" headers="mcps1.2.4.1.2 "><p id="p63097278386"><a name="p63097278386"></a><a name="p63097278386"></a>字符串</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.366336633663366%" headers="mcps1.2.4.1.3 "><p id="p7309827133819"><a name="p7309827133819"></a><a name="p7309827133819"></a>IAM用户ID。</p>
        </td>
        </tr>
        <tr id="row23091827173816"><td class="cellrowborder" valign="top" width="19.36193619361936%" headers="mcps1.2.4.1.1 "><p id="p14309122733811"><a name="p14309122733811"></a><a name="p14309122733811"></a>g:UserName</p>
        </td>
        <td class="cellrowborder" valign="top" width="17.27172717271727%" headers="mcps1.2.4.1.2 "><p id="p18309182710384"><a name="p18309182710384"></a><a name="p18309182710384"></a>字符串</p>
        </td>
        <td class="cellrowborder" valign="top" width="63.366336633663366%" headers="mcps1.2.4.1.3 "><p id="p1931052714381"><a name="p1931052714381"></a><a name="p1931052714381"></a>IAM用户名。</p>
        </td>
        </tr>
        </tbody>
        </table>


9.  （可选）在“策略配置方式”选择JSON视图，将可视化视图配置的策略内容转换为JSON语句，您可以在JSON视图中对策略内容进行修改。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果您修改后的JSON语句有语法错误，将无法创建策略，可以自行检查修改内容或单击界面弹窗中的“重置”，将JSON文件恢复到未修改状态。

10. （可选）如需创建多条自定义策略，请单击“添加权限”；也可在已创建的策略最右端单击“+”，复制此权限。
11. （可选）输入“策略描述”。
12. 单击“确定”，完成自定义策略的创建。
13. 参考[创建用户并授权使用DNS](创建用户并授权使用DNS.md)将新创建的自定义策略授予用户组，使得用户组中的用户具备自定义策略中的权限。

## JSON视图配置自定义策略<a name="section1627013490104"></a>

1.  登录管理控制台。
2.  在控制台页面，将鼠标移动至右上方的账号名，在下拉列表中选择“统一身份认证”。
3.  在“统一身认证服务”页面左侧导航栏中，选择“权限”。
4.  在“权限”页面，单击右上方的“创建自定义策略”。

    进入“创建自定义策略”页面。

5.  输入“策略名称”。
6.  选择“作用范围”，即自定义策略的生效范围，根据服务的部署区域选择。服务部署区域，请参考[系统权限](https://support.huaweicloud.com/permissions/policy_list.html?product=dns)。

    -   全局级服务：系统权限中该服务的“所属区域”为“全局区域”，表示该服务为全局级服务。创建全局级服务的自定义策略时，作用范围选择“全局级服务”。给用户组授予该自定义策略时，需要在全局区域中进行。
    -   项目级服务：系统权限中该服务的“所属区域”为“除全局区域外其他区域”，表示该服务为项目级服务。创建项目级服务的自定义策略时，作用范围选择“项目级服务”。给用户组授予该自定义策略时，需要在除全局区域外其他区域中进行。

    因DNS是区域级项目，此处选择“项目级服务”。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果一个自定义策略中包含多个服务的授权语句，这些服务必须是同一属性，即都是全局级服务或者项目级服务。如果需要同时设置全局服务和项目级服务的自定义策略，请创建两条自定义策略，“作用范围”分别为“全局级服务”以及“项目级服务”。

7.  “策略配置方式”选择“JSON视图”。
8.  （可选）在“策略内容”区域，单击“从已有策略复制”，例如选择“DNS FullAccess”作为模板。
9.  单击“确定”。
10. 修改模板中策略授权语句。

    -   作用（Effect）：允许（Allow）和拒绝（Deny）。
    -   权限集（Action）：写入各服务API授权项列表中“授权项”中的内容，例如："dns:zone:create"，来实现细粒度授权。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >自定义策略版本号（Version）固定为1.1，不可修改。

11. （可选）输入“策略描述”。
12. 单击“确定”后，系统会自动校验语法，如跳转到策略列表，则自定义策略创建成功；如提示“策略内容错误”，请按照语法规范进行修改。
13. 参考[创建用户并授权使用DNS](创建用户并授权使用DNS.md)将新创建的自定义策略授予用户组，使得用户组中的用户具备自定义策略中的权限。

## JSON视图自定义策略示例<a name="section51981826152017"></a>

-   示例1：授权用户创建域名，为域名添加记录集，并支持查看域名以及对应的记录集。

    ```
    {
        "Version": "1.1",
        "Statement": [
            {
                "Effect": "Allow",
                "Action": [
                    "dns:zone:create",
                    "dns:recordset:create",
                    "dns:zone:list"
    				"dns:recordset:list"
                ]
            },
            {
                "Effect": "Allow",
                "Action": [
                    "vpc:*:get*,
                    "vpc:*:list*"
                ]
            }
        ]
    }
    ```

-   示例2：拒绝用户删除DNS资源

    拒绝策略需要同时配合其他策略使用，否则没有实际作用。用户被授予的策略中，一个授权项的作用如果同时存在Alow和Deny，则遵循Deny优先原则。

    如果您给用户授予DNS FullAccess的系统策略，但不希望用户拥有DNS FullAccess中定义的删除DNS资源的权限，您可以创建一条拒绝删除DNS资源的自定义策略，然后同时将DNS FullAccess和拒绝策略授予用户，根据Deny优先原则，则用户可以对DNS执行除了删除外的所有操作。拒绝策略示例如下：

    ```
    { 
          "Version": "1.1", 
          "Statement": [ 
                { 
    		  "Effect": "Deny", 
                      "Action": [ 
                            "dns:*:delete*" 
                      ] 
                } 
          ] 
    }
    ```


-   示例3：多个授权项策略

    一个自定义策略中可以包含多个授权项，且除了可以包含本服务的授权项外，还可以包含其他服务的授权项，可以包含的其他服务必须跟本服务同属性，即都是项目级服务或都是全局级服务。多个授权语句策略描述如下：

    ```
    {
        "Version": "1.1",
        "Statement": [
            {
                "Effect": "Allow",
                "Action": [
                    "dns:zone:update",
                    "dns:zone:list"
                ]
            },
            {
                "Effect": "Allow",
                "Action": [
                    "vpc:subnets:create",
                    "vpc:vips:update"
                ]
            }
        ]
    }
    ```


