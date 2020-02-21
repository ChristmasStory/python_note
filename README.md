# python_note
python3学习笔记
1.	111：表示不懂222：表示不同和重点333：
2.	基本语法：
3.	多行注释”””或者’’’;单行注释 #
4.	没有{}，用缩进表示代码块
5.	一般一行就一个语句，如果一句很长可以用在这一行加一个\，来衔接下一行
6.	【】{}（）的多行语句不需要用\，直接换行
7.	只有4种数字类型：int、bool、float、complex（复数1+1j）
8.	字符串string：“+”将字符串连接起来，‘*’str*2可以输出两次字符串
9.	字符串两种索引，从左到右从0开始，从右往左从-1开始。（单个字符的索引）
10.	字符串截取：变量【头下标：尾下标】str[0]第一个字符，str[-1]最后一个字符，str[0:]表示从0取到最后，str[0：-1]表示从0到倒数第二个（不包含最后一个字符）
11.	转义字符\;如果不发生转义，就要字符串前面加一个r（exp：r’hello\n123’）
12.	空行？？？？？？
13.	Input？？
14.	Elif(即else if)
15.	Print()默认输出是换行的，如果要不换行就需要在变量末尾加上end=“ ”print(x,end=” ”)
16.	Import和from…input导入相应的模块
	Import somemodule:将整个模块都导入
	From somemoudule import somefunction:将某个模块中的某个函数导入
	From somemoudule import first function，secondfunc，thirdfunc：将某个模块中的导入多个函数
	From somemoudule import *：将某个模块中的全部函数都导入a, b, c = 1, 2, "runoob"
17.	a, b, c = 1, 2, "runoob"
18.	变量不用声明，但是用前都必须赋值，赋值之后才会被创建。
19.	六个数据类型（不可变数据：Number数字，string字符串，tuple元组；可变数据：list列表、dictionary字典、set集合）
20.	Type(变量)：显示变量类型，isinstance（变量，类型）返回01判断类型是否相同。
21.	Del：可以通过del语句删除单个或者多个对象，或者删除一些对象引用。Del var；del var_a，var_b
22.	2/4得到的是浮点数0.5；2//4得到的是整数0，2**5表示乘方2的5次方
23.	复数complex（a，b）或者可以用a+bj
24.	 截取的数值表示的中间的缝隙，从最一开始：（可以理解成0，第一个数值和第二个数值中的缝隙表示的是1）而在索引中的数值就是直接从数值上数。
25.	字符串不能被改变word[0]=‘m’是错误的。没有char字符类型，是长度为1的字符串。
26.	List中的类型也可以为数字、字符串升值列表（即嵌套）。索引方式和string一样，同样可以用+和*
27.	但是list可以改变，a=【1，2，3】，a【0】=9；a【2：5】=【】可以将对应的元素值设置为【】，把2-5截取掉。
28.	List可以接受第三个参数，参数的作用是截取的步长。即如果步长是2，那么会隔一个截取一个，如果步长为3，则隔着2个截取一个。默认为1；letter=【1：4：2】从1-4中，三个数，取前后。
29.	字长（截取函数第三个参数如果为负数，表示逆向读取）
30.	元组tuple：用小括号（）表示，但是元组中的元素不能修改。其他和list相似。Tuple可以包含可变的对象如list
31.	构造包含0个或者1个元素的元组比较特殊，所以由一些额外的语法规则：tuple1=（）#空元组；tuple2=（20，）#一个元素时需要在元素之后添加逗号。
32.	Set（集合）是由一个或者数个形态各异的大小整体组成的，构成集合的事事物或对象称为元素或者成员。
33.	基本功能是进行成员关系测试和删除重复元素。
	student = {'Tom', 'Jim', 'Mary', 'Tom', 'Jack', 'Rose'} print(student) # 输出集合，重复的元素被自动去掉 
	# 成员测试 
	if 'Rose' in student : 
	print('Rose 在集合中') 
	else :
	print('Rose 不在集合中')
34.	可以使用大括号{}或者set（）函数创建集合，创建一个空集合必须用set（）而不是{}，因为{}是用来创建一个空字典。
35.	Set可以进行集合运算，-减号为差集，|为并集，&为交集，a^b为a和b中不同时存在的元素
36.	字典：相对于list，它是一个无序的对象集，是用{}标识，它是一个无序的key-value的集合，通过键来存取的。不可变
37.	 
38.	字典构造函数dict（）
39.	 
40.	String类型中‘“\都需要用转义字符\，\n：换行；\r:回车;
41.	String类型中可以用in和not in成员运算符可以判断字符是否在字符串中。H in a
42.	不加r：里面的\n是换行。加r会直接翻译字符。”””三引号可以定义字符串跨多行的字符。
43.	List【】修改直接赋值修改，添加使用append()，del删除某一个del a【0】
44.	List的函数：len（list）：列表元素个数；max（）：返回最大值；min（）；list（seq）：将元组转换为list
45.	List方法查表把
46.	元组用（）定义，不能修改，删除只能删除整个元组。Tuple（）
47.	字典用{}定义，字典中的内容为key-value键值对，dict【‘key‘】
48.	Dict.clear():清空字典；del dict:删除
49.	字典的键不能重复，不能修改，所以键可以用数字，字符串，元组，但是不能用list等。Str（dict）可以将字典输出成字符串打印出来。
50.	集合{}，空集要用set（）。{}是空字典。
51.	添加集合元素s.add(x)。s.update（{x，y}）s.remove(x).s.discard(x):也可以移除元素。S.pop()随机删除一个
运算符
1.	逻辑运算符：and or not
2.	成员运算符：（包含一系列的成员，包括字符串，列表，元组）
	in(not in) 返回值为true false（在不在序列中）
3.	身份运算符：比较两个对象的存储单元
4.	is（is not）判断两个标识符是不是引用自一个对象。（a=20，b=20；a is b 返回true）
编程
1.	a, b = b, a+b（计算顺序，n=b,m=a+b,a=n,b=m）（不是a=b,b=a+b）
2.	end=’符号’：end关键字用于将结果输出到同一行，或者在输出的末尾添加不同的字符。如果不添加end就会换行输出，
3.	没有switch-case
4.	age = int(input("请输入你家狗狗的年龄: "))
5.	input("点击 enter 键退出")
6.	没有do-while
7.	While-else:条件语句为false时执行else 的语句块（1次）
8.	For x in <sequence>，同时也存在for else；当break打破循环体后，不会进入else语句中。
9.	如果需要遍历数字序列，可以使用内置range（）函数。For I in range(2,9),遍历2-8.range函数是左闭右开
10.	Range函数可以添加第三个参数，表示为步长。Range（0,10,3）表示为从0-10步长为3，输出为0369。步长也可以是负数，表示为反向取
11.	通过range函数和len函数遍历一个序列的索引。For I in range(len(a)):print(i,a[i])
12.	 
13.	通过range函数创建list：list(range(5))输出【0，1，2，3，4】
14.	Range函数左闭右开，range（2，2）好像是没有，不是2。也可以用for I in [2,3]
15.	Pass不做任何事情，一般用作占位置语句，为了保持程序结构的完整性。
16.	None也是false

迭代器和生成器
1.两个方法：iter()和next()
2.iter创建迭代器对象，参数为迭代的对象，字符串元组列表。Next输出迭代器下一个元素，参与为迭代器名称。it=iter(list);print(next(it))
3.同样也可以使用for来遍历。It=iter(list);for x in it : print(x,end=’’)
4. while True: 
try: 
print (next(it)) 
except StopIteration: 
sys.exit()
stoplteration异常用于标识迭代的完成，防止出现无尽循环的情况。
Try:xxx except Stoplteration:XXXX

函数
1.	def 函数名（参数）
2.	number是不可改变的对象，但是a=5;在赋值a=10，这实际是新生成一个int值对象10，再让a指向它，5被丢弃，不是改变了a的值。
3.	def ChangeInt( a ): 
a = 10 
b = 2
ChangeInt(b) 
print( b ) # 结果是 2。当b的值传给参数a，再函数里面把10再次赋给a，那么a会重新生成一个对象10，并将a指向。
可变对象当参数时，再函数内改变对象，那原始的参数也被改变。
def changeme( mylist ): #"修改传入的列表" 
mylist.append([1,2,3,4]) 
print ("函数内取值: ", mylist) 
return # 调用changeme函数 

mylist = [10,20,30] 
changeme( mylist ) 
print ("函数外取值: ", mylist)
输出都是。[10, 20, 30, [1, 2, 3, 4]]。
4.	不定长参数，一个函数能处理比当初声明时更多的参数。对于不定长的参数，在定义的时候采用加*的方式来定义该参数如：def f（【forma】，*var_args），加了*的参数会以元组的形式导入，存放所有未命名的变量参数。
5.	def printinfo( arg1, *vartuple ):{} printinfo( 70, 60, 50 )输出：70
6.	(60, 50)
7.	如果加了两个星号**的参数会以字典的形式导入。Def F(arg,**var);f(1,a=2,b=3)输出1，{‘a’:2,’b’:3}.
8.	声明函数时，参数中星号*可以单独出现，def f（a，b，*，c）：f(1,2,3)错误；f（1，2，c=3）。单独*出现在参数中必须用关键字传入。
9.	匿名函数使用lambda来创建函数，lambda的主体是一个表达式，而不是一个代码块，仅仅能在lambda表达式中封装有限的逻辑进去。lambda函数中不能访问自己参数列表之外或者全局命名空间的参数。
10.	Lambda 【arg1【，…】】：expression（sum = lambda arg1, arg2: arg1 + arg2）直接使用sum（）函数就可。
数据结构
1.	列表方法
2.	方法append(x),将x作为元素加到列表的结尾，x是一个元素，即便x是一个list类型，也是整体添加到结尾，输出结果为嵌套list 的list类型
3.	方法extend（seq）seq可以为元组tuple列表list集合，但是当为字典时，只将字典的key键作为元素依次添加到结尾
4.	insert（i,x）在指定位置上插入一个元素，第一个参数为元素索引，list.insert(0,x)会插入到整个列表之前，x为一个元素。会在索引i前面插入。
5.	remove（x）删除列表中值为x的第一个元素，如果没有返回一个错误
6.	clear清楚列表中所有元素
7.	pop（【i】），从列表的指定位置移除元素，并将其返回。如果没有指定索引，a.pop()返回最后一个元素，元素随即从列表中被移除。堆栈
8.	index（x）返回列表第一个值为x的元素的索引，没有匹配返回错误。
9.	count(x)返回x在列表中出现的次数
10.	sort（），对元素进行排序
11.	reverse（）倒排列表中的元素
copy，返回列表的浅复制
12.	列表当作堆栈使用	append为进栈函数，pop为出栈函数（pop函数返回的是出栈的元素值）
13.	list当做队列使用，append为进栈函数，popleft(),作出栈函数
列表推导式：由一个表达式生成一个新的列表。例如
vec=【2，4，6】；【3*x for x in vec】输出【6，12，18】
或者【【x,x**2】for x in vec】输出为【【2，4】【4，16】【6，36】】
或者【3*x for x in vec if x>3】输出为【12，18】首先判断if条件
或者【3*x for x in vec if x<2】输出为【】空的
或者【x*y for x in vec1 for y in vec2】输出x和y两两相乘的结果
或者【vec1[i]*vec2[i] for i in range(len[vec1])】即输出相应索引上的数相乘的结果
14.字符串方法strip（‘x’或者空）去除收尾字符x，或者去除首尾的空格
15.嵌套列表
Matrix=[
[1,2,3,4],
[5,6,7,8],
[9,10,11,12]]
对3*4矩阵进行转置：
第一种方法【【row[i] for row in maxtrix】for i in range(4)】
第二种方法：重新定义一个list，利用for和嵌套列表完成。
	Transposed=[];
	For i in range(4):
		Transposed.append([row[i] for row in matrix])
	第三种方法：for i in range(4):
transposed_row = []
for row in matrix:
    transposed_row.append(row[i])
transposed.append(transposed_row)
16.	 del可以删除一个元素，a[i],也可以一段a[:],也可以全部删除del a
17.	 {}是空字典，set（）是空集合set（‘abcdsfafwe’）输出为{‘a’,’b’…}
18.	字典的key是不可变类型，通常是字符串和数值，应该不能是可变的类型
19.	字典的添加可以直接添加tel={key：12，key2=23}；tel【key3】=456
20.	List（tel.keys()）输出list的key；sorted（tel.keys()）输出排序后的key
21.	字典的构造函数：dict（【（‘sape’，156），（‘sae’，56）】）
可以用字典推导{x:x**2 for x in (2,4,6)}输出{2:4,4:16,6:36}
Dict(spac=12,ef=489)
22.	字典的遍历：关键字和对应的值可以使用items（）方法同时解读出来
For k,v in dictionary.items():print(k,v)或者
For I,v in enumerate([‘key1’,’key2’]);print(I,v)
或者
>>> questions = ['name', 'quest', 'favorite color']
>>> answers = ['lancelot', 'the holy grail', 'blue']
>>> for q, a in zip(questions, answers):
...     print('What is your {0}?  It is {1}.'.format(q, a))
如果反向遍历
for i in reversed(range(1, 10, 2)):
...     print(i)
顺序排序遍历一个序列
basket = ['apple', 'orange', 'apple', 'pear', 'orange', 'banana']
>>> for f in sorted(set(basket)):
...     print(f)
模块
1.	Sys模块import 引入，如果长时间使用函数，那么可以使用fib=fibo.fib；（没有（））将模块中的函数赋给一个本地的名称。
2.	From 模块 import name(指定部分的命名空间或者函数)，当name为*可以引入所有内容
3.	__name__属性，一个模块被另一个程序第一次引用时，其主程序将运行。如果我们想在模块被引入时，模块中的某一程序块不执行，我们可以用__name__属性来使该程序块仅在该模块自身运行时执行。
！！！！__name__属性用于分开调用和自身运行的分流。自身运行和被其他程序用模块的方式调用。
4.	dir(模块名)输出模块内定义的所有名称，以一个字符串列表的形式返回。如果没有参数，则返回罗列出当前定义的所有名称。
5.	包是一种管理python模块命名空间的形式，采用点模块名称。比如一个模块的名称A.B，那么它表示一个包a中的子模块b。
6.	目录中有__init__.py的文件才会被认为是一个包，子包里也有一个__init__.py文件。
7.	两种模块引用方式：一个是import sound.effects.echo引用时也要将模块的名字写上，sound.effects.echo.echofilter()；另一个中方式是from sound.effect import echo使用的时候只用输出echo.echofiter()。
8.	多级包导入，最后一项之前都必须是包，最后一项可以是模块可以是包。A.b.c.d中abc必须是包
9.	除非是你要导入的子模块有可能和其他包的子模块重名。
输入输出（format）
1.	Print()
2.	使用文件对象的write()
3.	标准输出文件可以用sys.stdout引用
4.	Str.format()函数来格式化输出值
5.	如果将输出的值转化为字符串，可以使用repr()或str()函数来实现。
6.	Str函数返回一个用户易读的表达形式
7.	Repr函数产生一个解释器易读的表达形式
8.	字符串对象的rjust（x）方法，它可以将字符串靠右，并在左边填充空格。
9.	Ljust()和center()
10.	zfill()它会在数字的左边填充0。’12’.zfill(5)输出00012 。参数为字符串的长度，不是i添加0的个数，而是加上原有字符后再添加0，如果本身的长度大于5，那么不会再添加0.
11.	Str.format()括号及其里面的字符（称作格式化字段）将会format()中的参数替换。再括号中的数字用于指向传入对象再format（）中的位置。
Print(‘{}和{}’.format(‘google’,’max’))输出google和max
Print(‘{0}和{1}’.format(‘google’,’max’))输出google和max
Print（‘{1}和{0}’.format(‘google’,’max’)）输出max和google
12.	Format也可以使用位置及关键字参数可以任意的结合。
Print（‘{0}和{1}和{other}’.format(‘第一’，‘第二’，other=‘第三’)）
13.	 ‘{：}’.format（）：可选项：和格式标识符可以跟着字段名，
14.	读取键盘输入：Input（）从标准输入读入一行文本
Str=input(“请输入：”);print(str);
输入合法的整数：x=int(input(“请输入一个数字：”))
try: 
x = int(input("请输入一个数字: ")) 
break 
except ValueError: 
print("您输入的不是数字，请再次尝试输入！")
15.	读写文件：open()将会返回一个file对象 语法格式open(filename,mode),文件名包括后缀名，如果不在当前目录，需要地址。Mode模式决定打开文件的模式，只读，写入，追加等。默认文件访问模式为只读r。
rb以二进制格式打开一个文件用于只读，文件指针将会放在文件的开头。
r+打开一个文件用于读写
rb+二进制格式打开一个文件用于读写
w，wb，w+，wb+
a用于追加ab：二进制追加a+读写，放在结尾；ab+二进制读写放在结尾
  
16.	f.open（”/tmp/foo.txt”,”w”）#打开一个文件;f.write();#写进内容f.close();#关闭文件
17.	f.read(size),读取文件，size可选数字类型的参数。
18.	f.readline(),从文件中读取单独的一行，换行符为‘\n’如果返回是一个空字符串，说明已经读取到最后一行。
19.	f.readlines，将返回该文件中包含的所有行。如果设置可选参数sizehint，则读取指定长度的字节，并且将这些字节按行分割。
20.	f.write(string)写进文件，返回的是字符数。Num=f.write(“abcde”),输出num是5.
Value=(‘www’,14);s=str（value）;f.write(s);
21.	f.tell()返回文件对象当前所处的位置，它是从文件开头开始算起的字节数。
22.	f.seek()如果要改变文件当前的位置，可以使用f.seek（offset，from_what）函数，from_what的值，如果是0表示开头，如果是1表示当前位置，2表示文件的结尾。
seek(x,0):从起始位置即文件首行首字符开始移动x个字符
seek(x:1):表示从当前位置往后移动x个字符
seek(-x:2):表示从文件的结尾往前移动x个字符
异常和错误
1.	Try：XXX except 异常类型：XXX；如果异常的类型和except之后的名称符，那么except子句才会被执行。
2.	如果想同时处理多个异常，那么这些异常放在一个元组里except (RuntimeError, TypeError, NameError): pass
3.	当不同的异常执行不同程序时，可以多写几个except。
except OSError as err: 
print("OS error: {0}".format(err)) 
except ValueError: 
print("Could not convert data to an integer.") 
except: 
print("Unexpected error:", sys.exc_info()[0]) 
raise 
4.	Try except else finally:如果有异常，执行except异常处理，不会执行else，finally不管什么时候都会执行。如果没有异常，，执行完try后，会执行else，else专门为了执行没有出现异常时，执行的else。Finally也会在最后执行。
 
5.	Raise【exception[,args[,traceback]]】raise抛出异常。
x = 10 
if x > 5: 
raise Exception('x 不能大于 5。x 的值为: {}'.format(x))
运行会发生异常，提示出异常信息，输出x不能大于5，x的值为10
面向对象编程
1.	类又一个名为__init__()构造函数，该方法在类实例化时会自动调用。
Def __init__(srlf):self.data[]
例如：def __init__(self, realpart, imagpart): 
self.r = realpart 
self.i = imagpart
Self代表类的实例，而非类。Self在类中使用，表示被定义的实例（instance）对象。print(self)；print(self.__class__)输出<__main__.Test instance at 0x100771878>
__main__.Test
2.	Self不是关键字，所以换成其他的也是可以正常执行。所以需要在定义函数中写上想要的参数。
3.	定义函数中必须包含参数self，且为第一个参数。
