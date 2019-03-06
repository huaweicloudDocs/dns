# 修改Record Set<a name="ZH-CN_TOPIC_0077449085"></a>

## 功能介绍<a name="section49332166"></a>

修改单个Record Set。

## URI<a name="section41336317"></a>

PUT  /v2/zones/\{zone\_id\}/recordsets/\{recordset\_id\}

参数说明请参见[表1](#table52104579)。

**表 1**  URI格式的参数说明

<a name="table52104579"></a>
<table><thead align="left"><tr id="row50570707"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p2586631"><a name="p2586631"></a><a name="p2586631"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="22.24222422242224%" id="mcps1.2.4.1.2"><p id="p8190559"><a name="p8190559"></a><a name="p8190559"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="44.42444244424442%" id="mcps1.2.4.1.3"><p id="p59455556"><a name="p59455556"></a><a name="p59455556"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row51170717"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p51187411"><a name="p51187411"></a><a name="p51187411"></a>zone_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.24222422242224%" headers="mcps1.2.4.1.2 "><p id="p52539597"><a name="p52539597"></a><a name="p52539597"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="44.42444244424442%" headers="mcps1.2.4.1.3 "><p id="p27848947"><a name="p27848947"></a><a name="p27848947"></a>所属zone的ID。</p>
</td>
</tr>
<tr id="row49313939"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p35006119"><a name="p35006119"></a><a name="p35006119"></a>recordset_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.24222422242224%" headers="mcps1.2.4.1.2 "><p id="p16923420"><a name="p16923420"></a><a name="p16923420"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="44.42444244424442%" headers="mcps1.2.4.1.3 "><p id="p28619802"><a name="p28619802"></a><a name="p28619802"></a>待修改recordset的ID。</p>
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
    <tbody><tr id="row34337486173211"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p33154613173211"><a name="p33154613173211"></a><a name="p33154613173211"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.5.1.2 "><p id="p28540882173211"><a name="p28540882173211"></a><a name="p28540882173211"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.5.1.3 "><p id="p37402311173211"><a name="p37402311173211"></a><a name="p37402311173211"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p43441715173211"><a name="p43441715173211"></a><a name="p43441715173211"></a>可选配置，对域名的描述。</p>
    <p id="p9966775173211"><a name="p9966775173211"></a><a name="p9966775173211"></a>长度不超过255个字符。</p>
    </td>
    </tr>
    <tr id="row44235645173211"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p56753577173211"><a name="p56753577173211"></a><a name="p56753577173211"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.5.1.2 "><p id="p44923213173211"><a name="p44923213173211"></a><a name="p44923213173211"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.5.1.3 "><p id="p45055368173211"><a name="p45055368173211"></a><a name="p45055368173211"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p41610046141952"><a name="p41610046141952"></a><a name="p41610046141952"></a>Record Set的有效缓存时间，以秒为单位。</p>
    <p id="p54818170173211"><a name="p54818170173211"></a><a name="p54818170173211"></a>默认值为300s。</p>
    <p id="p20437753173211"><a name="p20437753173211"></a><a name="p20437753173211"></a>取值范围：</p>
    <p id="p27764803173211"><a name="p27764803173211"></a><a name="p27764803173211"></a>300-2147483647。</p>
    </td>
    </tr>
    <tr id="row59750658173211"><td class="cellrowborder" valign="top" width="22.45%" headers="mcps1.2.5.1.1 "><p id="p62596825173211"><a name="p62596825173211"></a><a name="p62596825173211"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.29%" headers="mcps1.2.5.1.2 "><p id="p32296167173211"><a name="p32296167173211"></a><a name="p32296167173211"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.89%" headers="mcps1.2.5.1.3 "><p id="p5792332173211"><a name="p5792332173211"></a><a name="p5792332173211"></a>List&lt;string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.37%" headers="mcps1.2.5.1.4 "><p id="p8321575173211"><a name="p8321575173211"></a><a name="p8321575173211"></a>不同Type对应的Value值规则不同。</p>
    <p id="p813988173211"><a name="p813988173211"></a><a name="p813988173211"></a>如Type为AAAA类型，Value是域名对应的IPv6地址列表。</p>
    <p id="p59053902173211"><a name="p59053902173211"></a><a name="p59053902173211"></a>具体参见《云解析服务用户指南》中“管理记录集”章节提供的说明及请求样例。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例
    -   A类型

        ```
        {
            "description": "This is an example record set.",
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
            "description": "This is an example record set.",
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
            "description": "This is an example record set.",
            "ttl": 3600,
            "records": [
                "1 mail.example.com"
            ]
        }
        ```

    -   CNAME类型

        ```
        {
            "description": "This is an example record set.",
            "ttl": 3600,
            "records": [
                "server1.example.com"
            ]
        }
        ```

    -   TXT类型

        ```
        {
            "description": "This is an example record set.",
            "ttl": 300,
            "records": [
                "\"This host is used for sale.\""
            ]
        }
        ```

    -   NS类型

        ```
        {
            "description": "This is an example record set.",
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
            "description": "This is an example record set.",
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
            "description": "This is an example record set.",
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
    <table><thead align="left"><tr id="zh-cn_topic_0037134404_row52466955175323"><th class="cellrowborder" valign="top" width="27.889999999999997%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0037134404_p2769858175323"><a name="zh-cn_topic_0037134404_p2769858175323"></a><a name="zh-cn_topic_0037134404_p2769858175323"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0037134404_p46296309175323"><a name="zh-cn_topic_0037134404_p46296309175323"></a><a name="zh-cn_topic_0037134404_p46296309175323"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.3%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0037134404_p62697904175323"><a name="zh-cn_topic_0037134404_p62697904175323"></a><a name="zh-cn_topic_0037134404_p62697904175323"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0037134404_row47909891175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p64112397175323"><a name="zh-cn_topic_0037134404_p64112397175323"></a><a name="zh-cn_topic_0037134404_p64112397175323"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p1660870175323"><a name="zh-cn_topic_0037134404_p1660870175323"></a><a name="zh-cn_topic_0037134404_p1660870175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p1249204175323"><a name="zh-cn_topic_0037134404_p1249204175323"></a><a name="zh-cn_topic_0037134404_p1249204175323"></a>Record Set的ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037134404_row6942422175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p64097412175323"><a name="zh-cn_topic_0037134404_p64097412175323"></a><a name="zh-cn_topic_0037134404_p64097412175323"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p44990515175323"><a name="zh-cn_topic_0037134404_p44990515175323"></a><a name="zh-cn_topic_0037134404_p44990515175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p32019574175323"><a name="zh-cn_topic_0037134404_p32019574175323"></a><a name="zh-cn_topic_0037134404_p32019574175323"></a>Record Set的名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037134404_row61442071175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p51194416175323"><a name="zh-cn_topic_0037134404_p51194416175323"></a><a name="zh-cn_topic_0037134404_p51194416175323"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p63301991175323"><a name="zh-cn_topic_0037134404_p63301991175323"></a><a name="zh-cn_topic_0037134404_p63301991175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p43966660175323"><a name="zh-cn_topic_0037134404_p43966660175323"></a><a name="zh-cn_topic_0037134404_p43966660175323"></a>Record Set的描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037134404_row2176746175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p11805366175323"><a name="zh-cn_topic_0037134404_p11805366175323"></a><a name="zh-cn_topic_0037134404_p11805366175323"></a>zone_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p1051908175323"><a name="zh-cn_topic_0037134404_p1051908175323"></a><a name="zh-cn_topic_0037134404_p1051908175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p10043845175323"><a name="zh-cn_topic_0037134404_p10043845175323"></a><a name="zh-cn_topic_0037134404_p10043845175323"></a>托管该记录的zone_id。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037134404_row61212722175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p8318586175323"><a name="zh-cn_topic_0037134404_p8318586175323"></a><a name="zh-cn_topic_0037134404_p8318586175323"></a>zone_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p31287919175323"><a name="zh-cn_topic_0037134404_p31287919175323"></a><a name="zh-cn_topic_0037134404_p31287919175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p16372315175323"><a name="zh-cn_topic_0037134404_p16372315175323"></a><a name="zh-cn_topic_0037134404_p16372315175323"></a>托管该记录的zone_name。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037134404_row38132372175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p37461920175323"><a name="zh-cn_topic_0037134404_p37461920175323"></a><a name="zh-cn_topic_0037134404_p37461920175323"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p27536075175323"><a name="zh-cn_topic_0037134404_p27536075175323"></a><a name="zh-cn_topic_0037134404_p27536075175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p24813356175323"><a name="zh-cn_topic_0037134404_p24813356175323"></a><a name="zh-cn_topic_0037134404_p24813356175323"></a>记录类型。</p>
    <p id="zh-cn_topic_0037134404_p173531225174112"><a name="zh-cn_topic_0037134404_p173531225174112"></a><a name="zh-cn_topic_0037134404_p173531225174112"></a>取值范围：A，AAAA，MX，CNAME，TXT，NS（仅限公网Zone），SRV，PTR（仅限内网Zone），CAA（仅限公网Zone）。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037134404_row20796819175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p4811553175323"><a name="zh-cn_topic_0037134404_p4811553175323"></a><a name="zh-cn_topic_0037134404_p4811553175323"></a>ttl</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p47559731175323"><a name="zh-cn_topic_0037134404_p47559731175323"></a><a name="zh-cn_topic_0037134404_p47559731175323"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p22097398175323"><a name="zh-cn_topic_0037134404_p22097398175323"></a><a name="zh-cn_topic_0037134404_p22097398175323"></a>域名的缓存时间，单位为秒，缓存时间越长更新生效越慢。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037134404_row13978060175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p43388342175323"><a name="zh-cn_topic_0037134404_p43388342175323"></a><a name="zh-cn_topic_0037134404_p43388342175323"></a>records</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p29596719175323"><a name="zh-cn_topic_0037134404_p29596719175323"></a><a name="zh-cn_topic_0037134404_p29596719175323"></a>List&lt;string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p30492925175323"><a name="zh-cn_topic_0037134404_p30492925175323"></a><a name="zh-cn_topic_0037134404_p30492925175323"></a>域名解析后的值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037134404_row23148559175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p36524189175323"><a name="zh-cn_topic_0037134404_p36524189175323"></a><a name="zh-cn_topic_0037134404_p36524189175323"></a>create_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p47080972175323"><a name="zh-cn_topic_0037134404_p47080972175323"></a><a name="zh-cn_topic_0037134404_p47080972175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p15737135175323"><a name="zh-cn_topic_0037134404_p15737135175323"></a><a name="zh-cn_topic_0037134404_p15737135175323"></a>创建时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037134404_row33465792175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p42570937175323"><a name="zh-cn_topic_0037134404_p42570937175323"></a><a name="zh-cn_topic_0037134404_p42570937175323"></a>update_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p27449776175323"><a name="zh-cn_topic_0037134404_p27449776175323"></a><a name="zh-cn_topic_0037134404_p27449776175323"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p63703533175323"><a name="zh-cn_topic_0037134404_p63703533175323"></a><a name="zh-cn_topic_0037134404_p63703533175323"></a>更新时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037134404_row17850883175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p36228271175323"><a name="zh-cn_topic_0037134404_p36228271175323"></a><a name="zh-cn_topic_0037134404_p36228271175323"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p6480061175323"><a name="zh-cn_topic_0037134404_p6480061175323"></a><a name="zh-cn_topic_0037134404_p6480061175323"></a>enum</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p65781854175323"><a name="zh-cn_topic_0037134404_p65781854175323"></a><a name="zh-cn_topic_0037134404_p65781854175323"></a>资源状态。</p>
    <p id="zh-cn_topic_0037134404_p51374523175323"><a name="zh-cn_topic_0037134404_p51374523175323"></a><a name="zh-cn_topic_0037134404_p51374523175323"></a>取值范围：PENDING_CREATE，ACTIVE，PENDING_DELETE，PENDING_UPDATE，ERROR。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037134404_row61184424175323"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p49633411175323"><a name="zh-cn_topic_0037134404_p49633411175323"></a><a name="zh-cn_topic_0037134404_p49633411175323"></a>default</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p56048766175323"><a name="zh-cn_topic_0037134404_p56048766175323"></a><a name="zh-cn_topic_0037134404_p56048766175323"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p37768157175323"><a name="zh-cn_topic_0037134404_p37768157175323"></a><a name="zh-cn_topic_0037134404_p37768157175323"></a>标识是否由系统默认生成，系统默认生成的Record Set不能删除与修改。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037134404_row15199048201026"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p23163408201026"><a name="zh-cn_topic_0037134404_p23163408201026"></a><a name="zh-cn_topic_0037134404_p23163408201026"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p40653752201026"><a name="zh-cn_topic_0037134404_p40653752201026"></a><a name="zh-cn_topic_0037134404_p40653752201026"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p4619625201026"><a name="zh-cn_topic_0037134404_p4619625201026"></a><a name="zh-cn_topic_0037134404_p4619625201026"></a>该Record Set所属的租户ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0037134404_row3965248419366"><td class="cellrowborder" valign="top" width="27.889999999999997%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0037134404_p2132803819366"><a name="zh-cn_topic_0037134404_p2132803819366"></a><a name="zh-cn_topic_0037134404_p2132803819366"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0037134404_p1127763319366"><a name="zh-cn_topic_0037134404_p1127763319366"></a><a name="zh-cn_topic_0037134404_p1127763319366"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.3%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0037134404_p4107308719366"><a name="zh-cn_topic_0037134404_p4107308719366"></a><a name="zh-cn_topic_0037134404_p4107308719366"></a>指向当前资源或者其他资源的链接。当查询需要分页时，需要包含一个next链接指向下一页。</p>
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


## 返回值<a name="section42637797161043"></a>

请参考[通用请求返回值](通用请求返回值.md)。

