# HTML学习笔记    

## 一.  初级知识

### 1.1 C/S架构:软件,在桌面上有图标.    

### 1.2 B/S架构:网页端  

C: client客户端  (安装 更新 不跨平台)--可承载大型,安全性要求高的应用

B:  browser浏览器(与C相反)--前端

S: server(服务器)--类似一个中转站   

### 2.浏览器相关知识  

### 2.1.浏览器的内核是什么?  

浏览器核心,用于处理浏览器的各种资源

webkit   blink   trident   gecko  (四大内核)  

### 3.网页  

  ### 3.1组成    

html:结构(骨架)

css:表现(皮肤)

js:交互  



## 二.HTML标准结构  

### 1.html是什么?    

1.0.1 **历史** :W3C正式发布--Adobe Flash Player(音 影&游戏)--HTML5(2014年)  

1.0.2 **准备工作**   

	* 查看扩展名(后缀) 的步骤:查看-显示-文件扩展名    
	* 打开方式的更改:

1.1初体验  

 * 新建文本文档-改后缀(.html)  

 * 在记事本改源代码--浏览器渲染(出页面)    --后续用VScode

   ```<marquee>雅锶HTML初体验!!</marquee>  ```     

   * 起始标签-标签体-结束标签</标签名>  
   
   * <input>单独存在:单标签
   
   * <input/>自结束
   
   * 标签可嵌套--!此时要换行,缩进
   
     

1.2标签属性  --可以有多个属性,但不能重复--不在乎大小写* 

	* <marquee loop="1">--表示让标签体循环一次
	* loop(每个属性名)前有一个英文空格
	*  loop="1"---属性

 * loop---属性名
 * 1---属性值(>=1)

* type="passward"(不让看input内容)

* bgcolor(背景色)

* disabled(禁用)

* type="text"(正常输入文本)---如果重复则只看第一个写的  

  

1.3基本结构   

* 浏览器在渲染前会进行 HTML格式检查   

* 基本结构  

  ```<html> 
  	<html>
  	<head></head>
  	<body>  
  		<marquee>我是标签体</marquee>  
  	</body>  
  	</html>  
  ```

  * 改页签名  

    <head>  
        <title>吴雅锶的网页</title>
    </head>

* PS:

  * 下载live sever:让用户通过服务器查看文件 
  * HTML注释   --注释内不可嵌套!--ctrl+/

  ​            ```<!-- 我是注释 -->```   

     * 注释还能让某一行临时不工作

       ​       

1.4文档声明  

* 为浏览器声明版本供其渲染

  ```<!DOCTYPE html>```

* 好玩的:去看看京东官网的源代码找这个声明  



1.5字符编码  

* UTF-8 万用  如下为浏览器表示解码方式.(可爱的live sever在你犯错时会帮你在运行时改过来) 

  ```<meta charset="UTF-8">```

  <!-- UTF大小写无所谓 -->

* 没存到就是 ? 表示编码失败,且此时数据丢失

* 如果是乱码 ? 表示数据没丢,解码失败

1.6设置语言  

* 目的? 

  告诉浏览器当前语言,便于翻译

* 代码如下  

  <html lang="zh-CN">   

* [语言代码参考手册](https://www.w3school.com.cn/tags/html_ref_language_codes.asp)

* [国家/地区代码参考手册](https://www.w3school.com.cn/tags/html_ref_country_codes.asp)

  

1.7标准结构  

```<!DOCTYPE html> 
<html lang="zh-CN">
	<head>
		<meta charset="utf-8">
		<title>我是标题</title>
	</head>
	<body>
	
	</body>
</html>
```

* 敲 ! 在VScode里可直接生成
* 快捷键- -删除

1.8图片标签   

* 基本装配

```<body>
```

  <!-- src:图片路径   alt:图片描述-->

​    <img src="lotus.jpg" alt="lotus flower">

</body> 

* width&height  调大小--应按比例调好

  