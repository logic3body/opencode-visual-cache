<div align="center">
<strong>
    <h1>OpenCode Visual Cache</h1>
    实时 Token 缓存命中率 · TUI 侧边栏可视化<br>
    自适应主题色 · 自动低饱和 · 支持中/英双语
</strong>
</div>

---

## 功能

- **缓存命中率**：实时显示 `cache_read / total_input × 100%`，自适应宽度进度条
- **Token 明细**：缓存读 / 缓存写 / 未命中 / 输出，标签左对齐 · 数据右对齐
- **费用与节省**：Session 累计费用 + 缓存命中带来的费用节省
- **模型定价**：显示当前模型的输入 / 缓存读单价（从 provider 配置动态读取）
- **折叠面板**：点击标题折叠为一行，节省侧边栏空间
- **颜色自适应**：命中率 ≥85% 绿 · ≥70% 橙 · <70% 红，颜色从主题色自动去饱和
- **语言适配**：自动检测系统语言，中文环境显示中文

---

## 安装

> [!NOTE]
> 安装方式待定 —— 本喵还在研究如何发布喵~
> 发布后将更新此部分。

```jsonc
// TODO: 安装步骤
```

---

## 调试

强制英文（Windows PowerShell）：

```powershell
$env:CACHE_TUI_LANG="en"; opencode
```

---

## 兼容性

代码完全模型无关，支持所有 OpenCode 兼容的 AI 模型（DeepSeek / Claude / GPT 等）。
Token 数据和定价信息均通过 OpenCode SDK 标准接口获取。

---

## License

MIT

---

## English

### Features

- **Cache Hit Rate**: Real-time `cache_read / total_input × 100%` with adaptive-width progress bar
- **Token Breakdown**: Cache Read / Write / Miss / Output, left-aligned labels, right-aligned values
- **Cost & Savings**: Session cost + cache savings (input_rate − cache_read_rate) × cache_read
- **Model Pricing**: Current model's input / cache-read rates (from provider config)
- **Collapsible**: Click title to fold into one line
- **Adaptive Colors**: ≥85% green · ≥70% orange · <70% red, auto-desaturated from theme
- **Language**: Auto-detects system locale, switches between Chinese and English

### Installation

> [!NOTE]
> Installation method TBD — will be updated after publishing.

```jsonc
// TODO: install steps
```

### Debug

Force English:

```powershell
# Windows PowerShell
$env:CACHE_TUI_LANG="en"; opencode
```

```bash
# macOS / Linux
CACHE_TUI_LANG=en opencode
```

### Compatibility

Model-agnostic — works with all OpenCode-compatible AI models (DeepSeek / Claude / GPT etc.).
Token data and pricing are read via OpenCode SDK standard interfaces.

### License

MIT
