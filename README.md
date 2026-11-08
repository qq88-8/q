# test
Move this repository's GitHub Actions jobs onto instabox.

1. Run npx instabox@latest to install or update the instabox CLI and its agent skill, then follow the skill's "CI (GitHub Actions)" section. If it asks me to sign in, show me the link and code.
2. Run instabox ci. If no GitHub App install is linked, or it can't see this repository, give me the link it prints and wait until I say I've installed it.
3. On a new branch, change runs-on: ubuntu-latest to runs-on: instabox-medium in .github/workflows. Leave the steps alone.
4. Show me the diff, then push the branch and open a pull request.
5. Watch its checks with gh pr checks --watch and instabox ci, and tell me when they pass on instabox. Don't merge it.
