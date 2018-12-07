# 什么是CAA？<a name="dns_faq_032"></a>

CAA（Certification Authority Authorization，证书颁发机构授权）是一项防止HTTPS证书错误颁发的安全措施，遵从IETF RFC6844。从2017年9月8日起，要求CA（Certification Authority，证书颁发）机构执行CAA强制性检查。

## CAA标准<a name="section78537244532"></a>

CAA标准是指域名所有者在其域名DNS记录的CAA字段中，授权指定的CA机构为其域名颁发证书。

全球约有上百个CA机构有权发放HTTPS证书，证明您网站的身份。CAA标准可以使网站将指定CA机构列入白名单，仅授权指定CA机构为网站的域名颁发证书，防止HTTPS证书错误颁发。设置CAA记录是提高网站安全性的方法之一。

CA机构在为域名签发证书时执行CAA强制性检查：

-   如果检查域名的DNS记录，发现未设置CAA字段，则为该域名颁发证书。

    这种情况下，任何CA机构均可为该域名签发证书，存在HTTPS证书错误颁发的风险。

-   如果检查域名的DNS记录，在CAA字段发现获得授权，则为该域名颁发证书。
-   如果检查域名的DNS记录，在CAA字段发现未获得授权，则拒绝为该域名颁发证书，防止未授权HTTPS证书错误颁发。

## CAA记录<a name="section167971597533"></a>

CAA记录由一个\[flag\]标志字节和一个被称为属性的\[tag\]-\[value\]标（标签-值）对组成，可以将多个CAA字段添加到域名的DNS记录中。

**表 1**  CAA记录配置规则

<a name="table17725641112120"></a>
<table><thead align="left"><tr id="row187268412211"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.4.1.1"><p id="p17260416215"><a name="p17260416215"></a><a name="p17260416215"></a>目的</p>
</th>
<th class="cellrowborder" valign="top" width="36%" id="mcps1.2.4.1.2"><p id="p107261741132119"><a name="p107261741132119"></a><a name="p107261741132119"></a>样例</p>
</th>
<th class="cellrowborder" valign="top" width="47%" id="mcps1.2.4.1.3"><p id="p6726104110214"><a name="p6726104110214"></a><a name="p6726104110214"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row117262041172112"><td class="cellrowborder" rowspan="2" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p137261841172118"><a name="p137261841172118"></a><a name="p137261841172118"></a>设置单域名CAA记录</p>
</td>
<td class="cellrowborder" valign="top" width="36%" headers="mcps1.2.4.1.2 "><p id="p19726184114218"><a name="p19726184114218"></a><a name="p19726184114218"></a>domain.com.  CAA 0 issue "ca.example.com"</p>
</td>
<td class="cellrowborder" valign="top" width="47%" headers="mcps1.2.4.1.3 "><p id="p45933152818"><a name="p45933152818"></a><a name="p45933152818"></a>该字段表示只有ca.example.com可以为域名domain.com颁发证书，未经授权的第三方CA机构申请域名domain.com的HTTP证书将被拒绝。</p>
</td>
</tr>
<tr id="row127268411218"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p072612416211"><a name="p072612416211"></a><a name="p072612416211"></a>domain.com.  CAA 0 issue ";"</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p14726134152119"><a name="p14726134152119"></a><a name="p14726134152119"></a>该字段表示拒绝任何CA机构为域名domain.com颁发证书。</p>
</td>
</tr>
<tr id="row5726341122120"><td class="cellrowborder" rowspan="2" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p149740122612"><a name="p149740122612"></a><a name="p149740122612"></a>设置发送警报通知</p>
</td>
<td class="cellrowborder" valign="top" width="36%" headers="mcps1.2.4.1.2 "><p id="p1172624172110"><a name="p1172624172110"></a><a name="p1172624172110"></a>domain.com. CAA 0 iodef "mailto:admin@domain.com"</p>
</td>
<td class="cellrowborder" valign="top" width="47%" headers="mcps1.2.4.1.3 "><p id="p572613411210"><a name="p572613411210"></a><a name="p572613411210"></a>该字段用于当第三方尝试为一个未获得授权的域名申请证书时，通知CA机构向网站所有者发送警报邮件。</p>
</td>
</tr>
<tr id="row6726114118217"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p1472634172117"><a name="p1472634172117"></a><a name="p1472634172117"></a>domain.com. CAA 0 iodef "http:// domain.com/log/"</p>
<p id="p15945133714424"><a name="p15945133714424"></a><a name="p15945133714424"></a>domain.com. CAA 0 iodef "https:// domain.com/log/"</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p177261419213"><a name="p177261419213"></a><a name="p177261419213"></a>该字段用于记录尝试在其他CA申请HTTPS证书的行为。</p>
</td>
</tr>
<tr id="row1091554812514"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p15915144822517"><a name="p15915144822517"></a><a name="p15915144822517"></a>设置颁发通配符域名证书</p>
</td>
<td class="cellrowborder" valign="top" width="36%" headers="mcps1.2.4.1.2 "><p id="p591564812251"><a name="p591564812251"></a><a name="p591564812251"></a>domain.com. CAA 0 issuewild "ca.example.com"</p>
</td>
<td class="cellrowborder" valign="top" width="47%" headers="mcps1.2.4.1.3 "><p id="p69154484255"><a name="p69154484255"></a><a name="p69154484255"></a>该字段用于将通配符证书的颁发权限指定CA机构ca.example.com。</p>
</td>
</tr>
<tr id="row6815165112515"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p08156512257"><a name="p08156512257"></a><a name="p08156512257"></a>综合配置样例</p>
</td>
<td class="cellrowborder" valign="top" width="36%" headers="mcps1.2.4.1.2 "><p id="p76671429277"><a name="p76671429277"></a><a name="p76671429277"></a>domain.com. CAA 0 issue "ca.abc.com"</p>
<p id="p3667742162717"><a name="p3667742162717"></a><a name="p3667742162717"></a>domain.com. CAA 0 issuewild "ca.def.com"</p>
<p id="p166794217275"><a name="p166794217275"></a><a name="p166794217275"></a>domain.com. CAA 0 iodef "mailto:admin@domain.com"</p>
</td>
<td class="cellrowborder" valign="top" width="47%" headers="mcps1.2.4.1.3 "><p id="p79761441164912"><a name="p79761441164912"></a><a name="p79761441164912"></a>该字段表示域名domain.com：</p>
<a name="ul2285344104918"></a><a name="ul2285344104918"></a><ul id="ul2285344104918"><li>授权CA机构ca.abc.com颁发不限类型的证书。</li><li>授权CA机构ca.def.com颁发通配符证书。</li><li>禁止其他CA机构颁发证书。</li><li>当有违反设置规则的情况发生，CA机构发送通知邮件到admin@domain.com。</li></ul>
</td>
</tr>
</tbody>
</table>

## 验证CAA解析记录是否生效？<a name="section614411459319"></a>

CAA解析记录可以通过dig+trace命令查看域名是否生效以及具体的解析过程。

命令格式为：dig \[类型\] \[域名\] +trace。

示例如下：

**dig caa www.example.com +trace**

>![](public_sys-resources/icon-note.gif) **说明：**   
>如果操作系统没有自带dig命令，需要手动安装后才能使用。  

