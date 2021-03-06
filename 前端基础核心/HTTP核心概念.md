# HTTP核心概念

## OSI模型



## 几种HTTP协议



## 请求方法



## HTTP状态码

##### 状态码的类别：

| 状态码 | 类别             | 原因                       |
| ------ | ---------------- | -------------------------- |
| 1XX    | 信息性状态码     | 接收的请求正在处理         |
| 2XX    | 成功状态码       | 请求正常处理完毕           |
| 3XX    | 重定向状态码     | 需要进行附加操作以完成请求 |
| 4XX    | 客户端错误状态码 | 服务器无法处理请求         |
| 5XX    | 服务端错误状态码 | 服务器处理请求出错         |

### 2XX成功状态码

* 200 OK

​      客户端发来的请求在服务器端被**正常**处理了。

* 204 No Content

​      请求成功，**资源无更新**，不刷新浏览器。

* 206 Partial Content

​      客户端进行了**范围请求**，而服务器成功执行了这部分的GET请求。

### 3XX重定向状态码

* 301 Moved Permanently

​      **永久性重定向**。

* 302 Found

​       **临时性重定向**，本次使用新的URI访问。

* 303 See Other

​       **临时性重定向**，使用**GET**方法请求资源。

* 304 Not Modified

​      当客户端发送附带条件的请求时，服务器端允许请求访问资源，但**未满足条件**的情况。

​      ***跟重定向没关系***。

* 307 Temporary Redirect

​      **临时重定向**。使用**POST**请求资源。

### 4XX客户端错误

* 400 Bad Request

​      **请求语法错误**。

* 401 Unauthorized

​       发送的请求**需要**有通过HTTP认证的**认证**信息。

* 403 Forbidden

​       访问**权限不够**，被服务器拒绝访问资源。

* 404 Not Found

​      **找不到资源**。

### 5XX服务器错误

* 500 Internal Server Error

​      服务器端在执行请求时**发生了错误**。

* 503 Service Unavailable

​      服务器暂时处于**超负载**或正在进行**停机维护**，现在**无法处理请求**。











