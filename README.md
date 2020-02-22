# 说明

这个项目演示使用[云捷易](http://www.cloudedi.cn)开发的mule适配器，实现简单的EDI单据的收发功能

## 申请测试账号

拨打电话010-83201217或填写[在线申请表单](https://www.wenjuan.com/s/numYryU/)

## 下载开发环境

通过以下地址注册并下载开发环境：

```
https://www.mulesoft.com/lp/dl/studio
```

## 下载项目实例

克隆模板项目文件到本地：

```bash
git clone https://github.com/cloudedi/edi-as2-template
```

## 修改配置文件

pom.xml

```xml
<repository>
  <id>cloudedi</id>
  <name>cloudedi</name>
  <url>http://repo.yiduijie.cn:8081/repository/您的帐号/</url>
  <layout>default</layout>
</repository>
```

## 设置试用帐号

修改maven配置文件

```xml
<settings xmlns="http://maven.apache.org/SETTINGS/1.0.0"
      xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0
                          https://maven.apache.org/xsd/settings-1.0.0.xsd">
  ...
  <servers>
      ...
    <server>
        <id>cloudedi</id>
        <username>您的帐号</username>
        <password>您的密码</password>
    </server>
      ...
  </servers>
</settings>
```

## 在开发环境打开项目