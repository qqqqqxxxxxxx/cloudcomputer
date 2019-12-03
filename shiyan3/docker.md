### Centos 7安装Docker

下载docker

![](../shiyan3/IMG/1.png)

![](../shiyan3/IMG/2.png)



查询docker版本

![](../shiyan3/IMG/4.png)

测试是否成功

![](../shiyan3/IMG/5.png)

### Docker加载CentOS镜像

**拉取 Centos 7**

![](../shiyan3/IMG/6.png)

**拉取完毕后查看镜像**

![](../shiyan3/IMG/7.png)

**运行Docker容器

查看已启动的容器

![](../shiyan3/IMG/8.png)

**进入容器前台**

![](../shiyan3/IMG/9.png)

容器里安装Apache Web

![](../shiyan3/IMG/10.png)

安装完成后，启动Apache Web服务器，设置开机自启

![](..\shiyan3\IMG\11.png)

访问服务器公网IP,出现下图代表Apache安装成功

![](..\shiyan3\IMG\12.png)

**安装MariaDB**

![](..\shiyan3\IMG\13.png)

**启动MariaDB设置MySQL的root密码**

![](..\shiyan3\IMG\14.png)

**设置开机自启MariaDB**

![](..\shiyan3\IMG\15.png)

### 安装PHP



**因为WordPress需要php5.6以上版本的支持，我们更新到7.2版本仓库**

![](..\shiyan3\IMG\17.png)

**安装PHP以及php-mysql**

![](..\shiyan3\IMG\18.png)

**查看安装的php版本**

![](..\shiyan3\IMG\19.png)
为了更好的运行PHP，需要启动PHP附加模块

![](..\shiyan3\IMG\20.png)

### .安装WordPress以及完成相关配置

登陆数据库 给wordpress创建新的数据库

![](..\shiyan3\IMG\21.png)

**进入刚创建的数据库**为WordPress创建一个独立的MySQL用户并授权给数据库访问权限****

![](..\shiyan3\IMG\22.png)

**安装WordPress**

![](..\shiyan3\IMG\23.png)

![](..\shiyan3\IMG\24.png)

点击继续，填写先前创建的数据库名，用户名及密码

![](..\shiyan3\IMG\25.png)

### 推送带有wordpress的镜像

![](..\shiyan3\IMG\26.png)

上传至DOCKER HUB

![](..\shiyan3\IMG\27.png)

