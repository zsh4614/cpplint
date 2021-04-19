### <center>CHANGELOG书写规范v0.2(试用版)</center>

​		本规范规定了团队工程CHANGELOG.MD以及commit message的格式，并通过hook机制在提交时进行监控，避免不规范的代码提交。

> #### CHANGELOG.MD规范

#### 1.CHANGELOG.MD格式

采用如下模板填写：

```
**版本号(日期) by 提交者**

类别: 一行总结性的描述（必须的，注意冒号后面的空格）

- 说明1（可选的）
- 说明2（可选的）
```

==举例如下：==

**0.2(2021.04.19) by zed**

Docs: 修改changelog和commit msg书写规则。

- 修改CHANGELOG.MD书写规范文档

#### 2.CHANGELOG.MD格式说明

1.日期格式为xxxx-xx-xx，提交者为英文名

2.类别只允许使用下面的标识：

- Feat：新功能feature
- Fix：修复bug，可以是外部反馈的bug，也可以是开发者自己发现的bug
- Docs：文档相关documentation
- Perf：优化相关，比如提升性能、体验performence
- Test：增加测试
- Refactor：重构，即不是新增功能，也不是修改bug的代码变动

3.类别后面跟一条本次commit的总结性描述，**使用中文，禁止超过一行**，注意空格

4.每个说明应简明凝练，必须使用**中文，每条禁止超过一行**，可以有也可以没有

5.最新的changelog信息应放在CHANGELOG.MD文档的前面，日期降序排列



> #### commit message规范

1.commit时应使用`git commit`命令，禁止使用`git commit -m "balabala"`

2.务必将CHANGELOG.MD里面本次的changlog信息==拷贝==到终端做为本次commit的message，即保证commit message和CHANGELOG.MD里的==格式与内容完全一致==

3.不用拷贝版本、日期、作者，即不拷贝`**版本号(日期) by 提交者**`这一行，剩下的完全拷贝



欢迎反馈！





