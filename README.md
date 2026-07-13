# Metronome — Premium Beat Keeper

> 一个精致的在线节拍器，为音乐练习和演奏提供精准的节奏参考。  
> A polished online metronome for precise rhythm reference in music practice and performance.

**[在线访问 / Live Demo](https://metronome.yororoice.top/)**

## 功能特性 / Features

### 节拍控制 / Beat Control

- **BPM 调节 / BPM Adjustment**：20–240 BPM，支持滑块拖拽、`+/-` 按钮和键盘方向键（`↑↓` 微调 1、`←→` 快调 5）
- **播放 / 停止 / Play & Stop**：使用 Web Audio API 生成精准的节拍音效，强拍频率更高（880Hz）、弱拍为 660Hz
- **指针动画 / Needle Animation**：弧形刻度盘上的指针随节拍左右摆动，强拍幅度更大（±28°），弱拍 ±22°

### 拍号 & 细分 / Time Signature & Subdivision

- **拍号 / Time Signature**：2/4、3/4、4/4、5/4、6/8、7/8
- **细分 / Subdivision**：四分音符 / Quarter、八分音符 / Eighth、三连音 / Triplet、十六分音符 / Sixteenth
- **节拍指示灯 / Beat Indicators**：底部圆点指示当前拍位，强拍圆点更大

### Tap Tempo

- 连续点击按钮按节奏打拍子，2 次以上自动计算平均 BPM
- Tap the button in rhythm; BPM is auto-calculated from 2+ taps
- 点击时按钮高亮反馈，右侧显示已点击次数

### 音量控制 / Volume

- 独立音量滑块，范围 0–100%

### 主题 & 语言 / Theme & Language

- 深色 / 浅色主题，自动跟随系统偏好
- Dark / Light theme with system preference detection
- 中 / 英 双语界面，一键切换
- Chinese / English bilingual UI with one-click toggle

### 持久化 / Persistence

- 所有设置项（BPM、拍号、细分、音量、主题、语言）自动保存到 localStorage
- All settings (BPM, time signature, subdivision, volume, theme, language) persist via localStorage

### 键盘快捷键 / Keyboard Shortcuts

| 按键 / Key | 功能 / Action |
|------------|--------------|
| `Space` | 播放 / 停止  Play / Stop |
| `↑` / `↓` | BPM ±1 |
| `←` / `→` | BPM ±5 |

## 技术栈 / Tech Stack

- 纯 HTML/CSS/JS，零依赖 / Zero dependencies
- Web Audio API 精确音频调度 / Precise audio scheduling
- SVG 弧形刻度盘 + requestAnimationFrame 动画 / SVG arc dial + rAF animation
- CSS Custom Properties 主题系统 / Theme system
- localStorage 状态持久化 / State persistence

## 目录结构 / Structure

```
beat/
├── index.html     # 主页面 / Main page
├── favicon.png    # 图标 / Icon
├── CNAME          # 自定义域名 / Custom domain
└── README.md
```
