# Day4_数据与Sim2Real 论文摘要

## 19_Open_X_Embodiment.pdf
- filename: 19_Open_X_Embodiment.pdf
- title: Open X-Embodiment: Robotic Learning Datasets and RT-X Models
- date: 2023/2024
- venue: 多机构合作数据集与模型论文
- 解决的问题（1～2句话）: 构建跨机构/跨实体的大规模机器人学习数据集与统一模型，提高跨任务与跨平台的泛化能力。
- 设计挑战: 数据标准化、标注一致性、跨平台动作接口与隐私合规。
- 方案介绍: 汇聚多源数据并推出RT-X统一模型与评测协议，促进开源复现与社区协作。
- 实验设置（简要）: 多平台多任务评测；指标为成功率/泛化等。
- 实验结果（2–4条）: 在跨任务/跨实体场景显著提升泛化；推动统一生态与基准。
- 不足和未来方向: 数据质量与覆盖仍需扩大；接口与评测需持续迭代。

## 20_BridgeData.pdf
- filename: 20_BridgeData.pdf
- title: BridgeData（数据集/管线）
- date: 不详
- venue: 论文/项目
- 解决的问题（1～2句话）: 搭建桥接仿真与现实的数据采集与整理管线，缓解Sim2Real落差并提升数据质量。
- 设计挑战: 现实噪声与视觉偏移；动力学差异；标注一致性。
- 方案介绍: 统一采集与清洗流程，涵盖多视角/多任务数据，支持后续训练与评测。
- 实验设置（简要）: 典型操控/导航任务数据；指标为成功率与迁移性能。
- 实验结果（2–4条）: 数据质量提升带来更稳定训练与更好迁移。
- 不足和未来方向: 需公布更详尽数据统计与开放基准；现实闭环评测应加强。

## 24_Domain_Randomization.pdf
- filename: 24_Domain_Randomization.pdf
- title: Domain Randomization for Sim-to-Real Transfer（综述/方法）
- date: 不详
- venue: 论文/综述
- 解决的问题（1～2句话）: 利用域随机化提升从仿真到现实的视觉/感知鲁棒性，减少对精确模拟的依赖。
- 设计挑战: 随机化策略设计与覆盖；避免过度随机化影响学习收敛。
- 方案介绍: 在纹理/光照/背景/噪声等维度系统随机化；配合数据增强与风格迁移。
- 实验设置（简要）: 仿真到现实的操控/视觉任务；指标为成功率与误差。
- 实验结果（2–4条）: 显著缓解视觉域偏移，提升现实性能。
- 不足和未来方向: 动力学差异仍难；需与系统辨识与现实数据相结合。

## RoboCOIN——An Open-Sourced Bimanual Robotic Data COllection for INtegrated Manipulation.pdf
- filename: RoboCOIN——An Open-Sourced Bimanual Robotic Data COllection for INtegrated Manipulation.pdf
- title: RoboCOIN: An Open-Sourced Bimanual Robotic Data Collection for Integrated Manipulation
- date: 2025（推测）
- venue: 数据集论文/项目
- 解决的问题（1～2句话）: 面向双臂（bimanual）综合操控的数据采集与开放集，支持协作与复杂装配任务。
- 设计挑战: 双臂协调与同步标注；复杂场景下的可重复采集与安全。
- 方案介绍: 系统化采集框架与数据协议，包含多视角与动作记录，适配下游策略学习。
- 实验设置（简要）: 双臂操控任务与基准；指标为成功率与动作质量。
- 实验结果（2–4条）: 提供高质量数据支持算法评测；在复杂协作任务上验证有效性。
- 不足和未来方向: 数据规模与多样性仍需扩大；与更多平台对接与开源工具链完善。

