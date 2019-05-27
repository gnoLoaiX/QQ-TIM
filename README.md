# QQ-TIM
预览地址：http://htmlpreview.github.io/?https://github.com/gnoLoaiX/QQ-TIM/blob/master/index.html
</br>
效果展示：
<img width="1080" height="450" src="https://github.com/gnoLoaiX/QQ-TIM/blob/master/images/demo.gif"/>

### Stellar插件
- 描述
    + 视差滚动（Parallax Scrolling）指网页滚动过程中，
      多层次的元素进行不同程度的移动，视觉上形成立体运动效果的网页展示技术
      主要核心就是前景和背景以不同的速度移动，从而创造出3D效果。 
      这种效果可以给网站一个很好的补充。
- 特性
    + 视差滚动效果酷炫，适合于个性展示的场合。
    + 视差滚动徐徐展开，适合于娓娓道来，讲故事的场合。
    + 视差滚动容易迷航，需要具备较强的导航功能。
- 原理
    + 传统的网页的文字、图片、背景都是一起按照相同方向相同速度滚动的，
      而视差滚动则是在滚动的时候，内容和多层次的背景实现或不同速度，或不同方向的运动。
      有的时候也可以加上一些透明度、大小的动画来优化显示。利用background-attachment属性实现。 

- 使用步骤
    + 引用文件
    ~~~html
        <script src="jquery/jquery.min.js"></script>
        <script src="jquery.stellar.min.js"></script>
    ~~~
    + html结构
    ```html
        <div class="content" id="content1">
            <p>TEXT HERE</p>
        </div>
        <div class="content" id="content2">
            <p>TEXT HERE</p>
        </div>
        <div class="content" id="content3" data-stellar-background-ratio="0.5">
            <p>TEXT HERE</p>
        </div>
        <div class="content" id="content4" data-stellar-background-ratio="0.5">
            <p>TEXT HERE</p>
        </div>
        <div class="content" id="content5" data-stellar-background-ratio="0.5">
            <p>TEXT HERE</p>
        </div>
        <div class="content" id="content6" data-stellar-background-ratio="0.5">
            <p>TEXT HERE</p>
        </div> 
    ```
    + 基本样式
    ~~~css
        .content {
            background-attachment: fixed;
            height: 400px;
        }
        #content1 {
            background-image: url("..");
        }
        #content2 {
            background-image: url("..");
        }
        #content3 {
            background-image: url("..");
        }
        #content4 {
            background-image: url("..");
        }
        #content5 {
            background-image: url("..");
        }
        #content6 {
            background-image: url("..");
        }
    ~~~
    + js初始化
    ~~~javascript
        $.stellar({
            horizontalScrolling: false,
            responsive: true
        });
    ~~~
- 参数解释

| 名称                                      | 说明                                       |
| --------------------------------------- | ---------------------------------------- |
| horizontalScrolling 和 verticalScrolling | 该配置项用来设置视差效果的方向。horizontalScrolling设置水平方向，verticalScro设置垂直方向， 为布尔值，默认为true |
| responsive                              | 该配置项用来制定load或者resize时间触发时是否刷新页面，其值为布尔值，默认为false |
| hideDistantElements                     | 该配置项用来设置移出视线的元素是否隐藏，其值为布尔值，若不想隐藏则设置为false |
| data-stellar-ratio="2"                  | 定义了此元素针对页面滚动的速度比率，比如，0.5为页面滚动的50%，2为页面滚动的200%，所以数值越大，你可以看到页面元素滚动速度越快。 |
| data-stellar-background-ratio           | 该配置项用在单个元素中，其值为一个正数，用来改变被设置元素的影响速度。 例如 值为0.3时，则表示背景的滚动速度为正常滚动速度的0.3倍。如果值为小数时最好在样式表中设置 |


##### 完成视觉滚动差页面开发

- 模块一: 导航(nav)
- 模块二: 宣传(banner)
- 模块三: 语音聊天(sound)
- 模块四: 文件传输(file)
- 模块五: 兴趣部落(interest)
- 模块六: 底部(footer)
