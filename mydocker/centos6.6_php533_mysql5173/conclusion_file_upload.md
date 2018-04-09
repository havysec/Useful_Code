# 文件上传漏洞

## 文件上传校验姿势

* 客户端javascript校验（一般只校验后缀名）
* 服务端校验
  * 文件头content-type字段校验（image/gif）
  * 文件内容头校验（GIF89a）
  * 后缀名黑名单校验
  * 后缀名白名单校验
  * 自定义正则校验
* WAF设备校验（根据不同的WAF产品而定）