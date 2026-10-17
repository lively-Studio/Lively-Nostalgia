# Lively-Nostalgia · 灵动怀旧

> 怀旧风格 Minecraft 光影 · 高饱和 · 暖色调 · 明亮通透

---

## 项目简介

**Lively-Nostalgia** 是一套参考 Complementary Reimagined r5 的 Minecraft Java 版光影包，专为怀旧视觉风格设计。

设计理念：

> *"用高饱和的暖色调与明亮的画面，还原记忆中那份温暖的 Minecraft 光影"*

---

## 核心特性

### 色彩 & 风格
- **怀旧色调映射**：饱和度 1.30 · 对比度 0.90 · 曝光 1.10
- **增强色彩模拟**（COLOR_LIGHT_MODE 2）：发光矿石全开 + 自发光方块 + 光色时段曲线
- **暖色清晨/傍晚**：清晨光照偏红 (R1.10)，大气偏蓝 (B0.95)，营造温暖晨光
- **冷色夜晚**：夜晚光照偏蓝 (B1.30)，大气偏蓝 (B1.20)，月色清冷
- **雨天氛围**：雨天光照微偏冷 (R0.90/G0.95/B1.10)，保持沉稳基调

### 光照 & 大气
- **柔和泛光**：BLOOM_STRENGTH 0.04，低强度辉光避免过曝
- **大气雾**：强度 0.65 · 距离 160m，通透远景
- **洞穴光照**：CAVE_LIGHTING 20，保留洞穴神秘感
- **阴影亮度**：AMBIENT_MULT 140，明亮阴影细节

### 兼容性
- **Apple Silicon 专属色彩模拟**：Mac 上完美运行
- **全中文界面** · 零依赖 · 开箱即用

---

## 关键参数

| 参数 | 值 | 说明 |
|------|-----|------|
| SHADER_STYLE | 3 | Nostalgia 视觉风格 |
| COLOR_LIGHT_MODE | 2 | 增强色彩模拟（Mac 兼容） |
| TM_EXPOSURE | 1.10 | 整体亮度 |
| TM_CONTRAST | 0.90 | 柔和对 |
| T_SATURATION | 1.30 | 高饱和度 |
| BLOOM_STRENGTH | 0.04 | 轻微泛光 |
| ATM_FOG_MULT | 0.65 | 轻雾 |
| CAVE_LIGHTING | 20 | 洞穴暗调 |
| AMBIENT_MULT | 140 | 明亮阴影 |

---

## 快速开始

### 安装

1. 下载 `Lively-Nostalgia-Shader.zip`
2. 放入 `.minecraft/shaderpacks/`（或你的 Fabric 实例目录）
3. 在 Iris / OptiFine 设置中选择 "Lively-Nostalgia"
4. 推荐搭配原版或暖色系资源包使用

### 推荐设置

| 设置项 | 推荐值 | 说明 |
|--------|--------|------|
| 模拟色彩光照 | 增强色彩 | 最佳怀旧色彩表现 |
| 视觉风格 | Nostalgia | 自动应用怀旧参数 |
| 泛光 | 开启 | 配合低强度泛光柔和画面 |
| 实时阴影 | 高或以上 | 最佳阴影效果 |

---

## 开发信息

### 技术栈
- **基础架构**：Complementary Reimagined r5
- **GLSL 版本**：`#version 130`（macOS ARM 兼容）
- **包装格式**：`shaders/` 前缀 zip

### macOS 注意事项
- `COLORED_LIGHTING`（彩色光源）在 Mac 上不可用，已用 `COLOR_LIGHT_MODE` 替代
- 打包时必须保持 `shaders/` 目录结构前缀

---

## 许可

GNU General Public License v3.0 · [github.com/lively-Studio](https://github.com/lively-Studio/Lively-Nostalgia)

---

**Lively-Nostalgia · 灵动怀旧** — Lively Studio (「零」影制作组) 出品 — 重温记忆中那束温暖的光