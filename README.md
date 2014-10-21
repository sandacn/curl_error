1  => " [CURLE_UNSUPPORTED_PROTOCOL] libcurl不支持传入的URL。
        可能编译的时候对应的选项没有打开，也可能是协议拼写错误，或者是libcurl还不支持该协议",
2  => " [CURLE_FAILED_INIT] 初始化失败。
        可能是内部错误或者是未能在初始化阶段获取资源",
3  => " [CURLE_URL_MALFORMAT] URL格式不正确。",
4  => " [CURLE_NOT_BUILT_IN] 在程序build阶段libcurl没有内置对应协议或者选项。
        就是说在libcurl内置的时候，对应的特性或者选项并没有打开或者被显式关闭了，解决方案重新build一个libcurl",
5  => " [CURLE_COULDNT_RESOLVE_PROXY] 无法解析代理服务器。 
        指定的代理服务器主机无法解析。",
6  => " [CURLE_COULDNT_RESOLVE_HOST] 无法解析主机。 
        指定的远程主机无法解析。",
7  => " [CURLE_COULDNT_CONNECT] 无法连接（connect()）主机或代理服务器。",
8  => " [CURLE_FTP_WEIRD_SERVER_REPLY] 在连接到 FTP 服务器后，libcurl 需要收到特定的回复。
        此错误代码表示libcurl收到了不正常或不正确的回复。 指定的远程服务器可能不是正确的 FTP 服务器。",
9  => " [CURLE_REMOTE_ACCESS_DENIED] 访问给定的URL资源被拒绝。
        对于FTP，一般发生在尝试更改远程目录阶段",
10 => " [CURLE_FTP_ACCEPT_FAILED] 等待一个活跃的FTP会话的服务器连接返回，从控制通道返回了错误代码，或者类似的情形发生",
11  => " [CURLE_FTP_WEIRD_PASS_REPLY ] 在将 FTP 密码发送到服务器后，libcurl 未收到正常回复。 此错误代码表示返回的是意外的编码。",
12  => " [CURLE_FTP_ACCEPT_TIMEOUT] 在活跃的FTP会话中等待服务器来connect，CURLOPT_ACCEPTTIMOUT_MS(3)（或者是内部默认）超时过期",
13  => " [CURLE_FTP_WEIRD_PASV_REPLY] libcurl 发出 PASV 或 EPSV 命令之后，服务器返回一个不合理的结果。
        可以断定FTP服务器有问题。",
14  => " [CURLE_FTP_WEIRD_227_FORMAT] FTP 发出PASV命令之后， 服务器返回227行（227-line）。
        如果 libcurl 无法解析此行，就会返回此代码。",
15  => " [CURLE_FTP_CANT_GET_HOST] 在建立新连接中，查找主机时出现内部错误。",
16  => " [CURLE_HTTP2] 在HTTP2的帧层出现问题。
        这个报错有点一般性，有好几个原因会导致这个问题，具体的原因看错误缓冲区",
17  => " [CURLE_FTP_COULDNT_SET_TYPE] 在尝试将传输模式设置为二进制或 ascii 时发生错误。",
18  => " [CURLE_PARTIAL_FILE ] 文件传输大小小于或大于预期。
        一般发生在服务器先报告了一个预期的传输大小，客户端所传送的数据与先前指定尺寸不相符。",
19  => " [CURLE_FTP_COULDNT_RETR_FILE] 原因有两个：“RETR” 命令收到了不正常的回复，或完成的传输大小为零字节。",
21  => " [CURLE_QUOTE_ERROR] 在向远程服务器发送自定义的 “QUOTE” 命令时，其中一个命令返回的错误代码为 400 或更大的数字（对于 FTP），或者说明此命令没有成功。",
22  => " [CURLE_HTTP_RETURNED_ERROR] 如果 CURLOPT_FAILONERROR 设置为 TRUE，且 HTTP 服务器返回 >= 400 的错误代码，就会返回此代码。 （此错误代码以前又称为 CURLE_HTTP_NOT_FOUND。）",
23  => " [CURLE_WRITE_ERROR] 在向本地文件写入所收到的数据时发生错误，或由写入回调 (write callback) 向 libcurl 返回了一个错误。",
25  => " [CURLE_UPLOAD_FAILED] 在上传开始时失败。 对于 FTP，服务器一般是由于拒绝执行 STOR 命令。错误缓冲区通常会有更详细的说明。 （此错误代码以前又称为 CURLE_FTP_COULDNT_STOR_FILE。）",
26  => " [CURLE_READ_ERROR] 读取本地文件出现问题，或由读取回调 (read callback) 返回了一个错误。",
27  => " [CURLE_OUT_OF_MEMORY] 内存分配请求失败。
        此错误比较严重，因为如果发生此错误，则表明机器出现了非常严重的问题，否则怎么连内存都无法分配了呢？",
28  => " [CURLE_OPERATION_TIMEDOUT] 操作超时。 
        已达到设定的超时时间。",
30  => " [CURLE_FTP_PORT_FAILED] FTP PORT 命令返回错误。 
        在没有为 libcurl 指定适当的地址使用时，最有可能发生此问题。 请参阅 CURLOPT_FTPPORT。",
31  => " [CURLE_FTP_COULDNT_USE_REST] FTP REST 命令返回错误。
        如果服务器正常，应该永远不会发生这种情况。",
33  => " [CURLE_RANGE_ERROR] 服务器不支持或不接受范围请求。",
34  => " [CURLE_HTTP_POST_ERROR] 此问题比较诡异，主要由内部混乱引发。",
35  => " [CURLE_SSL_CONNECT_ERROR] 在SSL/TLS握手阶段的某个环节出现了问题。
        更详细的报错可以查看错误缓冲区。可能是证书（文件格式、路径、许可）、密码及其他因素导致了此问题。",
36  => " [CURLE_BAD_DOWNLOAD_RESUME] 由于给定的文件位置已经超过了文件大小导致文件无法继续下载。",
37  => " [CURLE_FILE_COULDNT_READ_FILE] 无法打开 FILE:// 路径下的文件。很可能是文件路径无法定位已有文件。建议你检查文件的访问权限。",
38  => " [CURLE_LDAP_CANNOT_BIND] LDAP 无法绑定。
        LDAP 绑定操作失败。",
39  => " [CURLE_LDAP_SEARCH_FAILED] LDAP 搜索失败。",
41  => " [CURLE_FUNCTION_NOT_FOUND] 找不到函数。 
        找不到必要的 zlib 函数。",
42  => " [CURLE_ABORTED_BY_CALLBACK] 由回调中止本次调用。 
        回调向 libcurl 返回了 “abort”。",
43  => " [CURLE_BAD_FUNCTION_ARGUMENT] 内部错误。 
        调用函数所用的参数是有问题的。",
45  => " [CURLE_INTERFACE_FAILED] 接口错误。 
        指定的外部接口无法使用。 请通过 CURLOPT_INTERFACE 设置要使用哪个接口来确定连接锁使用来源 IP 地址。 （此错误代码以前又称为 CURLE_HTTP_PORT_FAILED。）",
47  => " [CURLE_TOO_MANY_REDIRECTS] 重定向次数过多。 
        进行重定向时，libcurl 达到了上限。请使用 CURLOPT_MAXREDIRS 设置上限。",
48  => " [CURLE_UNKNOWN_OPTION] 给libcurl传入了无法识别或者未知的选项。 
        请参阅选项的相关文档。这个一般来说调用libcurl的程序导致的。具体出错的选项在错误缓冲区有更详细的信息",
49  => " [CURLE_TELNET_OPTION_SYNTAX] telnet 选项字符串的格式不正确。",
51  => " [CURLE_PEER_FAILED_VERIFICATION] 远程服务器的 SSL 证书或 SSH md5 指纹不正确。",
52  => " [CURLE_GOT_NOTHING] 服务器未返回任何数据，在这种情况下，未返回任何数据就认为是错误。",
53  => " [CURLE_SSL_ENGINE_NOTFOUND] 指定的加密引擎没找到。",
54  => " [CURLE_SSL_ENGINE_SETFAILED] 无法将选定的SSL引擎设置为默认值。",
55  => " [CURLE_SEND_ERROR] 无法发送网络数据。",
56  => " [CURLE_RECV_ERROR] 接收网络数据失败。",
58  => " [CURLE_SSL_CERTPROBLEM] 本地客户端证书有问题",
59  => " [CURLE_SSL_CIPHER] 无法使用指定的密钥",
60  => " [CURLE_SSL_CACERT] 无法使用已知的 CA 证书验证对等证书",
61  => " [CURLE_BAD_CONTENT_ENCODING] 无法识别传输编码",
62  => " [CURLE_LDAP_INVALID_URL] LDAP 链接无效",
63  => " [CURLE_FILESIZE_EXCEEDED] 超过了文件大小上限",
64  => " [CURLE_USE_SSL_FAILED] 请求的 FTP SSL 级别失败",
65  => " [CURLE_SEND_FAIL_REWIND] 进行发送操作时，curl 必须rewind以便重新传输，但rewind操作未能成功",
66  => " [CURLE_SSL_ENGINE_INITFAILED] SSL 引擎初始化失败",
67  => " [CURLE_LOGIN_DENIED] 远程服务器拒绝 curl 登录（7.13.1 新增功能）",
68  => " [CURLE_TFTP_NOTFOUND] 在 TFTP 服务器上找不到文件",
69  => " [CURLE_TFTP_PERM] 在 TFTP 服务器上遇到权限问题",
70  => " [CURLE_REMOTE_DISK_FULL] 服务器磁盘空间不足",
71  => " [CURLE_TFTP_ILLEGAL] TFTP 操作非法",
72  => " [CURLE_TFTP_UNKNOWNID] TFTP 传输 ID 未知",
73  => " [CURLE_REMOTE_FILE_EXISTS] 文件已存在，无法覆盖",
74  => " [CURLE_TFTP_NOSUCHUSER] 运行正常的 TFTP 服务器不会返回此错误",
75  => " [CURLE_CONV_FAILED] 字符转换失败",
76  => " [CURLE_CONV_REQD] 调用方必须注册转换回调",
77  => " [CURLE_SSL_CACERT_BADFILE] 读取 SSL CA 证书时遇到问题（可能是路径错误或访问权限问题）",
78  => " [CURLE_REMOTE_FILE_NOT_FOUND] 网址中引用的资源不存在",
79  => " [CURLE_SSH] SSH 会话中出现无法识别的错误",
80  => " [CURLE_SSL_SHUTDOWN_FAILED] 关闭 SSL 连接失败",
81  => " [CURLE_AGAIN] Socket还没有做好发送/接收数据准备，可以等它准备好了之后再重试。
        该返回码只有可能从curl_easy_recv 或者 curl_easy_send返回（7.18.2新增功能）",
82  => " [CURLE_SSL_CRL_BADFILE] 加载 CRL 文件失败（7.19.0新增功能）",
83  => " [CURLE_SSL_ISSUER_ERROR] 证书发出者验证失败",
84  => " [CURLE_FTP_PRET_FAILED] FTP 服务器无法理解 PRET 命令或者不支持给定参数。
        在使用 CURLOPT_CUSTOMREQUEST 的时候要注意： a custom LIST command will be sent with PRET CMD before PASV as well（7.20.0新增功能）",
85  => " [CURLE_RTSP_CSEQ_ERROR] RTSP CSeq 序号不匹配",
86  => " [CURLE_RTSP_SESSION_ERROR] RTSP 会话ID不匹配",
87  => " [CURLE_FTP_BAD_FILE_LIST] 无法解析FTP 文件列表（在 FTP 模糊下载中）",
88  => " [CURLE_CHUNK_FAILED] Chunk回调报错",
89  => " [CURLE_NO_CONNECTION_AVAILABLE] （仅供内部使用，libcurl外部不会出现）没有连接可用，该会话将会进入队列（7.30.0新增功能）",
