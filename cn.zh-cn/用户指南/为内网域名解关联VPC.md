# 为内网域名解关联VPC<a name="dns_usermanual_0004"></a>

## 操作场景<a name="section901515124915"></a>

当用户创建的内网域名已经关联多个VPC时，如果要使该内网域名在某个关联VPC内不再生效，可以通过解关联VPC操作实现。

>![](public_sys-resources/icon-note.gif) **说明：** 
>如果内网域名当前仅关联一个VPC，则无法执行解关联VPC操作。若要使内网域名在当前VPC内不生效，可以直接删除该内网域名。

## 操作步骤<a name="section394212924913"></a>

1.  登录管理控制台。
2.  将鼠标悬浮于页面左侧的“![](figures/service-list.jpg)”，在服务列表中，选择“网络  \> 云解析服务”。

    进入“云解析”页面。

3.  在左侧树状导航栏，选择“域名解析 \> 内网解析”。

    进入“内网域名”页面。

4.  单击管理控制台左上角的![](figures/icon-region.png)，选择区域和项目。

1.  选择待解关联VPC的内网域名，单击“已关联的VPC”列下的“![](figures/icon-close.png)”，开始解关联VPC。

    **图 1**  已关联的VPC<a name="fig1993017326388"></a>  
    ![](figures/已关联的VPC-2.png "已关联的VPC-2")

2.  在“解关联VPC”对话框，单击“是”，完成解关联VPC。

    **图 2**  解关联VPC<a name="fig1145124813913"></a>  
    ![](figures/解关联VPC.png "解关联VPC")


