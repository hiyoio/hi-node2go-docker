# 说明 （部署前请仔细阅读完）
* 此分支更适合容器使用
* 
* PaaS 平台设置的环境变量
  | 变量名        | 是否必须 | 默认值 | 备注 |
  | ------------ | ------ | ------ | ------ |
  | PORT         | 否 |  3000  |http服务监听端口，也是订阅端口     |
  | ARGO_PORT    | 否 |  8080  |argo隧道端口，固定隧道token需和cloudflare后台设置的一致|
  | UUID         | 否 | 89c13786-25aa-4520-b2e7-12cd60fb5202|UUID|
  | NEZHA_SERVER | 否 |        | 哪吒服务端域名，例如nz.aaa.com    |
  | NEZHA_PORT   | 否 |  5555  | 哪吒端口为{443,8443,2096,2087,2083,2053}其中之一时，开启tls|
  | NEZHA_KEY    | 否 |        | 哪吒客务端专用KEY                |
  | ARGO_DOMAIN  | 否 |        | argo固定隧道域名                 |
  | ARGO_AUTH    | 否 |        | argo固定隧道json或token          |
  | CFIP         | 否 |na.ma   | 节点优选域名或ip                 |
  | CFPORT       | 否 |  443   |节点端口                          |
  | NAME         | 否 |  Vls   | 节点名称前缀，例如：Render，back4  |
  | FILE_PATH    | 否 |  tmp   | 运行目录,节点存放路径             | 

# 节点输出
* 输出log.txt节点文件，默认存放路径为tmp
* 订阅：分配的域名/log;例如https://www.google.com/log
* 非标端口订阅(游戏类):分配的域名:端口/log,前缀不是https，而是http，例如http://www.google.com:1234/log
  
# 免责声明
* 本程序仅供学习了解, 非盈利目的，请于下载后 24 小时内删除, 不得用作任何商业用途, 文字、数据及图片均有所属版权, 如转载须注明来源。
* 使用本程序必循遵守部署免责声明，使用本程序必循遵守部署服务器所在地、所在国家和用户所在国家的法律法规, 程序作者不对使用者任何不当行为负责。
