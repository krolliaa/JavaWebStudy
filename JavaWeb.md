# `JavaWeb`

## 1. `HTML`

全称：超文本标记语言。下面是一个简单的`html`文件，`HTML`是解释性语言，一行行解释，解释出错不显示，浏览器可以尽量容错。

下面这个`html`文件涵盖了几乎所有有必要学习的`html`标签。除此之外简单了解下`frameset iframe`两个标签。

```html
<html>
<head>
    <title>这是一个网页标题</title>
    <meta charset="utf-8">
    <style type="text/css">
        div {
            width: 200px;
            height: 200px;
            position: absolute;
        }
        #div1 {
            background-color: red;
            top: 0px;
            left: 20px;
        }
        #div2 {
            background-color: orange;
            top: 20px;
            left: 40px;
        }
        #div3 {
            background-color: yellow;
            top: 40px;
            left: 60px;
        }
    </style>
</head>
<body>
    Hello World!<br>你好，这是中国！
    <p>这是第一个段落</p>
    <p>这是第二个段落</p>
    <img src="images/default.jpg" width="100" height="100" alt="图片显示错误时显示【这里的images是相对路径】"/>
    <h6>标题六</h6>
    <h5>标题五</h5>
    <h4>标题四</h4>
    <h3>标题三</h3>
    <h2>标题二</h2>
    <h1>标题一</h1>
    <ol type="A" start="3">
        <li>Apple</li>
        <li>可口可乐</li>
        <li>美国通用</li>
        <li>宁德时代</li>
        <li>九安医疗</li>
    </ol>
    <ul type="square">
        <li>比亚迪</li>
        <li>浙江建投</li>
        <li>湖南发展</li>
        <li>浙江鼎力</li>
        <li>河化股份</li>
    </ul>
    <b>加粗：你是喜欢吃甜玉米还是糯玉米？</b><br>
    <i>斜体：你是喜欢吃甜玉米还是糯玉米？</i><br>
    <u>下划线：你是喜欢吃甜玉米还是糯玉米？</u><br>
    <b>水分子的表达式：H<sub>2</sub>O</b><br>
    <b>氧气的表达式：O<sup>2</sup></b><br>
    <b>5&lt;10</b><br>
    <b>10&gt;5</b><br>
    <b>5&le;10</b><br>
    <b>10&ge;5</b><br>
    <b>注册商标：&reg;</b><br>
    <b>版权符号：&copy;</b><br>
    <b>百度搜索：HTML实体即可</b><br>
    <span>Google</span><br>
    <a href="https://www.baidu.com" target="_parent">Google 注册号正确&reg; 版权正确&copy;</a><br>
    <a href="https://www.baidu.com" target="_self">Google 注册号正确&reg; 版权正确&copy;</a><br>
    <a href="https://www.baidu.com" target="_blank">Google 注册号正确&reg; 版权正确&copy;</a><br>
    <a href="https://www.baidu.com" target="_top">Google 注册号正确&reg; 版权正确&copy;</a><br>
    <div id="div1">div1</div>
    <div id="div2">div2</div>
    <div id="div3">div3</div>
    <table border="1" width="666" cellspacing="0" cellpadding="20">
        <tr align="center">
            <td>姓名</td>
            <td>年龄</td>
            <td>等级</td>
            <td>果实</td>
        </tr>
        <tr align="center">
            <td>张三</td>
            <td>10</td>
            <td>A</td>
            <td>橡胶果实</td>
        </tr>
        <tr align="center">
            <td>李四</td>
            <td>11</td>
            <td>B</td>
            <td>闪闪果实</td>
        </tr>
        <tr align="center">
            <td>王五</td>
            <td>12</td>
            <td>C</td>
            <td>烧烧果实</td>
        </tr>
    </table>
    <table border="1" cellspacing="0" cellpadding="20">
        <tr align="center">
            <td>名称</td>
            <td>单价</td>
            <td>数量</td>
            <td>小计</td>
            <td>操作</td>
        </tr>
        <tr align="center">
            <td>苹果</td>
            <td rowspan="3">5</td>
            <td>20</td>
            <td>100</td>
            <td>A</td>
        </tr>
        <tr align="center">
            <td>菠萝</td>
            <!--<td>5</td>-->
            <td>20</td>
            <td>100</td>
            <td>B</td>
        </tr>
        <tr align="center">
            <td>香蕉</td>
            <!--<td>5</td>-->
            <td>20</td>
            <td>100</td>
            <td>C</td>
        </tr>
        <tr align="center">
            <td>总计</td>
            <td colspan="4">181</td>
        </tr>
    </table>
    <form action="success.html" method="get">
        昵称：<input type="text" name="name" value="请输入您的昵称"/><br/>
        密码：<input type="password" name="pwd"/><br/>
        性别：<input type="radio" name="gender" value="male">男
             <input type="radio" name="gender" value="female" checked="checked">女
        爱好：<input type="checkbox" name="hobbies" value="basketball">篮球
             <input type="checkbox" name="hobbies" value="football">足球
             <input type="checkbox" name="hobbies" value="swimming" checked="checked">游泳<br/>
        星座：<select name="star">
                <option value="白羊座">白羊座</option>
                <option value="双鱼座">双鱼座</option>
                <option value="狮子座">狮子座</option>
                <option value="天蝎座" selected="selected">天蝎座</option>
                <option value="天秤座">天秤座</option>
                <option value="射手座">射手座</option>
                <option value="处女座">处女座</option>
             </select><br/>
        备注：<textarea name="remark" rows="4" cols="66"></textarea><br/>
        <input type="submit" value="注册">
        <input type="reset" value="重置">
        <input type="button" value="普通">
    </form>
</body>
</html>
```

```html
<html>
<head>
    <title>这是一个网页标题</title>
    <meta charset="utf-8">
</head>
<body>
    <h1 style="color: red">注册成功！</h1>
    <iframe src="frameset/top.html"/>
</body>
</html>
```

```html
<html>
<head>
</head>
<frameset rows="20%, *">
    <frame src="frameset/top.html">
    <frameset cols="20%, *">
        <frame src="frameset/left.html">
        <frameset rows="80%, *">
            <frame src="frameset/right.html">
            <frame src="frameset/bottom.html">
        </frameset>
    </frameset>
</frameset>
</html>

<html>
<head>
    <title>这是一个网页标题</title>
    <meta charset="utf-8">
</head>
<body>
<h1 style="color: deepskyblue">Top Page</h1>
</body>
</html>

<html>
<head>
    <title>这是一个网页标题</title>
    <meta charset="utf-8">
</head>
<body>
<h1 style="color: deepskyblue">Left Page</h1>
</body>
</html>

<html>
<head>
    <title>这是一个网页标题</title>
    <meta charset="utf-8">
</head>
<body>
<h1 style="color: deepskyblue">Right Page</h1>
</body>
</html>

<html>
<head>
    <title>这是一个网页标题</title>
    <meta charset="utf-8">
</head>
<body>
<h1 style="color: deepskyblue">Bottom Page</h1>
</body>
</html>
```

## 2. `CSS`

### 2.1 基础知识

```html
<html>
<head>
    <meta charset="UTF-8">
    <style type="text/css">
        p {
            color: deepskyblue;
        }

        .f20 {
            font-size: 20px;
        }

        #p3 {
            background-color: deeppink;
            font-size: 24px;
            font-weight: bolder;
            font-style: italic;
            font-family: 华文彩云;
        }

        .f32 {
            font-size: 32px;
        }
    </style>
    <link rel="stylesheet" href="index.html">
</head>
<body>
    <p>这是第一个段落</p>
    <p class="f20">这是第二个段落</p>
    <p id="p3">这是第三个段落</p>
    <div>
        <p><span style="font-size: 60px;font-weight: bolder;font-style: italic;color: orange">HELLO</span></p>
        <span class="f32">World</span>
    </div>
</body>
</html>
```

### 2.2 盒子模型

简单了解下`IE`盒子模型也称怪异盒子模型，第二种就是标准盒子模型，前者的`width`包含`width margin padding`，而后者`width`就是`width`。

`position: absolute` -- 绝对定位 , 需要配合使用`left , top`
`relative` -- 相对定位 , 一般会和`float , margin , padding ....`一起使用
