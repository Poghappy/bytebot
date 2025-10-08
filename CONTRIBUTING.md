# ByteBot 贡献指南

感谢你为 ByteBot 贡献！本指南帮助你在一致的开发环境中高效协作。

## 环境与工具
- 推荐 IDE：VS Code（已提供统一设置与推荐扩展）。
- 代码风格：遵循 <.editorconfig>、ESLint、Prettier 配置。
- 类型检查：遵循根级 `tsconfig.json` 与各 `packages/*` 下的 tsconfig。
- 容器化开发：使用 `.devcontainer/devcontainer.json`，需要 Docker 环境。

## 快速开始
1. 安装依赖：在项目根目录执行对应包管理器命令（如 `npm install`）。
2. 代码检查与格式化：
   - `npm run lint`（如已配置）
   - 保存时自动格式化（VS Code 设置已开启）。
3. 构建与运行：参考 `packages/*` 以及 `docker/` 下的 `docker-compose.*.yml`。

## 提交规范
- 保持 commit 信息清晰、描述完整。
- 在提交前确保通过格式化与静态检查。
- 避免提交二进制或本地环境文件；不要提交敏感信息（密钥、Token、密码等）。

## 协作与隔离
- 项目隔离：仅在 `bytebot/` 目录内进行改动与运行命令，不跨项目引用或修改。
- 文档结构：遵循 `docs/` 目录结构与语言分区（含 `zh/`）。
- UI/代理变更：涉及 UI 或代理配置改动时，在本项目内启动本地预览进行验证。

## AI 使用与协作规则
- 若 IDE/AI 支持项目提示配置，则遵循 `.cursor/` 中的规则（仅在本项目内生效）。
- 即使某些 AI/IDE 不识别 `.cursor`，也请遵循本贡献指南的规范。
- 详见：<mcfile name="AI-使用与协作规则.md" path="/Users/zhiledeng/Pictures/GAMEBOT/bytebot/AI-使用与协作规则.md"></mcfile>

感谢你的贡献！