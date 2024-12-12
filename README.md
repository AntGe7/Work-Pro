# Work - Pro

## 1.提交信息规范

提交信息需符合 [Conventional Commit](https://www.conventionalcommits.org/) 规范：

```text
<type>: <subject>
```

### Type 类型

- **feat**: 新功能
- **fix**: 修复问题
- **docs**: 文档修改
- **style**: 代码样式（不影响功能）
- **refactor**: 代码重构
- **test**: 添加或修改测试
- **chore**: 其他修改（例如构建流程）

### Subject 描述

- 简短清晰，描述本次提交的核心内容。
- **不需要以句号结尾。**

## 2.增加调式工具

- 使用 [code-inspector-plugin](https://inspector.fe-dev.cn/) 插件，增加调式工具。
- 在 `vite.config.ts` 中配置插件。

```ts
import { codeInspectorPlugin } from 'code-inspector-plugin'

export default defineConfig({
  plugins: [
    codeInspectorPlugin({
      bundler: 'vite',
    }),
  ],
})
```
