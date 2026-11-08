# test
Move this repository's GitHub Actions jobs onto instabox.

1. Run npx instabox@latest to install or update the instabox CLI and its agent skill, then follow the skill's "CI (GitHub Actions)" section. If it asks me to sign in, show me the link and code.
2. Run instabox ci. If no GitHub App install is linked, or it can't see this repository, give me the link it prints and wait until I say I've installed it.
3. On a new branch, change runs-on: ubuntu-latest to runs-on: instabox-medium in .github/workflows. Leave the steps alone.
4. Show me the diff, then push the branch and open a pull request.
5. Watch its checks with gh pr checks --watch and instabox ci, and tell me when they pass on instabox. Don't merge it.



将此仓库的 GitHub Actions 任务迁移到 instabox。

运行 `npx instabox@latest` 安装或更新 Instabox CLI 及其代理技能，然后按照技能的“CI (GitHub Actions)”部分进行操作。如果提示我登录，请提供链接和代码。
运行 instabox ci。如果没有链接 GitHub 应用安装，或者无法找到此仓库，请将它打印的链接给我，然后等待我确认安装完成。
在新分支上，将 .github/workflows 文件中的 runs-on: ubuntu-latest 改为 runs-on: instabox-medium。步骤保持不变。
请给我看看差异，然后推送分支并提交拉取请求。
使用 `gh pr checks --watch` 和 `instabox ci` 命令监控其检查结果，并在 `instabox` 检查通过时通知我。不要合并它。
