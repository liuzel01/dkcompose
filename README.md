## 使用说明

> 项目上、运维支撑组等用到的，各组件的docker-compose 配置，供参考

---
**<font>各目录快捷跳转：</font>**

- [frp](./dkcompose/frp/)

- [gitlab](./dkcompose/gitlab/)

- [jenkins](./dkcompose/jenkins/)

- [minio](./dkcompose/minio/)

- [kuboard](./dkcompose/kuboard/)

- [lanproxy](./dkcompose/lanproxy/)

- [nexus](./dkcompose/nexus/)

- [onlyoffice](./dkcompose/onlyoffice/)

### onlyoffice

- onlyoffice 主要是配合 confluence，实现在线预览、编辑文档

    `git clone https://github.com/ONLYOFFICE/Docker-DocumentServer.git`

- 对目录下的 docker-compose.yml 文件进行修改，或直接启动（本仓库内只有修改后的docker-compose.yml ）

- 启动成功后，在 confluence -“站点管理”进行配置，

    "Document Editing Service address": <http://172.16.2.123/>

    "Secret key (leave blank to disable)": wjjxw0pBvrOLxJUUEtNr  (这个是根据 local.json 文件中的配置获取的)
