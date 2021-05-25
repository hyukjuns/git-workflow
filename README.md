# Git Flow
### Initialize
```bash
echo "# TEST" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin <REPO_URL>
git push -u origin main
```
```bash
git clone <REPO_URL>
```
### Branch
```bash
git branch # git branch 목록 확인
git branch -b <NEW_BRANCHNAME>
git checkout <NEW_BRANCHNAME>
git add .
git commit -m "MESSAGE"
git push --set-upstream origin <NEW_BRANCHNAME>
```
git 에서 remote branch delete 하는 방법.
```bash
방법 1.
git push origin --delete <BRANCH_NAME>

방법 2.
git branch -d <BRANCH_NAME>
git push origin <BRANCH_NAME>
```
### Pull Request(PR) & Merge
```
1. Push To Personal Branch
2. Pull Request
3. Approve
4. Merge to Main Branch
```
### Main to Branch
```
git checkout <BRANCH_NAME>
git pull origin main(or master)
```
### git login pass
- github: username:password
- azure devops git: username:PAT(Personal Access Token)
```
1. vi ~/.git-credentials
https://<USERNAME>:<PASSWORD or PAT_TOKEN>@dev.azure.com
2. git config --global credential.helper store
```