# hsweb 演示
演示如何在新项目中使用hsweb
基于[hsweb-framework](https://github.com/hs-web/hsweb-framework)和[hsweb-platform](https://github.com/hs-web/hsweb-platform) 

## 环境
运行唯一需要的环境: **java8**

## 运行
**直接运行**
```shell
    $ ./mvnw spring-boot:run    #linux
    $ mvnw.cmd spring-boot:run  #windows
```
**IDE**
导入ide后等待maven依赖下载完成后执行`org.hsweb.demo.Run`

## 目录说明
```shell
----------src/main/java
---------------org.hsweb.demo
--------------------bean,controller,dao,service #不做过多说明，都懂
--------------------Run.java                    #项目启动类,直接运行启动项目
----------resources
---------------config                           #配置目录(logback和mybatis配置文件)
---------------mappers                          #mybatis mapper配置文件
---------------scripts.initialize               #系统初始化脚本
---------------templates                        #模板文件(freemarker)
---------------static                           #静态文件目录
---------------application.yml                  #应用主配置,数据源啥的都在这里
```

## 访问
启动成功登录后,用浏览器打开 `http://localhost:8080/` 
帐号:admin 密码:admin
[上报问题](https://github.com/hs-web/hsweb-demo/issues/new)

# 注意
启动日志提示sigar-amd64-winnt.dll相关错误,这是系统监控需要的库,不引入不影响程序运行.
要使用系统监控功能,请自行将 sigar-amd64-winnt.dll 放入system32 目录或者libsigar-amd64-linux.so  /usr/lib 目录.
[下载地址](https://github.com/hs-web/hsweb-platform/blob/master/lib/sigar)



https://registry.aurora.tencent.com/packages/0/00/all/1785484743/tcs-precheck-core-2.3.5-version.tar.gz?version=v1&issueDate=2026-07-31T16%3A05%3A31%2B08%3A00&uuid=08fa25cf-c48d-4895-abda-06432e59829f&authorization=y7F9SiR33bZjltMdL4Xy6zMfYjUZJa42Axkj2QSixMSLEC3n%2FlLTjFzENIJbuh9quMvEQszYW7Wp6ZdaZe06wjazHydDHteZ7fAf8pndy5LUgkuEktdxzL22hJonur8fDITxCZ9QgUo5U3eoUBgT3JtpPew1MfLX%2B6RKHvSoV3PH8TTNY2xy4MvRutYq7tvJuUtefqJuRDF3i2onQ1vsvYIgoRpjHagnJonHEkJCKXagM%2FQsSU%2F6GFA6rYKSe8IPPzQGnzqxbeGrfiPfrFSLn1MK2spLc9VxRGvx%2F262%2BpDAbjGeUlu92Zmo8QznDNVS01Nvk1DT0bncG2rDPOB%2Bgg%3D%3D&privateKeyHash=WJesrCD%2Fha5pRdC7i080TRzCfaLxcCe5dmoX01KsU4s%3D
