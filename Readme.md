# 开发前准备

## 准备
#### 一、人员角色安排与职责
- **产品负责人**
	- 资源管理（收集到的资源，分类管理）
		- 需求表
		- 测试账号 密码
	- 产品功能列表
	- 会议安排（计划会，评审会，反思会）
	- 决定发布时间和发布内容
	- 迭代任务
	- 工作排序
	- 审核原型，审核UI（合理性，缺漏，多余）

	- *如果使用jira*
	   - 编写用户故事
	   - 确定用户故事优先级

- **设计**
	- 提供UI设计（页面设计，图标设计）
	- 上传至蓝湖或其他工具。
	- 切好的图标单独放一起。

- **开发团队**  
    *前端*
    - 技术选型
    - 技术评估
    - 估算时间  

    *后端*
    - 技术选型
    - 技术评估
    - 估算时间
    - 确定接口规则

- **运维**
	- 提供环境
		- dev环境
		- test环境
		- staging环境
		- production环境

#### 二、版本（内容）更新
- **迭代版本：** x.0.0
- **功能版本：** 1.x.0
- **修复bug版本：** 1.0.x
- **每次版本更新内容，记录存档**

#### 三、生命周期
**每次迭代：**  商业建模 --> 需求 --> 分析&设计 --> 开发实现 --> 测试 --> 部署
- 商业建模
	*
- 需求
	*
- 分析&设计
	*
- 开发实现
	*
- 测试
	*
- 部署
	*
	
## 团队容量计算  
  22天 – 2天（计划会1天，评审会/反思会1天）  
=20天 – 5天（假设有5天已经确认的培训/出差等）  
=15天 × (0.5 to 0.7) （修改Bug/额外任务占用30 to 50%）  
=7.5～10.5天   
  
  若团队有10人，则有效工作日有75～105人天。  
  一般刚成立或刚实践敏捷的团队，取最低值75人天。

## 管理
#### 一、资源管理
- 项目资源
- 前端资源
- 后端资源

#### 二、代码管理
- **git**
	- 分支规范
		- `master`：线上稳定版 （保护分支）
		- `master1.x.x`：迭代版本
		- `dev`：开发最新 （保护分支）
		- `dev1.x.x`：某个迭代版本 最新
		- `test`：测试相关
		- `staging`：staging测试
		- `feat-xxx`：新增功能分支（每新增模块，功能需要新增，由开发者新增）
		- `fix-xxx`：修复bug分支（每修改一个bug，由修复的开发者新增）
		- `style` 代码风格相关无影响运行结果的
		- `perf` 优化/性能提升
		- `refactor` 重构
		- `revert` 撤销修改
		- `docs` 文档/注释
		- `chore` 依赖更新/脚手架配置修改等
		- `workflow` 工作流改进
		- `ci` 持续集成
		- `types` 类型定义文件更改
		- `wip` 开发中  
        ***注：***  
        团队开发人员多的话，更快区分代码的由谁负责，分支的命名可以改为：feat-（名字）-xxx（如：feat-caro-login）  
        每日，或功能完成，或bug修复，更新代码：创建合并请求（PR），由负责人检查合并到dev分支

- **前端开发规范**

1.公用资源管理规范：

- 公用资源管理，应备份记录在readme.md文件中
	- UI设计资源地址：（蓝湖的地址路径）
	- 测试账号，密码
	- 所用到的网络资源，例如：
		- 地图API  
			账号：   
			密码：  
			key：  
			sessert ID：  
			等
	- 部署：
		- 测试   
			IP：**  
			账号：**  
			密码：**  
			所在地址路径：**  
		- staging
		- production  
		- OSS  
			账号，密码，路径  
		**注**  （账号，密码 出于安全性考虑的话，可以由一个人保管，备注是谁：姓名）  

2.代码规范：

- 工程目录规范
- 命名规范
	- 驼峰命名
	- 文件夹下 应 以index为入口（如：`test/index.js`）
	- 公用组件命名：需以开发人员的名字（或代号）作为前缀, 英文名+组件名（用图，功能）如：CaroButton
	- 变量，文件夹，文件命名，可以使用英文，拼音（使用拼音者，需要全拼，太长的话，后面可以用首字母代替+注释）
- 编写规范
	- 以eslint为标准，根据个人偏好
- 封装的组件或工具
	- 要么写测试用例，要么在readme.md文件中编写实例，方便其他人使用。
