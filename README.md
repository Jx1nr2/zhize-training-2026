# 智泽实验室软件组新生培训 · 2026

个人培训仓库，按《软件组新生培训任务书》的题目组织源码、运行截图和学习报告。

## 个人简介

- GitHub：[@Jx1nr2](https://github.com/Jx1nr2)
- 姓名 / 专业 / 年级：待本人补充
- 学习目标与研究兴趣：待本人补充

## 任务完成清单

当前仅完成仓库初始化，下列培训任务均未验收。完成实践、补齐交付物并自检后再勾选。

- [ ] [A.1 基础环境与 AI 工具配置](A1_Base_and_AI_Tool/report%EF%BC%88%E7%94%B1%E4%BA%8E%E8%80%83%E8%AF%95%E5%92%8C%E5%A4%A7%E6%8C%91%E8%80%BD%E8%AF%AF%E4%BA%86%E4%B8%80%E4%BA%9B%E4%BA%9B%EF%BC%8C%E6%8C%81%E7%BB%AD%E6%9B%B4%E6%96%B0%E4%B8%AD%EF%BC%89.md)
- [ ] [B.1 OpenCV 基础图像处理与人脸模糊](B1_OpenCV_Basics/report.md)
- [ ] [C.1 MNIST：MLP 与 CNN 对比实验](C1_MNIST_Comparison/report.md)
- [ ] [B.2 YOLO 目标检测全流程](B2_YOLO_Detection/report.md)
- [ ] [D.1 ROS 2 基础通信与控制](D1_ROS2_Basics/report.md)
- [ ] [E.1 强化学习与具身智能导览](E1_RL_Overview/report.md)

建议学习顺序：A.1 → B.1 → C.1 → B.2 → D.1 → E.1；每周推进一项，结合实际情况调整。

## 仓库结构

```text
zhize-training-2026/
├── README.md
├── .gitignore
├── A1_Base_and_AI_Tool/
│   ├── src/
│   ├── images/
│   └── report（由于考试和大挑耽误了一些些，持续更新中）.md
├── B1_OpenCV_Basics/
│   ├── src/
│   ├── images/
│   └── report.md
├── B2_YOLO_Detection/
│   ├── src/                  # 训练、推理脚本与实际 data.yaml
│   ├── weights/              # 训练权重与获取说明
│   ├── images/
│   └── report.md
├── C1_MNIST_Comparison/
│   ├── src/
│   ├── images/
│   └── report.md
├── D1_ROS2_Basics/
│   ├── ros2_ws/
│   │   └── src/              # ROS 2 功能包源码
│   ├── images/
│   └── report.md
├── E1_RL_Overview/
│   ├── images/
│   └── report.md
└── Optional/                 # 按题号自建子目录
```

空目录通过 .gitkeep 纳入 Git 跟踪，放入真实文件后可移除占位文件。各题 report.md 为待填写提纲，不代表实验已完成。

## 提交与复现约定

1. 源码放在对应题目目录，截图放在 images/，报告统一写在 report.md。
2. 每题记录操作系统、Python / 框架版本、安装命令、运行命令、参数、数据来源和实际结果。
3. 使用有意义的提交，例如 `feat(opencv): add face blur script`、`docs(mnist): record comparison results`；随实际学习持续提交。
4. 提交前用 `git status` 和 `git diff --cached` 核对文件，不提交 API Key、虚拟环境、编译产物、缓存或大体积原始数据集。
5. 模型权重默认忽略；合规且适合提交的小文件可单独用 `git add -f <path>` 添加。较大权重可在对应目录记录下载地址、校验值及复现方式。B.2 应保留 best.pt 的获取说明。
6. 允许 AI 辅助代码与图示；必须读懂核心逻辑。心得总结、代码逻辑说明、问题回答和研究方向意向由本人独立撰写，使用真实实验记录，不代填结果。

## 开始使用

```bash
git clone https://github.com/Jx1nr2/zhize-training-2026.git
cd zhize-training-2026
git status
```

从 A.1 开始，完成相应实践后补充源码、截图和报告，再更新上面的清单。

选做任务及交付提示见 [Optional/README.md](Optional/README.md)。
