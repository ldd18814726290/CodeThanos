# Dubbox

##  简介
    定义：分布式服务框架
    功能：service层与web层分离
    
##  原理
一、节点角色
Provider    服务提供方
Consumer    服务消费方
Register    服务注册中心
Monitor     服务监控中心
Container   服务存放容器

二、调用关系
长连接：1,2,3,4
短连接：0,5

    0.Container:启动、加载、运行Provider
    1.Provider：运行,Register注册服务
    2.Consumer：运行,Register订阅服务
    3.Register：返回地址列表,地址列表改变则推送Consumer
    4.Consumer：获取地址列表,调用Provider
    5.Monitor： Provider、Consumer-每分钟发送统计数据
##  代码实现

Provider:
            service.interface 
            service.implement  @Service
Consumer:   
            service.interface  copy
            controller  @Controller         spirng
                        @RequestMapping     spring       
                        @ResponseBody       spring
                        @Reference          dubbox    远程注入
##  说明
    