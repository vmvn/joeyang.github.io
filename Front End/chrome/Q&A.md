# 问题解决与汇总

### 报错："CAUTION: Provisional headers are shown"

* 这个警告的意思是说：请求的资源可能会被（扩展／或其他什么机制）屏蔽掉。
* 之所以会出现这个警告，是因为去获取该资源的请求其实并（还）没有真的发生，所以 Header 里显示的是伪信息，直到服务器真的有响应返回，这里的 Header 信息才会被更新为真实的。不过这一切也可能不会发生，因为该请求可能会被屏蔽。比如说 AdBlock 什么的，当然了不全是浏览器扩展，具体情况具体分析了。