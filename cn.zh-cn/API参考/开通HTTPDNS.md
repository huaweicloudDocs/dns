# 开通HTTPDNS<a name="ZH-CN_TOPIC_0156607171"></a>

## 功能介绍<a name="zh-cn_topic_0124033543_section63355478"></a>

开通HTTPDNS。

## URI<a name="zh-cn_topic_0124033543_section33328392"></a>

POST /v1/httpdns

## 请求<a name="zh-cn_topic_0124033543_section31520075"></a>

无

## 响应<a name="zh-cn_topic_0124033543_section15245225"></a>

-   要素说明

    **表 1**  响应样例的要素说明

    <a name="zh-cn_topic_0124033543_table6255205892049"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0124033543_row1727035092049"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0124033543_p5672109992049"><a name="zh-cn_topic_0124033543_p5672109992049"></a><a name="zh-cn_topic_0124033543_p5672109992049"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.189999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0124033543_p3100628892049"><a name="zh-cn_topic_0124033543_p3100628892049"></a><a name="zh-cn_topic_0124033543_p3100628892049"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.629999999999995%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0124033543_p2848141492049"><a name="zh-cn_topic_0124033543_p2848141492049"></a><a name="zh-cn_topic_0124033543_p2848141492049"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0124033543_row2529320492049"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0124033543_p9950162792917"><a name="zh-cn_topic_0124033543_p9950162792917"></a><a name="zh-cn_topic_0124033543_p9950162792917"></a>account_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0124033543_p29501827182915"><a name="zh-cn_topic_0124033543_p29501827182915"></a><a name="zh-cn_topic_0124033543_p29501827182915"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0124033543_p195142782916"><a name="zh-cn_topic_0124033543_p195142782916"></a><a name="zh-cn_topic_0124033543_p195142782916"></a>账户ID，由系统生成。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0124033543_row1357301819290"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0124033543_p10952162718299"><a name="zh-cn_topic_0124033543_p10952162718299"></a><a name="zh-cn_topic_0124033543_p10952162718299"></a>sign_key</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.189999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0124033543_p595314278296"><a name="zh-cn_topic_0124033543_p595314278296"></a><a name="zh-cn_topic_0124033543_p595314278296"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.629999999999995%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0124033543_p1495312277298"><a name="zh-cn_topic_0124033543_p1495312277298"></a><a name="zh-cn_topic_0124033543_p1495312277298"></a>接入鉴权加密使用的key。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    { 
        "account_id": "12345678",
        "sign_key": "GGF9CL0E277E",
    }     
    ```


## 返回值<a name="zh-cn_topic_0124033543_section2989297"></a>

请参考[通用请求返回值](通用请求返回值.md)。

