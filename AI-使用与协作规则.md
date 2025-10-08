# AI 使用与协作规则（ByteBot）

目标：在不依赖特定 IDE 的情况下，确保协作一致性、项目隔离与安全合规。

- 项目隔离：仅在 bytebot 目录内进行改动与运行命令，不跨项目引用或修改。
- 代码风格：遵循 .editorconfig、ESLint、Prettier 配置；保存时自动格式化。
- 类型检查：使用根级 tsconfig.json 与各 packages 的 tsconfig，保证 IDE 类型推断一致。
- 容器与环境：使用项目内 docker/ 下的 Dockerfile 与 docker-compose.*.yml；敏感信息通过环境变量或密钥管理，不得硬编码。
- 文档结构：遵循 docs 目录结构与语言分区（含 zh）；不跨项目复制或移动文档。
- 命令执行：在项目根目录执行脚本；各包遵循独立模块边界。
- UI/代理变更：涉及 UI 或代理配置改动时，在本项目内启动本地预览进行验证。
- 提示协作：.cursor 中的规则仅在本项目内生效；其他 AI/IDE 不识别时，仍以本规范为准。