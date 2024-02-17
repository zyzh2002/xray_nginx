# xray_nginx

基于`docker compose`的`nginx`反向代理`xray`的`websocket`和`grpc`传输。经测试可以用于Cloudflare和AWS Cloudfront CDN。

你需要以下步骤以使他正确运行：
* 更改`config.json`中的UUID，websocket path和grpc servicename
* 同时更改`xray.conf`中的对应配置
* 将TLS证书放置于`./tls_certs`并参考`xray.conf`中的配置妥善命名