<h2 align="center">Robot Framework BuiltIn内置库关键字中文释义 </h2>

## 目录  
  
 --- 
###  🛠 Catenate  
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
> <td></td>
> </tr>
> <tr>
> <td>${str2} =</td>
> <td>Catenate</td>
> <td>SEPARATOR=---</td>
> <td>Hello</td>
> <td>world</td>
> </tr>
> </tbody></table>  
> 
>====>  
> \${str1} = 'Hello world'  
> \${str2} = 'Hello---world'

###  🛠 Comment
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