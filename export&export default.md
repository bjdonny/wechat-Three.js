在JavaScript ES6中，export与export default均可用于导出常量、函数、文件、模块等，你可以在其它文件或模块中通过import+(常量 | 函数 | 文件 | 模块)名的方式，将其导入，以便能够对其进行使用，但在一个文件或模块中，export、import可以有多个，export default仅有一个。 
具体使用： 
1、



//demo1.js
export const str = 'hello world'

export function f(a){
    return a+1
}123456

对应的导入方式：



//demo2.js
import { str, f } from 'demo1' //也可以分开写两次，导入的时候带花括号12

2、



//demo1.js
export default const str = 'hello world'12

对应的导入方式：



//demo2.js
import str from 'demo1' //导入的时候没有花括号
--------------------- 
作者：zhou_xiao_cheng 
来源：CSDN 
原文：https://blog.csdn.net/zhou_xiao_cheng/article/details/52759632 
版权声明：本文为博主原创文章，转载请附上博文链接！