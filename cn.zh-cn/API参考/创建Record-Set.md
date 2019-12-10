# 创建Record Set<a name="zh-cn_topic_0037134404"></a>

## 功能介绍<a name="section2763065016101"></a>

创建单个Record Set。

## URI<a name="section53701671161015"></a>

POST /v2/zones/\{zone\_id\}/recordsets

参数说明请参见[表1](#table30807893173129)。

**表 1**  URI格式的参数说明

<a name="table30807893173129"></a>
<table><thead align="left"><tr id="row38661368173129"><th class="cellrowborder" valign="top" width="23.357664233576642%" id="mcps1.2.5.1.1"><p id="p14212988173129"><a name="p14212988173129"></a><a name="p14212988173129"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.03799620037996%" id="mcps1.2.5.1.2"><p id="p23287688173129"><a name="p23287688173129"></a><a name="p23287688173129"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.31826817318268%" id="mcps1.2.5.1.3"><p id="p1215993599"><a name="p1215993599"></a><a name="p1215993599"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="39.28607139286072%" id="mcps1.2.5.1.4"><p id="p1114682173129"><a name="p1114682173129"></a><a name="p1114682173129"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row6301875173129"><td class="cellrowborder" valign="top" width="23.357664233576642%" headers="mcps1.2.5.1.1 "><p id="p5124116173129"><a name="p5124116173129"></a><a name="p5124116173129"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.03799620037996%" headers="mcps1.2.5.1.2 "><p id="p65804667173129"><a name="p65804667173129"></a><a name="p65804667173129"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.31826817318268%" headers="mcps1.2.5.1.3 "><p id="p71592310916"><a name="p71592310916"></a><a name="p71592310916"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.28607139286072%" headers="mcps1.2.5.1.4 "><p id="p56820233173129"><a name="p56820233173129"></a><a name="p56820233173129"></a>所属zone ID。</p>
<p id="p2557111672911"><a name="p2557111672911"></a><a name="p2557111672911"></a>公网Zone ID可以通过<a href="查询公网Zone列表.md">查询公网Zone列表</a>获取。</p>
<p id="p22777371252"><a name="p22777371252"></a><a name="p22777371252"></a>内网Zone ID可以通过<a href="查询内网Zone列表.md">查询内网Zone列表</a>获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section44958995161021"></a>

-   参数说明

    **表 2**  请求样例的参数说明

    <a name="table9470531173211"></a>
    <table><thead align="left"><tr id="row60397351173211"><th class="cellrowborder" valign="top" width="22.040000000000003%" id="mcps1.2.5.1.1"><p id="p65819295173211"><a name="p65819295173211"></a><a name="p65819295173211"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.22%" id="mcps1.2.5.1.2"><p id="p42278174173211"><a name="p42278174173211"></a><a name="p42278174173211"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.82%" id="mcps1.2.5.1.3"><p id="p26309572173211"><a name="p26309572173211"></a><a name="p26309572173211"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.92%" id="mcps1.2.5.1.4"><p id="p67071922173211"><a name="p67071922173211"></a><a name="p67071922173211"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row65160710173211"><td class="cellrowborder" valign="top" width="22.040000000000003%" headers="mcps1.2.5.1.1 "><p id="p21415905173211"><a name="p21415905173211"></a><a name="p21415905173211"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.2.5.1.2 "><p id="p58188388173211"><a name="p58188388173211"></a><a name="p58188388173211"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82%" headers="mcps1.2.5.1.3 "><p id="p45293229173211"><a name="p45293229173211"></a><a name="p45293229173211"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.92%" headers="mcps1.2.5.1.4 "><p id="p5054941173211"><a name="p5054941173211"></a><a name="p5054941173211"></a>域名，后缀需以zone name结束且为FQDN（即以“.”号结束的完整主机名）。</p>
    <p id="p4141499817341"><a name="p4141499817341"></a><a name="p4141499817341"></a>当为公网域名时，子域名级别最多为5级。</p>
    <p id="p27471407151355"><a name="p27471407151355"></a><a name="p27471407151355"></a>域名格式不区分大小写，系统会将输入的大写字母统一转换为小写。</p>
    </td>
    </tr>
    <tr id="row34337486173211"><td class="cellrowborder" valign="top" width="22.040000000000003%" headers="mcps1.2.5.1.1 "><p id="p33154613173211"><a name="p33154613173211"></a><a name="p33154613173211"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.2.5.1.2 "><p id="p28540882173211"><a name="p28540882173211"></a><a name="p28540882173211"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82%" headers="mcps1.2.5.1.3 "><p id="p37402311173211"><a name="p37402311173211"></a><a name="p37402311173211"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.92%" headers="mcps1.2.5.1.4 "><p id="p43441715173211"><a name="p43441715173211"></a><a name="p43441715173211"></a>可选配置，对域名的描述。</p>
    <p id="p9966775173211"><a name="p9966775173211"></a><a name="p9966775173211"></a>长度不超过255个字符。</p>
    <p id="p174334035418"><a name="p174334035418"></a><a name="p174334035418"></a>默认值为空。</p>
    </td>
    </tr>
    <tr id="row52503862173211"><td class="cellrowborder" valign="top" width="22.040000000000003%" headers="mcps1.2.5.1.1 "><p id="p4265712173211"><a name="p4265712173211"></a><a name="p4265712173211"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.2.5.1.2 "><p id="p43588224173211"><a name="p43588224173211"></a><a name="p43588224173211"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82%" headers="mcps1.2.5.1.3 "><p id="p44233480173211"><a name="p44233480173211"></a><a name="p44233480173211"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.92%" headers="mcps1.2.5.1.4 "><p id="p29114279173211"><a name="p29114279173211"></a><a name="p29114279173211"></a>Record Set的类型。</p>
    <p id="p160041663916"><a name="p160041663916"></a><a name="p160041663916"></a>取值范围：A,AAAA,MX,CNAME,TXT, NS（仅限公网Zone）,SRV,PTR（仅限内网Zone）,CAA（仅限公网Zone）。</p>
    <p id="p1656255110557"><a name="p1656255110557"></a><a name="p1656255110557"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a>。</p>
    </td>
    </tr>
    <tr id="row44235645173211"><td class="cellrowborder" valign="top" width="22.040000000000003%" headers="mcps1.2.5.1.1 "><p id="p56753577173211"><a name="p56753577173211"></a><a name="p56753577173211"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.2.5.1.2 "><p id="p44923213173211"><a name="p44923213173211"></a><a name="p44923213173211"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82%" headers="mcps1.2.5.1.3 "><p id="p15148058212620"><a name="p15148058212620"></a><a name="p15148058212620"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.92%" headers="mcps1.2.5.1.4 "><p id="p44661732103918"><a name="p44661732103918"></a><a name="p44661732103918"></a>解析记录在本地DNS服务器的缓存时间，以秒为单位。</p>
    <p id="p1995185423811"><a name="p1995185423811"></a><a name="p1995185423811"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    <p id="p20437753173211"><a name="p20437753173211"></a><a name="p20437753173211"></a>取值范围：</p>
    <p id="p27764803173211"><a name="p27764803173211"></a><a name="p27764803173211"></a>1~2147483647。</p>
    <p id="p1752884719548"><a name="p1752884719548"></a><a name="p1752884719548"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="row59750658173211"><td class="cellrowborder" valign="top" width="22.040000000000003%" headers="mcps1.2.5.1.1 "><p id="p62596825173211"><a name="p62596825173211"></a><a name="p62596825173211"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.2.5.1.2 "><p id="p32296167173211"><a name="p32296167173211"></a><a name="p32296167173211"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82%" headers="mcps1.2.5.1.3 "><p id="p5792332173211"><a name="p5792332173211"></a><a name="p5792332173211"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.92%" headers="mcps1.2.5.1.4 "><p id="p8321575173211"><a name="p8321575173211"></a><a name="p8321575173211"></a>解析记录的值。不同类型解析记录对应的值的规则不同。</p>
    <p id="p813988173211"><a name="p813988173211"></a><a name="p813988173211"></a>如Type为AAAA类型，Value是域名对应的IPv6地址列表。</p>
    <p id="p59053902173211"><a name="p59053902173211"></a><a name="p59053902173211"></a>具体参见《云解析服务用户指南》中“<a href="https://support.huaweicloud.com/usermanual-dns/zh-cn_topic_0035467703.html" target="_blank" rel="noopener noreferrer">管理记录集</a>”章节的说明及请求样例。</p>
    </td>
    </tr>
    <tr id="row11879661194927"><td class="cellrowborder" valign="top" width="22.040000000000003%" headers="mcps1.2.5.1.1 "><p id="p24376203194927"><a name="p24376203194927"></a><a name="p24376203194927"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.22%" headers="mcps1.2.5.1.2 "><p id="p28315431194927"><a name="p28315431194927"></a><a name="p28315431194927"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82%" headers="mcps1.2.5.1.3 "><p id="p1170236162"><a name="p1170236162"></a><a name="p1170236162"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.92%" headers="mcps1.2.5.1.4 "><p id="p20210224194927"><a name="p20210224194927"></a><a name="p20210224194927"></a>资源标签。详细信息请参见<a href="数据结构.md#table19530794112436">表2</a>。</p>
    <p id="p878665895419"><a name="p878665895419"></a><a name="p878665895419"></a>默认值为空。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    为Zone ID为“2c9eb155587194ec01587224c9f90149”域名添加记录集。

    ```
    POST https://{DNS_Endpoint}/v2/zones/2c9eb155587194ec01587224c9f90149/recordsets
    ```

    -   A类型

        ```
        {
            "name": "www.example.com.",
            "description": "This is an example record set.",
            "type": "A",
            "ttl": 3600,
            "records": [
                "192.168.10.1",
                "192.168.10.2"
            ],
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```

    -   AAAA类型

        ```
        {
            "name": "www.example.com.",
            "description": "This is an example record set.",
            "type": "AAAA",
            "ttl": 3600,
            "records": [
                "fe80:0:0:0:202:b3ff:fe1e:8329",
                "ff03:0db8:85a3:0:0:8a2e:0370:7334"
            ],
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```

    -   MX类型

        ```
        {
            "name": "www.example.com.",
            "description": "This is an example record set.",
            "type": "MX",
            "ttl": 3600,
            "records": [
                "1 mail.example.com"
            ],
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```

    -   CNAME类型

        ```
        {
            "name": "sale.example.com.",
            "description": "This is an example record set.",
            "type": "CNAME",
            "ttl": 3600,
            "records": [
                "server1.example.com"
            ],
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```

    -   TXT类型

        ```
        {
            "name": "server1.example.com.",
            "description": "This is an example record set.",
            "type": "TXT",
            "ttl": 300,
            "records": [
                "\"This host is used for sale.\""
            ],
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```

    -   NS类型

        ```
        {
            "name": "server1.example.com.",
            "description": "This is an example record set.",
            "type": "NS",
            "ttl": 300,
            "records": [
                "node1.example.com.",
                "node2.example.com."
            ],
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```

    -   SRV类型

        ```
        {
            "name": "_sip._tcp.example.com.",
            "description": "This is an example record set.",
            "type": "SRV",
            "ttl": 300,
            "records": [
                "3 60 2176 sipserver.example.com.",
                "10 100 2176 sipserver.example.com."
            ],
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```

    -   PTR类型

        ```
        {
            "name": "1.1.168.192.in-addr.arpa.",
            "description": "This is an example record set.",
            "type": "PTR",
            "ttl": 300,
            "records": [
                "webserver.example.com."
            ],
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        
        ```

    -   CAA类型

        ```
        {
            "name": "www.example.com.",
            "description": "This is an example record set.",
            "type": "CAA",
            "ttl": 300,
            "records": [
                "0 issue \"example.com\"",
                "0 issuewild \"www.certinomis.com\"",
                "0 iodef \"mailto:xx@example.org\"",
                "0 iodef \"http://iodef.example.com\""
            ],
            "tags": [
                {
                  "key": "key1",
                  "value": "value1"
                }
            ]
        }
        ```



## 响应<a name="section40090803161031"></a>

-   参数说明

    **表 3**  响应样例的参数说明

    <a name="table7669703175323"></a>
    <table><thead align="left"><tr id="row52466955175323"><th class="cellrowborder" valign="top" width="18.23%" id="mcps1.2.4.1.1"><p id="p2769858175323"><a name="p2769858175323"></a><a name="p2769858175323"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.77%" id="mcps1.2.4.1.2"><p id="p46296309175323"><a name="p46296309175323"></a><a name="p46296309175323"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62%" id="mcps1.2.4.1.3"><p id="p62697904175323"><a name="p62697904175323"></a><a name="p62697904175323"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row47909891175323"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="p64112397175323"><a name="p64112397175323"></a><a name="p64112397175323"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.4.1.2 "><p id="p1660870175323"><a name="p1660870175323"></a><a name="p1660870175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p1249204175323"><a name="p1249204175323"></a><a name="p1249204175323"></a>Record Set的ID。</p>
    </td>
    </tr>
    <tr id="row6942422175323"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="p64097412175323"><a name="p64097412175323"></a><a name="p64097412175323"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.4.1.2 "><p id="p44990515175323"><a name="p44990515175323"></a><a name="p44990515175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p32019574175323"><a name="p32019574175323"></a><a name="p32019574175323"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="row61442071175323"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="p51194416175323"><a name="p51194416175323"></a><a name="p51194416175323"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.4.1.2 "><p id="p63301991175323"><a name="p63301991175323"></a><a name="p63301991175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p43966660175323"><a name="p43966660175323"></a><a name="p43966660175323"></a>Record Set的描述信息。</p>
    </td>
    </tr>
    <tr id="row2176746175323"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="p11805366175323"><a name="p11805366175323"></a><a name="p11805366175323"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.4.1.2 "><p id="p1051908175323"><a name="p1051908175323"></a><a name="p1051908175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p10043845175323"><a name="p10043845175323"></a><a name="p10043845175323"></a>托管该记录的zone_id。</p>
    </td>
    </tr>
    <tr id="row61212722175323"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="p8318586175323"><a name="p8318586175323"></a><a name="p8318586175323"></a>zone_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.4.1.2 "><p id="p31287919175323"><a name="p31287919175323"></a><a name="p31287919175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p16372315175323"><a name="p16372315175323"></a><a name="p16372315175323"></a>托管该记录的zone_name。</p>
    </td>
    </tr>
    <tr id="row38132372175323"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="p37461920175323"><a name="p37461920175323"></a><a name="p37461920175323"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.4.1.2 "><p id="p27536075175323"><a name="p27536075175323"></a><a name="p27536075175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p24813356175323"><a name="p24813356175323"></a><a name="p24813356175323"></a>记录类型。</p>
    <p id="p173531225174112"><a name="p173531225174112"></a><a name="p173531225174112"></a>取值范围：A，AAAA，MX，CNAME，TXT，NS（仅限公网Zone），SRV，PTR（仅限内网Zone），CAA（仅限公网Zone）。</p>
    <p id="p15442435577"><a name="p15442435577"></a><a name="p15442435577"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a>。</p>
    </td>
    </tr>
    <tr id="row20796819175323"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="p4811553175323"><a name="p4811553175323"></a><a name="p4811553175323"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.4.1.2 "><p id="p47559731175323"><a name="p47559731175323"></a><a name="p47559731175323"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p123031523174010"><a name="p123031523174010"></a><a name="p123031523174010"></a>解析记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="p1030317233408"><a name="p1030317233408"></a><a name="p1030317233408"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    </td>
    </tr>
    <tr id="row13978060175323"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="p43388342175323"><a name="p43388342175323"></a><a name="p43388342175323"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.4.1.2 "><p id="p29596719175323"><a name="p29596719175323"></a><a name="p29596719175323"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p30492925175323"><a name="p30492925175323"></a><a name="p30492925175323"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="row23148559175323"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="p36524189175323"><a name="p36524189175323"></a><a name="p36524189175323"></a>create_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.4.1.2 "><p id="p47080972175323"><a name="p47080972175323"></a><a name="p47080972175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p15737135175323"><a name="p15737135175323"></a><a name="p15737135175323"></a>创建时间。</p>
    <p id="p91253279589"><a name="p91253279589"></a><a name="p91253279589"></a>格式：yyyy-MM-dd'T'HH:mm:ss.SSS</p>
    </td>
    </tr>
    <tr id="row33465792175323"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="p42570937175323"><a name="p42570937175323"></a><a name="p42570937175323"></a>update_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.4.1.2 "><p id="p27449776175323"><a name="p27449776175323"></a><a name="p27449776175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p63703533175323"><a name="p63703533175323"></a><a name="p63703533175323"></a>更新时间。</p>
    <p id="p1291282918585"><a name="p1291282918585"></a><a name="p1291282918585"></a>格式：yyyy-MM-dd'T'HH:mm:ss.SSS</p>
    </td>
    </tr>
    <tr id="row17850883175323"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="p36228271175323"><a name="p36228271175323"></a><a name="p36228271175323"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.4.1.2 "><p id="p6480061175323"><a name="p6480061175323"></a><a name="p6480061175323"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p65781854175323"><a name="p65781854175323"></a><a name="p65781854175323"></a>资源状态。</p>
    <p id="p17497161105814"><a name="p17497161105814"></a><a name="p17497161105814"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="row61184424175323"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="p49633411175323"><a name="p49633411175323"></a><a name="p49633411175323"></a>default</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.4.1.2 "><p id="p56048766175323"><a name="p56048766175323"></a><a name="p56048766175323"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p37768157175323"><a name="p37768157175323"></a><a name="p37768157175323"></a>标识是否由系统默认生成，系统默认生成的Record Set不能删除。</p>
    </td>
    </tr>
    <tr id="row15199048201026"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="p23163408201026"><a name="p23163408201026"></a><a name="p23163408201026"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.4.1.2 "><p id="p40653752201026"><a name="p40653752201026"></a><a name="p40653752201026"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p4619625201026"><a name="p4619625201026"></a><a name="p4619625201026"></a>该Record Set所属的项目ID。</p>
    </td>
    </tr>
    <tr id="row3965248419366"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="p2132803819366"><a name="p2132803819366"></a><a name="p2132803819366"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.4.1.2 "><p id="p1127763319366"><a name="p1127763319366"></a><a name="p1127763319366"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62%" headers="mcps1.2.4.1.3 "><p id="p4107308719366"><a name="p4107308719366"></a><a name="p4107308719366"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p8605123216466"><a name="p8605123216466"></a><a name="p8605123216466"></a>详细信息请参见<a href="#table52442344175457">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  links参数说明

    <a name="table52442344175457"></a>
    <table><thead align="left"><tr id="row58979189175457"><th class="cellrowborder" valign="top" width="18.3018301830183%" id="mcps1.2.4.1.1"><p id="p46156243175457"><a name="p46156243175457"></a><a name="p46156243175457"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.591959195919593%" id="mcps1.2.4.1.2"><p id="p47668234175457"><a name="p47668234175457"></a><a name="p47668234175457"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.10621062106211%" id="mcps1.2.4.1.3"><p id="p35921708175457"><a name="p35921708175457"></a><a name="p35921708175457"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row54859922175457"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p14468674175457"><a name="p14468674175457"></a><a name="p14468674175457"></a>self</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.591959195919593%" headers="mcps1.2.4.1.2 "><p id="p31111955175457"><a name="p31111955175457"></a><a name="p31111955175457"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.10621062106211%" headers="mcps1.2.4.1.3 "><p id="p37040428175457"><a name="p37040428175457"></a><a name="p37040428175457"></a>当前资源的链接。</p>
    </td>
    </tr>
    <tr id="row1639371017497"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
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
        "id": "2c9eb155587228570158722b6ac30007",
        "name": "www.example.com.",
        "description": "This is an example record set.",
        "type": "A",
        "ttl": 300,
        "records": [
            "192.168.10.1",
            "192.168.10.2"
        ],
        "status": "PENDING_CREATE",
        "links": {
            "self": "https://Endpoint/v2/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587228570158722b6ac30007"
        },
        "zone_id": "2c9eb155587194ec01587224c9f90149",
        "zone_name": "example.com.",
        "create_at": "2016-11-17T12:03:17.827",
        "update_at": null,
        "default": false,
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c"
    }
    
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

