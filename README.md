cssFormat
=========
一直想自己写个css格式化工具，因为原先的《CSS代码格式化和压缩化》工具，压缩or格式化的都不是我的编码习惯。我的格式化工具也许代码方面细节方面都没他的好，但是符合自身需要的东西才是好东西。

从去年刚学CSS到上个月初，应该正好一年时间。这一年时间，我的CSS编码习惯一直是这样的：

```css
body,div,h1,h2,h3,h4,h5,h6,p,td,tr,form,ul,ol,li,dl,dt,dd,input,button,textarea{
    margin:0;
    padding:0;
}
table{
    border-collapse:collapse;
    border-spacing:0;
    margin:0;
    padding:0;
    line-height:17px;
}
h1,h2,h3,h4,h5,h6{
    font-size:100%;
    font-weight:normal;
}
fieldset,img{
    border:none;
}
ul,ol,li{
    list-style:none;
    vertical-align:bottom;
}
a,a:link,a:visited,a:hover,a:active{
    text-decoration:none;
}
```

直到上月的中旬开始，我才开始转变自己的编码习惯，因为这种编码格式，占的CSS行数太多，不利于查看，尤其是在做大项目的时候。所以我开始采用了下面的CSS编码习惯：

```css
body,div,h1,h2,h3,h4,h5,h6,p,td,tr,form,ul,ol,li,dl,dt,dd,input,button,textarea{margin:0;padding:0}
table{border-collapse:collapse;border-spacing:0;margin:0;padding:0;line-height:17px}
h1,h2,h3,h4,h5,h6{font-size:100%;font-weight:normal}
fieldset,img{border:none}
ul,ol,li{list-style:none;vertical-align:bottom}
a,a:link,a:visited,a:hover,a:active{text-decoration:none}
.clear{clear:both}
.clearfix:after{display:block;content:"";clear:both;height:0}
.clearfix{*zoom:1}
```
这种方式，明显看起来更清爽一些。但是这种又不利于阅读，既然以前收藏的《CSS代码格式化和压缩化》工具满足不了我的需求，那就自己写个好了。于是今天一大早起来看《javascript权威指南》、到公司闲着没事搜索相关文章（《精通 JS正则表达式》），晚上成功写出了半成品。为什么说是半成品呢，因为只限于我自己的编码习惯来操作，别人的CSS未必能很好的格式化出来= =（今天又修改了一下，现在应该是完结版了-2013.07.04）

好吧，晒下地址，欢迎批评指正~

PS：去年写的，刚接触github测试性的上传后删除了，现在想起这是我的第一个github项目（额，小工具）无论如何都要放回去~
