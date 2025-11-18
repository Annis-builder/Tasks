CSS 学习笔记  

## 一.CSS(层叠样式表 ) 

### 1.1编写位置  

1.1.1行内样式  

* 名值对  :"名:值"

  ```style="color:red;"```   

  * style--名  

  * ""--值 
  * color--名
  * red--值

* 改字体:font-size  

* 不推荐这种方式  

  * 没有体现结构样式分离  (混乱)

    

1.1.2内部样式

```<html lang="en">
```

<head>
    <meta charset="UTF-8">
    <!-- <meta name="viewport" content="width=device-width, initial-scale=1.0"> -->
    <title>内部样式</title>
    <style>
    h1 {
        color: pink;
        font-size: 24px;
    }
    </style>
</head>

* style中间就是CSS--内部样式

​	即:将所有CSS代码提取出来

* <style>一般放在<head>中

* 问题  
  * 结构与样式没有完全分离  

1.1.3外部样式  

* 新建css文件--建联  

  ``` <link rel ="stylesheet" href="./position3.css">```

* 优点  
  * 完全分离  
  * 触发浏览器缓存机制  
  * 可以复用
  * 表达清晰

1.2.1语法规范  

* h1:选择器(selecter)  --找到要操作的元素  

* {color: green;font-size:40px}:声明块(这里面有两个声明块) 

* color:属性名    freen:属性值  

  