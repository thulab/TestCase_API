
# TestCase_API

Software Engineering Group

1.jmeter用例的命名:

保存为jmx:模块首字母_Swagger中模块的名字(模块名字:如果引用多个模块中的接口,写主要模块的名字)

测试计划:模块首字母_模块名称(中英文)

线程组:子功能编号_文字/英文描述

请求:模块首字母_子功能编号_步骤编号S_[Y/N]_文字/英文描述  (Y/N正向,逆向; 请求的描述对应Swagger请求的名字)

2.详细的断言

3.对于做验重的参数，使用变量

4.涉及到ip地址位置不要写死ip，使用 ${ipAddress}

5.如图片：规则示例图

6. 接口用例新增和修改：
  修改：在原有jmx文件上修改
  新增：接口在原来Controller内（如6060：Meta Class Controller），就在原有jmx用例后面增加新的线程组。
        接口新建了Controller时，用例重新创建jmx文件，命名规则如上所示。
        
下载安装说明：

1.下载后将data文件夹复制到jmeter安装根目录。

2.jmeter需要安装插件plugins Manager，在plugins Manager中搜索Custom JMeter Functions进行安装，为了支持base64函数。
  


