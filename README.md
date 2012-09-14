escape
======

---
安装

    npm install escape
    
---
escape 主要用来对数据安全处理，现在能处理的数据类型包括:string, html

用法

    var escape = require('escape');
    var str = escape.execute('hello\tworld');//默认是string类型
    var html = escape.execute('<script>',  {type: 'html'});//html代码
    
运行结果

    str:  'hello\\tworld'
    html: '&lt;script&gt;'