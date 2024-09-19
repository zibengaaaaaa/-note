#!/bin/bash

# 进入到你的 Git 仓库目录
cd /path/to/your/repo || exit

# 检测变动
if [[ $(git status --porcelain) ]]; then
    # 添加变动
    git add .

    # 提交变动
    git commit -m "Automated commit: $(date +"%Y-%m-%d %H:%M:%S")"
    
    # 推送到 GitHub
    git push origin main  # 请根据需要替换分支名称
fi