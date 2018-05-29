# h1～h6 标题

* 无须列表
* 无须列表
* 无须列表

1. 有序列表
2. 有序列表
3. 有序列表


我的名字叫``,所以我要标记他。

````
 console.log(window.document.URL)//获取当前页面URl

````



window.setInterval(),可以传两个参数，第一个：可以是个函数或一段代码字符串；第二个：要间隔执行代码的毫秒数。

````
  var t =  setInterval(function () {
        console.log(new Date())
    },1000);

    setTimeout(function () {
        clearInterval(t)  //停止间断循环执行的setInterval时钟
    },6000)

````


标题跑马灯效果

````

    setInterval(function () {

        var charArray=document.title.split('')//把字符串 转 字符数组
        var lastChat=charArray.pop();
        charArray.unshift(lastChat);
        var newTitle=charArray.join('');
        document.title=newTitle;

    },1000)

````
