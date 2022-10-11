# rcy-pc

## Project setup

###将 npm 设置为淘宝镜像：

```
npm config set registry https://registry.npm.taobao.org
```

###全局安装 yarn， 如已经安装，请略过

```
npm install yarn -g
```

```
yarn install
```

### 本工程已经集成[tailwindcss](https://tailwindcss.com/)，使用详情请查阅官方文档

## IconFonts

1. 从 [iconfont](https://www.iconfont.cn/) 网站复制项目的 Font class url
2. 命令行执行 iconfont 命令更新

```shell
yarn iconfont -d <iconfont url>
```

## CSS 命名规范

**BEM** : http://getbem.com/introduction/

## Liners

**vscode 插件**

vscode 安装 eslint 插件 .vscode/setting.json 配置如下
{
// 开启自动修复
"editor.codeActionsOnSave": {
"source.fixAll": false,
"source.fixAll.eslint": true
}
}

## stylelint

vscode 安装 stylelint 插件 .vscode/setting.json 配置如下
"editor.formatOnSave": true,
"editor.defaultFormatter": "esbenp.prettier-vscode"

[prettier-vscode](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

考虑到多人协同开发为保证代码统一风格和效率问题：建议使用 vscode 编辑器并且安装 eslint 和 styleint 插件！
强烈建议保存代码的时候自动去使用 eslint 和 stylelint 格式化代码

## Commitlint

```
- feat：新功能
- fix：修补 bug
- docs：修改文档，比如 README, CHANGELOG, CONTRIBUTE 等等
- style： 不改变代码逻辑 (仅仅修改了空格、格式缩进、逗号等等)
- refactor：重构（既不修复错误也不添加功能）
- perf: 优化相关，比如提升性能、体验
- test：增加测试，包括单元测试、集成测试等
- build: 构建系统或外部依赖项的更改
- ci：自动化流程配置或脚本修改
- chore: 非 src 和 test 的修改
- revert: 恢复先前的提交

```
