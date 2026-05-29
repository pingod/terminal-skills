<p align="center">
  <img src="https://img.shields.io/badge/Claude-Skills-blueviolet?style=for-the-badge&logo=anthropic" alt="Claude Skills">
  <img src="https://img.shields.io/badge/Terminal-Focused-green?style=for-the-badge&logo=gnometerminal" alt="Terminal">
  <img src="https://img.shields.io/badge/License-Apache%202.0-blue?style=for-the-badge" alt="License">
  <img src="https://img.shields.io/badge/Skills-63+-orange?style=for-the-badge" alt="Skills Count">
</p>

<h1 align="center">🖥️ Terminal Skills</h1>

<p align="center">
  <strong>面向终端、服务器、Kubernetes、DevOps 和云计算场景的 Claude Skills 集合</strong>
</p>

<p align="center">
  <a href="#-特性">特性</a> •
  <a href="#-快速开始">快速开始</a> •
  <a href="#-技能分类">技能分类</a> •
  <a href="#-热门技能">热门技能</a> •
  <a href="#-贡献">贡献</a>
</p>

<p align="center">
  <a href="./README.md">🇺🇸 English</a>
</p>

---

## 🎯 什么是 Terminal Skills？

Terminal Skills 是一个专为终端工作流设计的 [Claude Skills](https://docs.anthropic.com/en/docs/claude-code/skills) 综合集合。每个技能都为 Claude 提供特定领域的知识和命令，涵盖系统管理、DevOps、云运维等场景。

**为什么使用 Terminal Skills？**
- 🚀 **即时专业知识** - Claude 获得特定工具和工作流的深度知识
- 📋 **实战命令** - 内置最佳实践的真实命令
- 🔧 **故障排查指南** - 包含常见问题和解决方案
- 🎓 **学习资源** - 适合初学者和资深工程师

## ✨ 特性

| 分类 | 描述 | 技能数 |
|------|------|--------|
| 🐧 **Linux** | 系统管理、文件操作、进程管理、Shell 脚本 | 6 |
| 🖧 **服务器** | Nginx、Apache、SSH、Systemd、Cron、日志分析 | 6 |
| 🗄️ **数据库** | MySQL、PostgreSQL、MongoDB、Redis、Elasticsearch、SQL 优化 | 6 |
| ☸️ **Kubernetes** | kubectl、部署、服务、Helm、故障排查 | 7 |
| 🐳 **Docker** | 容器操作、镜像、Compose、网络、Dockerfile | 5 |
| ☁️ **云服务 CLI** | AWS CLI、Azure CLI、Google Cloud、阿里云 | 4 |
| 🔧 **DevOps** | Git 高级、Ansible、Terraform、CI/CD、监控 | 5 |
| 🌐 **网络** | TCP/IP、DNS、VPN、代理、负载均衡、流量分析 | 6 |
| 💾 **备份** | rsync、tar、快照、云备份、灾难恢复 | 6 |
| 🔒 **安全** | 防火墙、SSL/TLS、审计、系统加固 | 4 |
| 📊 **性能** | 基准测试、性能分析、调优、故障排查 | 4 |
| 🦀 **OpenClaw** | 安装部署、配置管理、问题排查、运维修复 | 4 |

**总计：63 个技能**

## 🚀 快速开始

### 安装

```bash
git clone https://github.com/your-username/terminal-skills.git
cd terminal-skills
```

### 在 Claude Code 中使用

1. 将所需技能文件夹复制到 Claude skills 目录：
   ```bash
   # 示例：添加 kubectl-basics 技能
   cp -r kubernetes/kubectl-basics ~/.claude/skills/
   ```

2. 或直接在项目中引用技能：
   ```bash
   # 添加到项目的 .claude/skills 目录
   cp -r linux/file-operations ./your-project/.claude/skills/
   ```

3. Claude 会在相关场景自动加载和使用技能

### 技能结构

每个技能遵循一致的结构：

```
skill-name/
├── SKILL.md          # 主技能文件，包含指令和命令
├── examples/         # 使用示例（可选）
├── scripts/          # 辅助脚本（可选）
└── resources/        # 额外参考资料（可选）
```

### SKILL.md 格式

```yaml
---
name: skill-name
description: 简短描述
version: 1.0.0
author: contributor-name
tags: [tag1, tag2, tag3]
---

# 技能标题

## 概述
技能用途和使用场景。

## 核心命令
带说明的基础命令。

## 常见场景
带步骤指南的实际用例。

## 故障排查
常见问题和解决方案。
```

## 📂 技能分类

### 🐧 Linux 系统管理

| 技能 | 描述 |
|------|------|
| [file-operations](./linux/file-operations) | 文件和目录操作、find、权限 |
| [process-management](./linux/process-management) | 进程监控、信号、作业控制 |
| [user-permissions](./linux/user-permissions) | 用户管理、sudo、ACL |
| [network-tools](./linux/network-tools) | 网络诊断、netstat、ss、ip |
| [system-admin](./linux/system-admin) | 系统监控、资源管理 |
| [shell-scripting](./linux/shell-scripting) | Bash 脚本、自动化 |

### 🖧 服务器运维

| 技能 | 描述 |
|------|------|
| [nginx](./server/nginx) | Nginx 配置、虚拟主机、SSL |
| [apache](./server/apache) | Apache httpd 配置和管理 |
| [ssh](./server/ssh) | SSH 配置、密钥、隧道 |
| [systemd](./server/systemd) | 服务管理、单元、journalctl |
| [cron](./server/cron) | 定时任务、crontab |
| [log-analysis](./server/log-analysis) | 日志解析、分析、监控 |

### 🗄️ 数据库管理

| 技能 | 描述 |
|------|------|
| [mysql](./database/mysql) | MySQL 管理、查询、备份 |
| [postgresql](./database/postgresql) | PostgreSQL 管理、psql、复制 |
| [mongodb](./database/mongodb) | MongoDB 操作、聚合、分片 |
| [redis](./database/redis) | Redis 命令、持久化、集群 |
| [elasticsearch](./database/elasticsearch) | Elasticsearch 查询、索引、集群 |
| [sql-optimization](./database/sql-optimization) | 查询优化、索引、explain |

### ☸️ Kubernetes

| 技能 | 描述 |
|------|------|
| [kubectl-basics](./kubernetes/kubectl-basics) | kubectl 基础命令 |
| [pod-management](./kubernetes/pod-management) | Pod 生命周期、调试 |
| [deployment](./kubernetes/deployment) | 部署、滚动更新、扩缩容 |
| [service-ingress](./kubernetes/service-ingress) | 服务、Ingress、网络 |
| [configmap-secret](./kubernetes/configmap-secret) | 配置管理 |
| [helm](./kubernetes/helm) | Helm charts、发布 |
| [troubleshooting](./kubernetes/troubleshooting) | K8s 调试和诊断 |

### 🐳 Docker

| 技能 | 描述 |
|------|------|
| [container-ops](./docker/container-ops) | 容器生命周期管理 |
| [image-management](./docker/image-management) | 镜像构建、标签、仓库 |
| [dockerfile](./docker/dockerfile) | Dockerfile 最佳实践 |
| [compose](./docker/compose) | Docker Compose 多容器应用 |
| [networking](./docker/networking) | Docker 网络、桥接、overlay |

### ☁️ 云服务 CLI

| 技能 | 描述 |
|------|------|
| [aws-cli](./cloud-cli/aws-cli) | AWS CLI：EC2、S3、IAM 等 |
| [azure-cli](./cloud-cli/azure-cli) | Azure CLI 操作 |
| [gcloud](./cloud-cli/gcloud) | Google Cloud CLI |
| [aliyun-cli](./cloud-cli/aliyun-cli) | 阿里云 CLI |

### 🔧 DevOps 工具

| 技能 | 描述 |
|------|------|
| [git-advanced](./devops/git-advanced) | Git 高级工作流、变基 |
| [ansible](./devops/ansible) | Ansible playbooks、inventory |
| [terraform](./devops/terraform) | 基础设施即代码 |
| [ci-cd](./devops/ci-cd) | CI/CD 流水线、GitHub Actions |
| [monitoring](./devops/monitoring) | Prometheus、Grafana、告警 |

### 🌐 网络

| 技能 | 描述 |
|------|------|
| [tcp-ip](./network/tcp-ip) | TCP/IP 基础、故障排查 |
| [dns](./network/dns) | DNS 配置、dig、nslookup |
| [vpn](./network/vpn) | VPN 设置和管理 |
| [proxy](./network/proxy) | 代理服务器、反向代理 |
| [load-balancer](./network/load-balancer) | 负载均衡策略 |
| [traffic-analysis](./network/traffic-analysis) | tcpdump、Wireshark、抓包分析 |

### 💾 备份与恢复

| 技能 | 描述 |
|------|------|
| [rsync](./backup/rsync) | rsync 文件同步 |
| [tar-compression](./backup/tar-compression) | 归档和压缩 |
| [snapshot](./backup/snapshot) | 文件系统快照 |
| [cloud-backup](./backup/cloud-backup) | 云备份策略 |
| [backup-strategy](./backup/backup-strategy) | 备份规划和策略 |
| [disaster-recovery](./backup/disaster-recovery) | 灾难恢复规划和执行 |

### 🔒 安全

| 技能 | 描述 |
|------|------|
| [firewall](./security/firewall) | iptables、firewalld、ufw |
| [ssl-tls](./security/ssl-tls) | SSL/TLS 证书、Let's Encrypt |
| [audit](./security/audit) | 安全审计、合规 |
| [hardening](./security/hardening) | 系统加固最佳实践 |

### 📊 性能

| 技能 | 描述 |
|------|------|
| [benchmarking](./performance/benchmarking) | 性能基准测试工具 |
| [profiling](./performance/profiling) | 应用性能分析 |
| [tuning](./performance/tuning) | 系统和应用调优 |
| [troubleshooting](./performance/troubleshooting) | 性能问题诊断 |

### 🦀 OpenClaw

| 技能 | 描述 |
|------|------|
| [installation](./openclaw/installation) | OpenClaw 安装与部署 |
| [configuration](./openclaw/configuration) | 配置管理与调优 |
| [troubleshooting](./openclaw/troubleshooting) | 问题排查与诊断 |
| [maintenance](./openclaw/maintenance) | 运维与故障修复 |

## 🎯 热门技能

### kubectl-basics
```bash
# 快速查看 Pod 状态
kubectl get pods -o wide

# 进入容器调试
kubectl exec -it pod-name -- /bin/bash

# 查看最近日志
kubectl logs pod-name --tail=100
```

### mysql
```bash
# 数据库备份
mysqldump -u root -p database > backup.sql

# 查看慢查询
SHOW VARIABLES LIKE 'slow_query%';

# 恢复数据库
mysql -u root -p database < backup.sql
```

### rsync
```bash
# 带进度的增量备份
rsync -avzP --delete source/ dest/

# 通过 SSH 远程同步
rsync -avz -e ssh /local/path user@remote:/remote/path
```

### docker container-ops
```bash
# 带资源限制运行容器
docker run -d --name app --memory=512m --cpus=1 nginx

# 实时查看容器日志
docker logs -f container_name

# 进入运行中的容器
docker exec -it container_name /bin/bash
```

## 🤝 贡献

欢迎贡献！请查看 [贡献指南](./CONTRIBUTING.md) 了解详情。

**快速贡献步骤：**

1. Fork 仓库
2. 在适当的分类下创建新技能文件夹
3. 按照模板编写 `SKILL.md`
4. 提交 Pull Request

**什么是好的技能？**
- ✅ 清晰、经过测试的命令
- ✅ 真实场景用例
- ✅ 故障排查部分
- ✅ 正确的 frontmatter 元数据

## 📄 许可证

本项目采用 [Apache License 2.0](./LICENSE) 许可证。

## 🔗 相关资源

- [Claude Skills 文档](https://docs.anthropic.com/en/docs/claude-code/skills)
- [awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills) - Claude Skills 精选列表
- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) - Claude Code 文档

## 🌟 Star 历史

如果这个项目对你有帮助，请给个 ⭐ Star！

---

<p align="center">
  为 DevOps 社区用 ❤️ 制作
</p>
