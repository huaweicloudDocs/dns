# SOA记录中的Email格式为什么变化了？<a name="dns_faq_009"></a>

用户在创建域名时输入的Email，是域名管理员的邮箱，用于接收该域名的错误信息和问题报告。您可以使用常用的邮箱地址作为管理员邮箱，但是，RFC 2142强烈建议您优先使用保留邮箱“HOSTMASTER@_域名”_  作为该域名的管理员邮箱。

域名创建完成后，Email信息会自动记录在该域名的SOA记录中。但是，由于“@”符号在SOA记录中有特殊的含义，因此邮箱地址中的“@”符号会被替换为“.”符号，同时，如果“@”符号前面有“.”符号，系统会自动使用转义字符“\\”进行转换。更多详情，请参见RFC1035。

示例：

以“test.hostmaster@example.com”为例。假设用户在创建域名时输入的Email为“test.hostmaster@example.com”，那么，域名创建完成后，SOA记录中呈现的Email为“test\\.hostmaster.example.com”。

