1.项目简介
  (1)模拟当当网主要的功能
  (2)主要包含以下功能模块
     a.产品浏览模块 main
     b.购物车模块 cart
     c.用户管理模块 user
     d.创建订单模块 order
  (3)主要采用哪些技术
     a.Struts2框架
     b.JDBC+dbcp连接池
            连接池好处:
        1.避免频繁创建和销毁connection
     	2.将connection控制在一定数量范围内
     	    保证服务器稳定.
     c.客户端采用jQuery+Ajax
   (4)数据库设计(可以使用PowerDesign工具)
      a. d_user表
                存储用户注册的信息.
      b. d_receive_address表
                存储用户使用过的收货地址.
      c. d_category表
                存储产品类别信息
      d. d_product表
                存储各种类型产品的共有信息
      e. d_book表
                 存储图书产品的特有信息
      f. d_category_product表
                 存储类别和产品之间的包含关系
      g. d_order表
                存储订单信息表.
      h. d_item表
                存储订单明细表.
2.工程结构
   表现层 : JSP页面 涉及标签,OGNL表达式,jQuery,Ajax
   控制层 : 使用Struts2控制器,涉及struts.xml配置
   业务层 : Action组件
   数据访问层 : DAO组件
  src源码包结构如下:
  com.tarena.dang.action
  com.tarena.dang.action.user 用户模块Action
  com.tarena.dang.action.order 订单模块Action
  com.tarena.dang.action.main 产品浏览模块Action
  com.tarena.dang.action.cart 购物车Action
  com.tarena.dang.dao  接口
  com.tarena.dang.dao.impl 实现类
  com.tarena.dang.entity 实体类
  com.tarena.dang.util 工具类
  com.tarena.dang.interceptor 拦截器
  Struts配置文件结构如下:
     struts.xml(主配置)
        --struts-main.xml(产品浏览模块配置)
        --struts-order.xml(订单模块配置)
        --struts-user.xml(用户管理模块配置)
        --struts-cart.xml(购物车模块配置)
  WebRoot目录结构如下:
   /WebRoot/main/ 产品浏览JSP目录
   /WebRoot/cart/ 购物车JSP目录
   /WebRoot/order/ 订单JSP目录
   /WebRoot/user/  用户管理JSP目录
   /WebRoot/common/ 页眉页脚目录
   /WebRoot/css/  样式文件目录
   /WebRoot/js/   脚本文件目录
   /WebRoot/images/ JSP中图片目录
   /WebRoot/productImages/ 产品图片目录
  
  
  http://localhost:8080/dang/user/login.action
  
   
   



   
   
   
     
     
     
     
     
     
     
     