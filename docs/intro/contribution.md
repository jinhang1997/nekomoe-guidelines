# 参与编写

## 环境安装

喵萌奶茶屋大宝典基于 Docusaurus 制作，[这里是官方的文档](https://docusaurus.io/docs)。<br/>
要运行或修改这个项目，需要机器上[安装 Node.js 环境](https://nodejs.org/)。

## 获取项目

直接从奶茶屋主 GitHub 的仓库列表中克隆（clone）本仓库到本地修改，或分叉（fork）后修改再提交合并请求（pull request）。

## 启动项目

1. 将仓库克隆到本地后，切换到仓库的根目录。
2. 执行 `npm install` 命令自动安装相关依赖。
3. 执行 `npm start` 命令启动项目。
4. 使用浏览器打开链接 [http://localhost:3000/baseurlplaceholder/](http://localhost:3000/baseurlplaceholder/)

注1：Docusaurus 支持热重载（hot reload），大多数情况下可直接在启动状态修改内容而不需重启项目，甚至无需刷新浏览器页面。<br/>
注2：启动时默认使用本地 `3000` 号端口。若端口处于占用状态将无法启动，也可以自行修改默认使用的端口号。

## 如何编辑

### 内容修改

所有内容以 Markdown 形式存储于 `./docs` 目录下，直接修改 Markdown 文件内容即可。<br/>
关于 Docusaurus 支持的特性，可参考这篇[文档](https://docusaurus.io/docs/markdown-features)。

### Web 美化

Docusaurus 基于 React 框架开发，维护者也不是很懂。有兴趣的朋友可自行研究框架结构后修改。

:::warning
请勿修改 `docusaurus.config.js` 文件内的 `url` 和 `baseUrl` 两个项目。
未来将使用 Github Actions 自动替换这两个属性。
:::

## 提交修改

提交记录（commit）格式要求：

```
<TYPE>: <TITLE>.
(<CONTENTS>)
```

:::note \<TYPE\> 字段允许使用的种类和意义
Init - 初始化项目，一般不会使用。<br/>
Content - 内容修改，主要指针对 `docs` 下内容的增删操作。<br/>
Style - 样式修改，主要针对 Web 组件或页面的修改和定制操作。<br/>
Merge - 合并分支。<br/>
:::

:::note \<TITLE\> 字段
简明扼要地使用英文或中文指出本次修改的主要内容。
:::

:::note \<CONTENTS\> 字段（可选）
详细描述本次修改的内容。浅显易懂的修改就不用写了。
:::

:::warning
请尽量在本地分支修改或编写内容，提交前同一主旨的修改请换基（rebase）整理后再合并（merge）到主分支（master）上。<br/>
非开发组成员请提交合并请求（pull request）后呼叫管理员处理。
:::
