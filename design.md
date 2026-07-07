# RV2V Studio — Design System

## 设计方向：Studio Canvas

从"AI 聊天工具"变成"创作者的视频画布"。视频是主角，界面安静退后。

---

## 配色

| Token | Hex | 用途 |
|---|---|---|
| `--accent` | `#FF6B4A` | 主强调色（珊瑚橘）— 发送按钮、选中态、品牌点 |
| `--accent-light` | `#FFF0EC` | 强调色浅底 — 选中标签背景 |
| `--magic` | `#8B7AFF` | 输出/魔法色（柔紫）— 编辑结果侧标识 |
| `--magic-light` | `#F0EEFF` | 魔法色浅底 |
| `--bg` | `#F5F3F0` | 页面背景 — 暖石灰，静态，不动画 |
| `--surface` | `rgba(255,255,255,.92)` | 卡片/面板表面 |
| `--border` | `rgba(0,0,0,.06)` | 边框 — 保持半透明 |
| `--text` | `#232226` | 主文字 |
| `--text2` | `#605D59` | 次文字 |
| `--text3` | `#9C9891` | 三级文字 |
| `--video-bg` | `#1A1920` | 视频区暖炭黑 |

## 字体

```
Display: 'Space Grotesk', sans-serif — 品牌名、面板标题
Body:    'DM Sans', sans-serif — 正文、输入、标签
```

## 排版层级

| 元素 | 字号 | 字重 | 字体 |
|---|---|---|---|
| 品牌名 | 16px | 700 | Space Grotesk |
| 面板标题 | 11px + 0.8px 字距 | 600 | Space Grotesk, uppercase |
| 输入框 | 14px | 400 | DM Sans |
| 场景标签 | 12px | 500 | DM Sans |
| 历史条目 | 12px | 400 | DM Sans |
| 微型/tooltip | 10px | 400 | DM Sans |

## 砍掉

- `gradientShift` 背景渐变动画
- `breathe` 占位符呼吸动画
- `sparkle` 四芒星动画
- 大面积 `backdrop-filter:blur()` — 仅保留 header
- 场景面板灰底 `#F0F1F4` → 白底 + 阴影

## 保留

- 100vh 不滚动布局
- 双面板并排 + 底部指令栏结构
- 图片占位符倾斜卡片
- 录制 pulse 动画（功能性）
- 面板浮层弹出交互

## 记忆点

编辑结果面板顶部：渲染完成时一道极细的紫色光带短暂亮起（0.6s fade）。唯一的"魔法时刻"。
