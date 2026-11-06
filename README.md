# learning-embodied-ai · 具身智能学习笔记

> 基于 [curriculum-builder](https://github.com/doloveplayer/curriculum-builder) 构建的结构化具身智能课程与学习笔记。多设备同步使用，主学习环境为 Obsidian。

## 课程结构

| Phase | 主题 | 状态 |
|:-----:|------|:----:|
| 1 | 具身智能全景与基础打底 | 🔄 进行中 |
| 2 | 模仿学习与 Diffusion Policy | 📋 预览 |
| 3 | VLA 视觉-语言-动作模型 | 📋 预览 |
| 4 | Sim2Real 与部署落地 | 🔮 待细化 |

## 目录结构

```
├── knowledge/               # 知识库（Obsidian vault 根目录就打开本仓库）
│   ├── curriculum.md        # 滚动课程表（单一真相来源）
│   ├── learning-roadmap.canvas  # Canvas 可视化路线图
│   ├── _index.md            # 仪表盘
│   ├── templates/           # 笔记模板
│   └── 01-foundations/      # Phase 1 课程笔记
├── experiments/             # 动手实验
├── scripts/                 # 脚本
├── configs/                 # 配置
└── data/                    # 数据集
```

> `.claude/` 与 `.workbuddy/` 为本地工具与私有配置，不入库。

## 课程工具

本课程由 **curriculum-builder** 驱动：

- 仓库地址：<https://github.com/doloveplayer/curriculum-builder>
- 功能：自动生成课程大纲、维护滚动课程表、追踪学习进度、五层防偏机制

## 新设备同步指南

1. 克隆本仓库：

   ```bash
   git clone https://github.com/JohnSiegfried/learning-embodied-ai.git
   cd learning-embodied-ai
   ```

2. 安装 curriculum-builder skill（本地依赖，不入库）：

   ```bash
   mkdir -p .claude/skills
   git clone https://github.com/doloveplayer/curriculum-builder.git .claude/skills/curriculum-builder
   ```

3. 查看课程进度，继续学习：

   ```bash
   python .claude/skills/curriculum-builder/driver.py status
   python .claude/skills/curriculum-builder/driver.py schedule --next 3
   ```

前置要求：Python 3.10+（skill 零外部依赖）。

## 参考资料

- [Xbotics-Embodied-Guide](https://github.com/Xbotics-Embodied-AI-club/Xbotics-Embodied-Guide) — 本课程路线的蓝本
- [Modern Robotics](https://hpnicto.github.io/files/ModernRobotics.pdf) — 机器人学教材（免费）
- [LeRobot (Hugging Face)](https://github.com/huggingface/lerobot) — Phase 2/4 使用的开源框架
