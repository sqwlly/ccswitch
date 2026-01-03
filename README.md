# ccswitch

Claude Code 多供应商管理工具 - 支持多供应商配置、智能路由、故障转移。

## 功能特性

- **多供应商配置管理** - 支持添加/编辑/删除/启用禁用供应商
- **快速切换主供应商** - 一键切换不同的 API 供应商
- **备用供应商（故障转移）** - 设置备用供应商，主供应商故障时自动切换
- **路由模式** - 支持 primary / round_robin / smart 三种路由模式
- **速度测试** - 测试所有已启用供应商的连通性和响应速度
- **交互式菜单** - 美观的终端界面，支持键盘导航

## 安装

```bash
# 下载脚本
curl -o /usr/local/bin/ccswitch https://raw.githubusercontent.com/sqwlly/ccswitch/main/ccswitch

# 添加执行权限
chmod +x /usr/local/bin/ccswitch
```

## 使用方法

### 交互式模式

```bash
ccswitch
```

### 命令行模式

```bash
# 查看当前配置
ccswitch --current

# 列出预设供应商
ccswitch --list

# 显示帮助
ccswitch --help
```

## 预设供应商

- `official` - Anthropic 官方 API
- `bigmodel` - 智谱 GLM

## 配置文件

- `~/.claude/settings.json` - Claude 配置
- `~/.claude/providers.json` - 供应商配置

## 许可证

MIT
