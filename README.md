<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <!-- 引入 layui.css -->
    <link href="//unpkg.com/layui@2.9.13/dist/css/layui.css" rel="stylesheet">
    <link rel="stylesheet" href="./css/style.css">
    <style></style>
</head>

<body>
    <div class="pos"></div>
    <div style="margin: 0 auto;width: 80%;">
        <nav style="display: flex;justify-content: space-around;align-items: center;height: 120px;">
            <h4>个人中心</h4>
            <img src="./img/蓝色隔断三角形服装公司logo创意服饰中文logo.png" alt="" style="width: 200px;">
            <h2 style="color: #6fc6b5;width: 30%;font-size: 36px;">传播学系官网<br>Communication</h2>
            <div class="layui-form-item">
                <div class="layui-input-group">
                    <div class="layui-input-prefix">
                        搜索
                    </div>
                    <input type="text" placeholder="搜索学校新闻" class="layui-input">
                    <div class="layui-input-split layui-input-suffix" style="cursor: pointer;">
                        <i class="layui-icon layui-icon-search"></i>
                    </div>
                </div>
            </div>
        </nav>
        <ul class="layui-nav layui-bg-gray"
            style="display: flex;justify-content: space-around;border-bottom: 2px solid #ccc;margin-bottom: 10px;">
            <li class="layui-nav-item layui-this">
                <a href="javascript:;">首页</a>
                <dl class="layui-nav-child">
                    <dd><a href="">选项1</a></dd>
                    <dd><a href="">选项2</a></dd>
                    <dd><a href="">选项3</a></dd>
                </dl>
            </li>
            <li class="layui-nav-item">
                <a href="./page.html">介绍</a>
                <dl class="layui-nav-child">
                    <dd><a href="">选项1</a></dd>
                    <dd><a href="">选项2</a></dd>
                    <dd><a href="">选项3</a></dd>
                </dl>
            </li>
            <li class="layui-nav-item">
                <a href="javascript:;">教务系统</a>
                <dl class="layui-nav-child">
                    <dd><a href="">选项1</a></dd>
                    <dd><a href="">选项2</a></dd>
                    <dd><a href="">选项3</a></dd>
                </dl>
            </li>
            <li class="layui-nav-item">
                <a href="javascript:;">学生天地</a>
                <dl class="layui-nav-child">
                    <dd><a href="">选项1</a></dd>
                    <dd><a href="">选项2</a></dd>
                    <dd><a href="">选项3</a></dd>
                </dl>
            </li>
            <li class="layui-nav-item">
                <a href="javascript:;">资料下载</a>
                <dl class="layui-nav-child">
                    <dd><a href="">选项1</a></dd>
                    <dd><a href="">选项2</a></dd>
                    <dd><a href="">选项3</a></dd>
                </dl>
            </li>
        </ul>
        <div class="layui-carousel" id="ID-carousel-demo-set" lay-filter="filter-demo-carousel-set"
            style="margin: 0 auto;">
            <div carousel-item>
                <div>
                    <img src="./img/WechatIMG6e4caa39700ac3fef612c52a660bdabc.jpeg" alt="">
                </div>
                <div>
                    <img src="./img/WechatIMG29.jpeg" alt="">
                </div>
                <div>
                    <img src="./img/WechatIMG6e4caa39700ac3fef612c52a660bdabc.jpeg" alt="">
                </div>
                <div>
                    <img src="./img/WechatIMG6e4caa39700ac3fef612c52a660bdabc.jpeg" alt="">
                </div>
                <div>
                    <img src="./img/WechatIMG6e4caa39700ac3fef612c52a660bdabc.jpeg" alt="">
                </div>
            </div>
        </div>

        <div style="width: 70%;margin: 100px auto;">
            <ul>
                <li style="display: flex;align-items: center;">
                    <img src="./img/WechatIMG285.jpg" alt="" style="width: 50%;height: 300px;">
                    <div style="display: inline-block;width: 50%;">
                        <h1 style="font-size: 40px;text-align: center;">我院女篮成果夺冠</h1>
                        <button class="xun">5月4日我院女篮在分院杯夺冠</button>
                    </div>
                </li>
                <li style="display: flex;align-items: center;flex-direction: row-reverse;margin-top: 150px;">
                    <img src="./img/WechatIMG286.jpg" alt="" style="width: 50%;height: 300px;">
                    <div style="display: inline-block;width: 50%;">
                        <h1 style="font-size: 40px;text-align: center;">红船杯一等奖</h1>
                        <button class="xun" style="position: relative;margin-left: 0px;">我选获得红船杯一等奖</button>
                    </div>
                </li>
            </ul>
        </div>
        <div class="mybox mybox1" style="">
            <img src="./img/WechatIMG287.jpg" alt="">
            <img src="./img/DSC01827-2.JPG" alt="">
            <img src="./img/WechatIMG6e4caa39700ac3fef612c52a660bdabc.jpeg" alt="">
        </div>
        <div class="mybox" style="background-color: #6fc6b5;height: 300px;transform: translateY(200px);">
            <img src="./img/Snipaste_2024-06-20_16-05-09.png" alt=""
                style="display: block;margin: 0 auto;transform: translateY(-100px)">
            <div style="text-align: center;color: #000;">
                <h2>联系我们</h2>
                <h2>×××××××××××××××××××××××××××××××××</h2>
            </div>
        </div>
    </div>
    <!-- 引入 layui.js -->
    <script src="//unpkg.com/layui@2.9.13/dist/layui.js"></script>
    <script>
        layui.use(function () {
            var carousel = layui.carousel
            var form = layui.form
            var util = layui.util
            var $ = layui.$
            // 渲染
            var carInst = carousel.render({
                elem: '#ID-carousel-demo-set',
                indicator: "outside"
            })
        });
    </script>
</body>

</html>
