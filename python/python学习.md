### 六个标准数据类型

Number

String

List列表

Tuple元祖

Set集合

Dictionary字典

不可变数据:number\String\Tuple

可变数据:List\Dictionary\Set 





### 字符串常用方法

```.lower()  ```

```  .upper()   ```  

```.split(sep)  ```

``` .replace(old,new)  ``` 

``` .format()  #向str中填充内容```

字符串里的变量:{variable}

转义符:\



### 切片

name = ['','']

### 集合

set(name)

{'',''}

###### 集合的方法





### 字典 key:value

name = dict()

{}



###### 字典的方法

``` .items() 返回所有item``` 

``` .keys() ``` 

```.values()  ```

```.get()  ```

``` []```

转换成list : list(infos.items())[0]



### 传参

*代表之后都使用关键字

1. 序列传参(使用较少)

   `def calc(a,b,c)`

   `l=[1,5,10]`

   `func(*l)`

2. 字典传参(常见)

   `param={"name":"zhangsan","age":18  ...}`

   `func(**param)`

3. 返回值包含多个数据

   `dict={`

   ​		`"employee":[{"s":123},{},{}],`

   ​		`"device":[{},{}]`

   `}`

   `return dict`