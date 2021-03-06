#Soo
Soo是简易的自制类C编程语言,支持基本的数据类型int,string,支持if,while语句类型,前端经过词法分析,语法分析,语义分析,后端生成自制虚拟机 [Lvm](https://github.com/Leviathan1995/Lvm) 的目标代码.

##File:
* Lsy_Lvm: lvm虚拟机源码
* Lsy_Soo: soo编译器源码
* test:    测试代码
* pzi:截屏图片


##Building and Running:

###*nix:
	$ git clone https://github.com/Leviathan1995/Soo.git
	$ cd Soo/Lsy_Soo
	$ make
	$ ./Soo
	$ 输入源代码绝对路径.例如:/Users/leviathan/Code/Soo/test/heart.txt
	$ 输入中间代码绝对路径.例如:/Users/leviathan/Code/Soo/test/heartlvm.txt
	$ cd ../Lsy_Lvm
	$ make
	$ ./Lvm
	$ 输入中间代码绝对路径.例如:/Users/leviathan/Code/Soo/test/heartlvm.txt
	$ 输入结果文件绝对路径.如果没有结果文件可输入参数:null
	
##Example:
* 利用Soo画一个"心"
* [源代码](https://github.com/Leviathan1995/Soo/blob/master/test/heart.txt)

![image](https://github.com/Leviathan1995/Soo/blob/master/pzi/heart.png)

##Syntax：

* 支持的int,string数据类型
* 支持int型数组
* 支持if,while语句类型
* 支持函数，目前暂不支持参数传递
* 注释使用"#"
* 每行代码结束无须使用";",直接换行即可
* 定义变量使用"var"关键字:
			
		var int i,j,k
		or
		vat string heart
* 定义函数使用"def"关键字:
		
		def heart()
		{
		
			...
			代码语句
			...
		}
* if条件语句:
		
		if(表达式)
		{
			...
			代码语句
			...
		}
* while条件语句:
	
		while(表达式)
		{
			...
			代码语句
			...
		}
* 终端输出使用print():

		print("hello world")
		or
		print(variable)


###License:
	
		MIT
