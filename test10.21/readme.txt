1.将两个字符利用字符串对象的方法变成一个字符,显示在页面id为h1的元素中
答:<body>
    <h1 id="h1"></h1>
    <script>
        var str='你好';
        var str1='tom';
        var str=str.concat(str1);
        h1.innerHTML=str;
    </script>
</body>

2.一个富豪想存87万,给理财顾问写了87w,请自动生成存储870000的方法,显示在页面id为h2的元素中
答:<body>
    <h2 id="h2"></h2>
    <script>
        var str='87';
        var sstr=str.padEnd(6,0);
        h2.innerHTML=sstr;
    </script>
</body>

3.一个数字79387.348的工程款,保留两位小数存入,显示在页面id为h3的元素中
答:<body>
    <h3 id="h3"></h3>
    <script>
        var num=79387.348;
        h3.innerHTML=(num.toFixed(2));
    </script>
</body>

4.一张图片是一个相对路径img/head/,icon/1.jpg,我只需要拿到它的文件夹目录后显示在页面id为h4的元素中
答:<body>
    <h4 id="h4"></h4>
    <script>
        var href='img/head/icon/1.jpg';
        h4.innerHTML=href.substring(0,14);
    </script>
</body>

5.用户输入验证码,无论大小写输入都会正确的方法,显示在页面id为h1的元素中,显示在页面id为h4的元素中
答:<body>
    <h5 id="h5"></h5>
    验证码:<input type="password" id="in1">
           <button id="btn">点击</button>
    <script>
        var in1=document.getElementById('in1');
        var btn=document.getElementById('btn');
        var num='ABCD';
        btn.onclick=function(){
            if(in1.value==num.toLowerCase()||in1.value==num.toUpperCase()){
                alert('验证成功');
            }
        }
    </script>
</body>
