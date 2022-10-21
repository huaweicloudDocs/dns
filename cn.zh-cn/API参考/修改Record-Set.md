# 修改Record Set<a name="dns_api_64006"></a>

## 功能介绍<a name="section49332166"></a>

修改单个Record Set。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=DNS&api=UpdateRecordSet)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI<a name="section41336317"></a>

PUT /v2/zones/\{zone\_id\}/recordsets/\{recordset\_id\}

参数说明请参见[表1](#table52104579)。

**表 1**  URI格式的参数说明

<a name="table52104579"></a>
<table><thead align="left"><tr id="row50570707"><th class="cellrowborder" valign="top" width="22.240000000000002%" id="mcps1.2.5.1.1"><p id="p2586631"><a name="p2586631"></a><a name="p2586631"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.840000000000003%" id="mcps1.2.5.1.2"><p id="p8190559"><a name="p8190559"></a><a name="p8190559"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="21.48%" id="mcps1.2.5.1.3"><p id="p21461417487"><a name="p21461417487"></a><a name="p21461417487"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="39.440000000000005%" id="mcps1.2.5.1.4"><p id="p59455556"><a name="p59455556"></a><a name="p59455556"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row51170717"><td class="cellrowborder" valign="top" width="22.240000000000002%" headers="mcps1.2.5.1.1 "><p id="p51187411"><a name="p51187411"></a><a name="p51187411"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.840000000000003%" headers="mcps1.2.5.1.2 "><p id="p52539597"><a name="p52539597"></a><a name="p52539597"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="21.48%" headers="mcps1.2.5.1.3 "><p id="p714101419486"><a name="p714101419486"></a><a name="p714101419486"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.440000000000005%" headers="mcps1.2.5.1.4 "><p id="p27848947"><a name="p27848947"></a><a name="p27848947"></a>所属zone的ID。</p>
<p id="p2171125516411"><a name="p2171125516411"></a><a name="p2171125516411"></a>公网Zone ID可以通过<a href="查询公网Zone列表.md">查询公网Zone列表</a>获取。</p>
<p id="p22777371252"><a name="p22777371252"></a><a name="p22777371252"></a>内网Zone ID可以通过<a href="查询内网Zone列表.md">查询内网Zone列表</a>获取。</p>
</td>
</tr>
<tr id="row49313939"><td class="cellrowborder" valign="top" width="22.240000000000002%" headers="mcps1.2.5.1.1 "><p id="p35006119"><a name="p35006119"></a><a name="p35006119"></a>recordset_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.840000000000003%" headers="mcps1.2.5.1.2 "><p id="p16923420"><a name="p16923420"></a><a name="p16923420"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="21.48%" headers="mcps1.2.5.1.3 "><p id="p414121454818"><a name="p414121454818"></a><a name="p414121454818"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.440000000000005%" headers="mcps1.2.5.1.4 "><p id="p28619802"><a name="p28619802"></a><a name="p28619802"></a>待修改recordset的ID。</p>
<p id="p12406443193011"><a name="p12406443193011"></a><a name="p12406443193011"></a>可以通过<a href="查询单个Zone下Record-Set列表.md">查询单个Zone下Record Set列表</a>获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section36482533"></a>

-   参数说明

    **表 2**  请求样例的参数说明

    <a name="table9470531173211"></a>
    <table><thead align="left"><tr id="row60397351173211"><th class="cellrowborder" valign="top" width="22.45%" id="mcps1.2.5.1.1"><p id="p65819295173211"><a name="p65819295173211"></a><a name="p65819295173211"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.29%" id="mcps1.2.5.1.2"><p id="p42278174173211"><a name="p42278174173211"></a><a name="p42278174173211"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.89%" id="mcps1.2.5.1.3"><p id="p26309572173211"><a name="p26309572173211"></a><a name="p26309572173211"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.37%" id="mcps1.2.5.1.4"><p id="p67071922173211"><a name="p67071922173211"></a><a name="p67071922173211"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2428104916113"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p21415905173211"><a name="p21415905173211"></a><a name="p21415905173211"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.5.1.2 "><p id="p58188388173211"><a name="p58188388173211"></a><a name="p58188388173211"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.5.1.3 "><p id="p45293229173211"><a name="p45293229173211"></a><a name="p45293229173211"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p5054941173211"><a name="p5054941173211"></a><a name="p5054941173211"></a>域名，后缀需以zone name结束且为FQDN（即以“.”号结束的完整主机名）。</p>
    <p id="p4141499817341"><a name="p4141499817341"></a><a name="p4141499817341"></a>当为公网域名时，子域名级别最多为5级。</p>
    <p id="p27471407151355"><a name="p27471407151355"></a><a name="p27471407151355"></a>域名格式不区分大小写，系统会将输入的大写字母统一转换为小写。</p>
    </td>
    </tr>
    <tr id="row34337486173211"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p33154613173211"><a name="p33154613173211"></a><a name="p33154613173211"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.5.1.2 "><p id="p28540882173211"><a name="p28540882173211"></a><a name="p28540882173211"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.5.1.3 "><p id="p37402311173211"><a name="p37402311173211"></a><a name="p37402311173211"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p43441715173211"><a name="p43441715173211"></a><a name="p43441715173211"></a>可选配置，对域名的描述。</p>
    <p id="p9966775173211"><a name="p9966775173211"></a><a name="p9966775173211"></a>长度不超过255个字符。</p>
    <p id="p513811402423"><a name="p513811402423"></a><a name="p513811402423"></a>如果为空，表示维持原值。</p>
    <p id="p86941318184212"><a name="p86941318184212"></a><a name="p86941318184212"></a>默认值为空。</p>
    </td>
    </tr>
    <tr id="row1640071516215"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p4265712173211"><a name="p4265712173211"></a><a name="p4265712173211"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.5.1.2 "><p id="p43588224173211"><a name="p43588224173211"></a><a name="p43588224173211"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.5.1.3 "><p id="p44233480173211"><a name="p44233480173211"></a><a name="p44233480173211"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p29114279173211"><a name="p29114279173211"></a><a name="p29114279173211"></a>Record Set的类型。</p>
    <p id="p160041663916"><a name="p160041663916"></a><a name="p160041663916"></a>取值范围：A、AAAA、MX、CNAME、TXT、NS（仅限公网Zone）、SRV、PTR（仅限内网Zone）、CAA（仅限公网Zone）。</p>
    <p id="p1656255110557"><a name="p1656255110557"></a><a name="p1656255110557"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a>。</p>
    </td>
    </tr>
    <tr id="row44235645173211"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p56753577173211"><a name="p56753577173211"></a><a name="p56753577173211"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.5.1.2 "><p id="p44923213173211"><a name="p44923213173211"></a><a name="p44923213173211"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.5.1.3 "><p id="p45055368173211"><a name="p45055368173211"></a><a name="p45055368173211"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p123031523174010"><a name="p123031523174010"></a><a name="p123031523174010"></a>解析记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="p1030317233408"><a name="p1030317233408"></a><a name="p1030317233408"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    <p id="p20437753173211"><a name="p20437753173211"></a><a name="p20437753173211"></a>取值范围：</p>
    <a name="ul12272931135310"></a><a name="ul12272931135310"></a><ul id="ul12272931135310"><li>公网解析：1~2147483647。</li><li>内网解析：300~2147483647。</li></ul>
    <p id="p16253220614"><a name="p16253220614"></a><a name="p16253220614"></a>如果为空，表示维持原值。</p>
    <p id="p8877142595919"><a name="p8877142595919"></a><a name="p8877142595919"></a>默认值为空。</p>
    </td>
    </tr>
    <tr id="row59750658173211"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p62596825173211"><a name="p62596825173211"></a><a name="p62596825173211"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.5.1.2 "><p id="p32296167173211"><a name="p32296167173211"></a><a name="p32296167173211"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.5.1.3 "><p id="p5792332173211"><a name="p5792332173211"></a><a name="p5792332173211"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p8321575173211"><a name="p8321575173211"></a><a name="p8321575173211"></a>解析记录的值。不同类型解析记录对应的值的规则不同。</p>
    <p id="p813988173211"><a name="p813988173211"></a><a name="p813988173211"></a>如Type为AAAA类型，Value是域名对应的IPv6地址列表。</p>
    <p id="p59053902173211"><a name="p59053902173211"></a><a name="p59053902173211"></a>具体参见《云解析服务用户指南》中“<a href="https://support.huaweicloud.com/usermanual-dns/zh-cn_topic_0035467703.html" target="_blank" rel="noopener noreferrer">管理记录集</a>”章节提供的说明及请求样例。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    修改域名的记录集，域名的Zone ID为“2c9eb155587194ec01587224c9f90149”，Recordset ID为“2c9eb155587228570158722b6ac30007”。

    ```
    PUT https://{DNS_Endpoint}/v2/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587228570158722b6ac30007
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
            ]
        }
        ```

    -   CNAME类型

        ```
        {
            "name": "www.example.com.",
            "description": "This is an example record set.",
            "type": "CNAME",
            "ttl": 3600,
            "records": [
                "server1.example.com"
            ]
        }
        ```

    -   TXT类型

        ```
        {
            "name": "www.example.com.",
            "description": "This is an example record set.",
            "type": "TXT",
            "ttl": 300,
            "records": [
                "\"This host is used for sale.\""
            ]
        }
        ```

    -   NS类型

        ```
        {
            "name": "www.example.com.",
            "description": "This is an example record set.",
            "type": "NS",
            "ttl": 300,
            "records": [
                "node1.example.com.",
                "node2.example.com."
            ]
        }
        ```

    -   SRV类型

        ```
        {
            "name": "www.example.com.",
            "description": "This is an example record set.",
            "type": "SRV",
            "ttl": 3600,
            "records": [
                "3 60 2176 sipserver.example.com.",
                "10 100 2176 sipserver.example.com."
            ]
        }
        ```

    -   PTR类型

        ```
        {
            "name": "www.example.com.",
            "description": "This is an example record set.",
            "type": "PTR",
            "ttl": 3600,
            "records": [
                "host.example.com."
        
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
            ]
        }
        ```



## 响应<a name="section40090803161031"></a>

-   参数说明

    **表 3**  响应样例的参数说明

    <a name="table44131970191032"></a>
    <table><thead align="left"><tr id="rf63e3f73474e4c278a069c18f2cbda2e"><th class="cellrowborder" valign="top" width="18.23%" id="mcps1.2.4.1.1"><p id="a6ef51227cb264b32bebfc986d3e637d9"><a name="a6ef51227cb264b32bebfc986d3e637d9"></a><a name="a6ef51227cb264b32bebfc986d3e637d9"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.57%" id="mcps1.2.4.1.2"><p id="ae4f0a65aa76a4fb1957074bb69d5dbdd"><a name="ae4f0a65aa76a4fb1957074bb69d5dbdd"></a><a name="ae4f0a65aa76a4fb1957074bb69d5dbdd"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.2%" id="mcps1.2.4.1.3"><p id="a47bf2f8c9f504cc9bee2e5ec1257eb3f"><a name="a47bf2f8c9f504cc9bee2e5ec1257eb3f"></a><a name="a47bf2f8c9f504cc9bee2e5ec1257eb3f"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="rc4ac2a5267624f239ad9b1cd01768435"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="aed4e16cb934a49af80a35a677f91d92e"><a name="aed4e16cb934a49af80a35a677f91d92e"></a><a name="aed4e16cb934a49af80a35a677f91d92e"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.57%" headers="mcps1.2.4.1.2 "><p id="a5fe96ba32d0f47149f32f3ea7d4f05e6"><a name="a5fe96ba32d0f47149f32f3ea7d4f05e6"></a><a name="a5fe96ba32d0f47149f32f3ea7d4f05e6"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="a0b0a5c0cd1f24b55a29ecdb6066b3705"><a name="a0b0a5c0cd1f24b55a29ecdb6066b3705"></a><a name="a0b0a5c0cd1f24b55a29ecdb6066b3705"></a>Record Set的ID。</p>
    </td>
    </tr>
    <tr id="ra9e885d12b4d43428831752336a0d4c0"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="a32fb714b039b4a978222179f61a0f076"><a name="a32fb714b039b4a978222179f61a0f076"></a><a name="a32fb714b039b4a978222179f61a0f076"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.57%" headers="mcps1.2.4.1.2 "><p id="a83b8bc6a22eb48f087f3b842f1a177be"><a name="a83b8bc6a22eb48f087f3b842f1a177be"></a><a name="a83b8bc6a22eb48f087f3b842f1a177be"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="a3a0582b25e7f4c9c9028a0a082553e63"><a name="a3a0582b25e7f4c9c9028a0a082553e63"></a><a name="a3a0582b25e7f4c9c9028a0a082553e63"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="r8a5cb7251c6e4ad2aac8e92c1fc1c825"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="a2ba0b3a7490e4f8c9f2d001abc31b5fc"><a name="a2ba0b3a7490e4f8c9f2d001abc31b5fc"></a><a name="a2ba0b3a7490e4f8c9f2d001abc31b5fc"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.57%" headers="mcps1.2.4.1.2 "><p id="a590b27e6f7304033beb416c2615febf4"><a name="a590b27e6f7304033beb416c2615febf4"></a><a name="a590b27e6f7304033beb416c2615febf4"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="a6566187b31744bdfbfd273d05ada45cc"><a name="a6566187b31744bdfbfd273d05ada45cc"></a><a name="a6566187b31744bdfbfd273d05ada45cc"></a>Record Set的描述信息。</p>
    </td>
    </tr>
    <tr id="r6ff9dc233cc64b6eb856a2f2d4ecdfea"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="adb2e4a3dc5264bd194c9fdbb52d738f0"><a name="adb2e4a3dc5264bd194c9fdbb52d738f0"></a><a name="adb2e4a3dc5264bd194c9fdbb52d738f0"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.57%" headers="mcps1.2.4.1.2 "><p id="a9a32df9951ea4e63a36979ffe7839125"><a name="a9a32df9951ea4e63a36979ffe7839125"></a><a name="a9a32df9951ea4e63a36979ffe7839125"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="a69a040838e314d9992462ec5cb23db6f"><a name="a69a040838e314d9992462ec5cb23db6f"></a><a name="a69a040838e314d9992462ec5cb23db6f"></a>托管该记录的zone_id。</p>
    </td>
    </tr>
    <tr id="r82492d1a4b134373ba3e3fb657f19346"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="ade468dd7e4d24dc2bc83795202c2e618"><a name="ade468dd7e4d24dc2bc83795202c2e618"></a><a name="ade468dd7e4d24dc2bc83795202c2e618"></a>zone_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.57%" headers="mcps1.2.4.1.2 "><p id="ae9bad680780945638499d66748a089ee"><a name="ae9bad680780945638499d66748a089ee"></a><a name="ae9bad680780945638499d66748a089ee"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="af6bb9568887946fd83f837a9f67c9d35"><a name="af6bb9568887946fd83f837a9f67c9d35"></a><a name="af6bb9568887946fd83f837a9f67c9d35"></a>托管该记录的zone_name。</p>
    </td>
    </tr>
    <tr id="r58a2d0249a9d46608dceb58752487962"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="a6812a6c96d0b4f08ad96cd4aa92c29ef"><a name="a6812a6c96d0b4f08ad96cd4aa92c29ef"></a><a name="a6812a6c96d0b4f08ad96cd4aa92c29ef"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.57%" headers="mcps1.2.4.1.2 "><p id="a0cacd81f8e7247ed9b3e4b4a0d5a1c1a"><a name="a0cacd81f8e7247ed9b3e4b4a0d5a1c1a"></a><a name="a0cacd81f8e7247ed9b3e4b4a0d5a1c1a"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="a3db4aa6f5f604faeb111cc5b98a05bf9"><a name="a3db4aa6f5f604faeb111cc5b98a05bf9"></a><a name="a3db4aa6f5f604faeb111cc5b98a05bf9"></a>记录类型。</p>
    <p id="p941142431517"><a name="p941142431517"></a><a name="p941142431517"></a>取值范围：A、AAAA、MX、CNAME、TXT、NS（仅限公网Zone）、SRV、PTR（仅限内网Zone）、CAA（仅限公网Zone）。</p>
    <p id="zh-cn_topic_0037134404_p15442435577"><a name="zh-cn_topic_0037134404_p15442435577"></a><a name="zh-cn_topic_0037134404_p15442435577"></a>详细信息请参见<a href="枚举类型.md#section1188113824413">解析记录类型</a>。</p>
    </td>
    </tr>
    <tr id="r06be1132e6b544eaac47c6b6cae4af1d"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="abe5c52a6e2154f6391976aa80857198f"><a name="abe5c52a6e2154f6391976aa80857198f"></a><a name="abe5c52a6e2154f6391976aa80857198f"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.57%" headers="mcps1.2.4.1.2 "><p id="a57fe1965995b4f99a67c1c84d927f3b6"><a name="a57fe1965995b4f99a67c1c84d927f3b6"></a><a name="a57fe1965995b4f99a67c1c84d927f3b6"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="p7539104316419"><a name="p7539104316419"></a><a name="p7539104316419"></a>解析记录在本地DNS服务器的缓存时间，缓存时间越长更新生效越慢，以秒为单位。</p>
    <p id="p11539174314415"><a name="p11539174314415"></a><a name="p11539174314415"></a>如果您的服务地址经常更换，建议TTL值设置相对小些，反之，建议设置相对大些。</p>
    <p id="p1042612588514"><a name="p1042612588514"></a><a name="p1042612588514"></a>取值范围：</p>
    <a name="ul1526514741611"></a><a name="ul1526514741611"></a><ul id="ul1526514741611"><li>公网解析：1~2147483647。</li><li>内网解析：300~2147483647。</li></ul>
    <p id="p10651531171611"><a name="p10651531171611"></a><a name="p10651531171611"></a>默认值为300s。</p>
    </td>
    </tr>
    <tr id="r8cb1518cb4b84bf0b8115a7f4a8835c4"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="ae57bbd14742845c2aced32f030bc6a80"><a name="ae57bbd14742845c2aced32f030bc6a80"></a><a name="ae57bbd14742845c2aced32f030bc6a80"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.57%" headers="mcps1.2.4.1.2 "><p id="a5a480487a4fc42fa987d5ba2c6d920b9"><a name="a5a480487a4fc42fa987d5ba2c6d920b9"></a><a name="a5a480487a4fc42fa987d5ba2c6d920b9"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="a7ff6973b19f84ee5aa83b0967e0c2434"><a name="a7ff6973b19f84ee5aa83b0967e0c2434"></a><a name="a7ff6973b19f84ee5aa83b0967e0c2434"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="r93b32291d1e64da39452a8997fcda248"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="a9bc903f33fd54c9aa3b1f9d07ed6a31a"><a name="a9bc903f33fd54c9aa3b1f9d07ed6a31a"></a><a name="a9bc903f33fd54c9aa3b1f9d07ed6a31a"></a>create_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.57%" headers="mcps1.2.4.1.2 "><p id="a55f1491f864c456eae0b254526eaf1f8"><a name="a55f1491f864c456eae0b254526eaf1f8"></a><a name="a55f1491f864c456eae0b254526eaf1f8"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="ab802d00a14d74a5abe323755a0c1a9c3"><a name="ab802d00a14d74a5abe323755a0c1a9c3"></a><a name="ab802d00a14d74a5abe323755a0c1a9c3"></a>创建时间。</p>
    <p id="zh-cn_topic_0037134404_p91253279589"><a name="zh-cn_topic_0037134404_p91253279589"></a><a name="zh-cn_topic_0037134404_p91253279589"></a>格式：yyyy-MM-dd'T'HH:mm:ss.SSS</p>
    </td>
    </tr>
    <tr id="rececad4599034fec9010552d92c3b3d1"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="ae3d53158cf0e4b0c81f9aeafbbf377a2"><a name="ae3d53158cf0e4b0c81f9aeafbbf377a2"></a><a name="ae3d53158cf0e4b0c81f9aeafbbf377a2"></a>update_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.57%" headers="mcps1.2.4.1.2 "><p id="a1b01ca3627dc49c986c67d231de5c85f"><a name="a1b01ca3627dc49c986c67d231de5c85f"></a><a name="a1b01ca3627dc49c986c67d231de5c85f"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="acbcc47bca305436b8fb99d10b0de8765"><a name="acbcc47bca305436b8fb99d10b0de8765"></a><a name="acbcc47bca305436b8fb99d10b0de8765"></a>更新时间。</p>
    <p id="ab3462c7056cd417e81ff267a3ea46443"><a name="ab3462c7056cd417e81ff267a3ea46443"></a><a name="ab3462c7056cd417e81ff267a3ea46443"></a>格式：yyyy-MM-dd'T'HH:mm:ss.SSS</p>
    </td>
    </tr>
    <tr id="r18fd03e795cb427a953b0efb798cdc64"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="afe9aea31aae443be91d0a1ea8db8806d"><a name="afe9aea31aae443be91d0a1ea8db8806d"></a><a name="afe9aea31aae443be91d0a1ea8db8806d"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.57%" headers="mcps1.2.4.1.2 "><p id="a7f0d877c3b134d3bbaaa813571ef16fb"><a name="a7f0d877c3b134d3bbaaa813571ef16fb"></a><a name="a7f0d877c3b134d3bbaaa813571ef16fb"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="a9a68c20d53b843ed98875ccfce9781f4"><a name="a9a68c20d53b843ed98875ccfce9781f4"></a><a name="a9a68c20d53b843ed98875ccfce9781f4"></a>资源状态。</p>
    <p id="a6083e4f4301a476da8c39b9587e46bb9"><a name="a6083e4f4301a476da8c39b9587e46bb9"></a><a name="a6083e4f4301a476da8c39b9587e46bb9"></a>详细信息请参见<a href="枚举类型.md#section33673592114748">资源状态</a>。</p>
    </td>
    </tr>
    <tr id="rf566452075b04b41ac618d76387832ab"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="aad28018162974cd3ab00f6e7b50a0d40"><a name="aad28018162974cd3ab00f6e7b50a0d40"></a><a name="aad28018162974cd3ab00f6e7b50a0d40"></a>default</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.57%" headers="mcps1.2.4.1.2 "><p id="a4d66625c999244ffa5a6dcfa967cc6d2"><a name="a4d66625c999244ffa5a6dcfa967cc6d2"></a><a name="a4d66625c999244ffa5a6dcfa967cc6d2"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="aa87419f5ec904492968127f0424e88dd"><a name="aa87419f5ec904492968127f0424e88dd"></a><a name="aa87419f5ec904492968127f0424e88dd"></a>标识是否由系统默认生成，系统默认生成的Record Set不能删除。</p>
    </td>
    </tr>
    <tr id="r327b7fd09445440cb72ab3cd7fd54f76"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="a4b770fd18dd948aea76499724a625eca"><a name="a4b770fd18dd948aea76499724a625eca"></a><a name="a4b770fd18dd948aea76499724a625eca"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.57%" headers="mcps1.2.4.1.2 "><p id="a319fefa4c28b48ee9c5918b78a8746d8"><a name="a319fefa4c28b48ee9c5918b78a8746d8"></a><a name="a319fefa4c28b48ee9c5918b78a8746d8"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="p4619625201026"><a name="p4619625201026"></a><a name="p4619625201026"></a>该Record Set所属的项目ID。</p>
    </td>
    </tr>
    <tr id="r63b97c55056a4b32a3895d2af40c74a0"><td class="cellrowborder" valign="top" width="18.23%" headers="mcps1.2.4.1.1 "><p id="a94878242f50449aaae37b65105b3d867"><a name="a94878242f50449aaae37b65105b3d867"></a><a name="a94878242f50449aaae37b65105b3d867"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.57%" headers="mcps1.2.4.1.2 "><p id="af62c9f365b1f4d9b8743da27e6085818"><a name="af62c9f365b1f4d9b8743da27e6085818"></a><a name="af62c9f365b1f4d9b8743da27e6085818"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.2%" headers="mcps1.2.4.1.3 "><p id="ad757db1edea54d3cacac51db1def8abf"><a name="ad757db1edea54d3cacac51db1def8abf"></a><a name="ad757db1edea54d3cacac51db1def8abf"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
    <p id="p1230417511478"><a name="p1230417511478"></a><a name="p1230417511478"></a>详细信息请参见<a href="#table354521744216">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  links参数说明

    <a name="table354521744216"></a>
    <table><thead align="left"><tr id="row954518179427"><th class="cellrowborder" valign="top" width="18.3018301830183%" id="mcps1.2.4.1.1"><p id="p654513173424"><a name="p654513173424"></a><a name="p654513173424"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.591959195919593%" id="mcps1.2.4.1.2"><p id="p654551714212"><a name="p654551714212"></a><a name="p654551714212"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.10621062106211%" id="mcps1.2.4.1.3"><p id="p1545141717427"><a name="p1545141717427"></a><a name="p1545141717427"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3545101710429"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p115467171428"><a name="p115467171428"></a><a name="p115467171428"></a>self</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.591959195919593%" headers="mcps1.2.4.1.2 "><p id="p254611713427"><a name="p254611713427"></a><a name="p254611713427"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.10621062106211%" headers="mcps1.2.4.1.3 "><p id="p5546171744214"><a name="p5546171744214"></a><a name="p5546171744214"></a>当前资源的链接。</p>
    </td>
    </tr>
    <tr id="row125151707508"><td class="cellrowborder" valign="top" width="18.3018301830183%" headers="mcps1.2.4.1.1 "><p id="p136561245153620"><a name="p136561245153620"></a><a name="p136561245153620"></a>next</p>
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
        "ttl": 3600,
        "records": [
            "192.168.10.1",
            "192.168.10.2"
        ],
        "status": "PENDING_UPDATE",
        "links": {
            "self": "https://Endpoint/v2/zones/2c9eb155587194ec01587224c9f90149/recordsets/2c9eb155587228570158722b6ac30007"
        },
        "zone_id": "2c9eb155587194ec01587224c9f90149",
        "zone_name": "example.com.",
        "create_at": "2016-11-17T12:03:17.827",
        "update_at": "2016-11-17T12:56:03.827",
        "default": false,
        "project_id": "e55c6f3dc4e34c9f86353b664ae0e70c"
    }
    ```


## 返回值<a name="section9249181042119"></a>

接口正常的返回值为2xx，例如200、202或者204。

返回值含义以及更多返回值请参考[状态码](状态码.md)。

