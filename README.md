<h2 align="center">Robot Framework BuiltIn内置库关键字中文释义 </h2>

## 目录  
   1. **<a href="#Catenate">Catenate</a>**
   2. **<a href="#Catenate">Comment</a>**
   3. **<a href="#ContinueForLoop">Continue For Loop</a>**
   4. **<a href="#ContinueForLoopIf">Continue For Loop If</a>**
 --- 
###  🛠  Catenate<a id="Catenate"></a>
> **释义:**   
>  将给定的项目链接在一起，并返回结果字符串，默认以空格链接。   
> **参数:**   
> *args  
> **Examples:**   
> <table border="1">
> <tbody><tr>
> <td>${str1} =</td>
> <td>Catenate</td>
> <td>Hello</td>
> <td>world</td>
> <td></td></tr>
> <tr>
> <td>${str2} =</td>
> <td>Catenate</td>
> <td>SEPARATOR=---</td>
> <td>Hello</td>
> <td>world</td>
> </tr></tbody></table>  
> 
>====>  
> \${str1} = 'Hello world'  
> \${str2} = 'Hello---world'


###  🛠 Comment<a id="Comment"></a>
> **释义:**   
>  注释，不执行接受的参数，但是在日志中可见。   
> **参数:**   
> *msg  
> **Examples:**  
> <table border="1">
> <tbody><tr>
> <td>Comment</td>
> <td>这是一个注释</td>
> <td>${arg}</td>
> <td></td>
> </tr>
> </tbody></table>  


###  🛠 Continue For Loop<a id="ContinueForLoop"></a>
> **释义:**   
>  跳过当前循环，进行下一次循环。   
> **参数:**   
> 无  
> **Examples:**  
> <table border="1"><tbody><tr><td>@{VALUES}</td><td>Create List</td><td>CONTINUE</td><td>A</td></tr><tr><td>FOR</td><td>${var}</td><td>IN</td><td>@{VALUES}</td></tr><tr><td></td><td>Run Keyword If</td><td>'${var}' == 'CONTINUE'</td><td>Continue For Loop</td></tr><tr><td></td><td>Log</td><td>${var}</td><td></td></tr><tr><td>END</td><td></td><td></td><td></td></tr></tbody></table>
> 
>====>  
> INFO : A


###  🛠 Continue For Loop If<a id="ContinueForLoopIf"></a>
> **释义:**   
>  跳过当前循环r如果判断为真，进行下一次循环。   
> **参数:**   
> condition  
> **Examples:**  
> <table border="1"><tbody><tr><td>@{VALUES}</td><td>Create List</td><td>CONTINUE</td><td>A</td></tr><tr><td>FOR</td><td>${var}</td><td>IN</td><td>@{VALUES}</td></tr><tr><td></td><td>Continue For Loop If</td><td>'${var}' == 'CONTINUE'</td><td></td></tr><tr><td></td><td>Log</td><td>${var}</td><td></td></tr><tr><td>END</td><td></td><td></td><td></td></tr></tbody></table>
> 
>====>  
> INFO : A
