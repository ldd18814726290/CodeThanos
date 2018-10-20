# AngularJS

##  Version 1.0
    一、四大特征
    1.MVC模式   通过DI来视图、数据、逻辑组件松耦合  Model,View,Controller
               [1]双向绑定：视图 -控制器
               [2]依赖注入：控制器-服务
    2.双向绑定   视图、数据双向更新     UI视图-数据模型
    3.依赖注入   Service、Controller
    4.模块设计   官方模块  ng、ngRoute、ngAnimate
               自定义模块 angular.module('moduleName',[])
##  代码
    引入      <script src="angular.min.js"></srcipt>
    表达式    <body ng-app>    {{ data }}
    双向绑定   <input ng-module>   
    初始化指令 <body ng-app ng-init=""> 
    
    控制器    script   app.controller
             body     ng-controller    
             input    ng-module
    事件指令   <> 
    循环数组
    循环对象数组
    内置服务    