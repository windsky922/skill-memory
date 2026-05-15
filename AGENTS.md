# AGENTS.md

## 角色定位

你是协助我长期开发项目的 Codex。工作时优先务实、简洁、可验证，不要做无关重构。

## 通用要求

1. 项目文档全部使用中文。
2. 每次开始工作先确认：

```powershell
Get-Location
git status --short --branch
git remote -v
```

3. 不要在错误目录执行 Git 命令。
4. 不要修改我明确排除的目录。
5. 不要硬编码密钥。
6. 不要删除历史周报、历史数据或归档文件，除非我明确要求。
7. 如果需要提交，先给我提交命令，由我自己执行。
8. 操作日志必须倒序排列，最新内容放在最上面。
9. 修改后必须说明做了什么、验证了什么、下一步建议做什么。

## GitHub Weekly Agent 特定要求

1. GitHub Trending 是热点追踪第一指标。
2. 热点项目应按一周内热度判断，不按创建时间判断。
3. Trending Top 10 至少应有 7 个进入周报候选或最终周报，除非有明确过滤原因。
4. 新增 Star 是重要筛选依据。
5. Telegram 推送发送周报链接，不发送 Markdown 全文。
6. Kimi 失败时允许降级版周报，但要记录失败原因。
7. 别人项目的 README 只保留 2-3 句中文摘要，不复制完整 README。
8. 后续开发优先建设核心能力：采集、评分、后端 API、数据库、任务系统、个性化推荐。
9. 安全检查要保留，但当前阶段不要让安全评分挤占核心功能建设。
10. 前端和数据库要逐步推进，并保留未来复杂框架扩展空间。

## 验证命令

常用验证：

```powershell
py -m unittest discover -v
py scripts\security_check.py
git diff --check
```

本地后端：

```powershell
py -m uvicorn src.api.app:app --reload
```

后端检查入口：

```text
http://127.0.0.1:8000/v1/health
http://127.0.0.1:8000/v1/jobs?limit=20
http://127.0.0.1:8000/v1/projects?limit=20
http://127.0.0.1:8000/docs
```
