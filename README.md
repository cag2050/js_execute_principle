### js执行代码流程(边编译边处理)：对所有的代码块，按顺序进行 语法分析=》预编译=》执行。
    　　step 1. 读入第一个代码块。
    　　step 2. 做语法分析，有错则报语法错误（比如括号不匹配等），并跳转到step5。
    　　step 3. 对var变量和function定义做“预编译处理”（永远不会报错的，因为只解析正确的声明）。
    　　step 4. 执行代码段，有错则报错（比如变量未定义）。
    　　step 5. 如果还有下一个代码段，则读入下一个代码段，重复step2。
    　　step 6. 结束。
* 地址：http://www.cnblogs.com/cag2050/p/7687775.html
    
### 配置了gulp和browser-sync。  
说明：
1. 在项目目录运行gulp命令(需要先全局安装gulp)，会打开gulpfile.js中设置的根目录下的index.html。
2. 若访问其他文件，需要自己补充网址。例如：http://localhost:3000/html/[xxx].html
