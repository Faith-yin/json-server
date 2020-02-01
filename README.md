<!--
 * @Author: 殷鹏飞
 * @Date: 2019-08-22 16:50:41
 * @Description: 
 -->
// 获取所有用户信息
http://localhost:3000/users

// 获取id为1的用户信息
http://localhost:3000/users/1

// 获取公司的所有信息
http://localhost:3000/companies

// 获取单个公司的信息
http://localhost:3000/companies/1

// 获取所有公司id为3的用户
http://localhost:3000/companies/3/users

// 根据公司名字获取信息
http://localhost:3000/companies?name=Microsoft

// 根据多个名字获取公司信息
http://localhost:3000/companies?name=Microsoft&name=Apple

// 获取一页中只有两条数据
http://localhost:3000/companies?_page=1&_limit=2

// 升序排序 asc升序 desc降序
http://localhost:3000/companies?_sort=name&_order=asc

// 获取年龄30及以上的
http://localhost:3000/users?age_gte=30

// 获取年龄在30到40之间
http://localhost:3000/users?age_gte=30&age_lte=40

// 搜索用户信息
http://localhost:3000/users?q=h




一、搭建本地数据接口总结笔记：

	1、全局安装 json-server（已安装）

		npm install -g json-server

	2、创建自定义文件夹，然后 cd  该文件夹目录下

	3、初始化 package.json

		npm init

	4、安装依赖包

		npm install json-server

	5、配置启动方式（命令）

		{
			
			"name": "jsonserver",
			"version": "1.0.0",
			"description": "",
			"main": "index.js",
			"script": {
				"json-server": "json-server  --watch  user.json"
			}

		}


	6、在当前目录下创建 user.json 文件（名字自定义）

	7、在终端中启动 jsonserver

		npm run json-server
