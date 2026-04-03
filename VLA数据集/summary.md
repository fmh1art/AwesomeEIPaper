# VLA数据集 论文摘要

## AgiBot World Colosseo A Large-scale Manipulation Platform.pdf
- filename: AgiBot World Colosseo A Large-scale Manipulation Platform.pdf
- title: AgiBot World Colosseo: A Large-scale Manipulation Platform
- date: 2025（推测）
- venue: 平台/数据集论文
- 解决的问题（1～2句话）: 提供大规模操控平台与数据集，支持多任务训练与评测，提升复杂场景的通用性。
- 设计挑战: 平台一致性与多任务覆盖；数据质量与接口标准化。
- 方案介绍: 统一采集/标注/评测协议，支持多视角与多实体。
- 实验设置（简要）: 多任务基准；指标为成功率与泛化。
- 实验结果（2–4条）: 在复杂任务与跨实体场景表现优。
- 不足和未来方向: 需更广数据覆盖与开放工具链。

## DROID A Large-Scale In-The-Wild.pdf
- filename: DROID A Large-Scale In-The-Wild.pdf
- title: DROID: A Large-Scale In-The-Wild Robotic Dataset
- date: 2024
- venue: 数据集论文
- 解决的问题（1～2句话）: 真实环境下的大规模示范数据集，提升策略在自然场景的鲁棒与泛化。
- 设计挑战: 真实场景采集与标注一致性；隐私与合规。
- 方案介绍: 分布式采集与质量控制；统一数据格式支持下游训练。
- 实验设置（简要）: 多任务真实环境评测；指标为成功率与泛化。
- 实验结果（2–4条）: 在真实场景训练更稳健，泛化更好。
- 不足和未来方向: 数据共享政策与跨机构扩展。

## FAST Efficient Action Tokenization for.pdf
- filename: FAST Efficient Action Tokenization for.pdf
- title: FAST: Efficient Action Tokenization for Robotic Control
- date: 不详
- venue: 论文
- 解决的问题（1～2句话）: 高效动作tokenization以支持VLA/Transformer对动作序列的可执行生成。
- 设计挑战: 动作离散化的表达力与逆映射可行性；词表规模与采样效率。
- 方案介绍: 优化动作词表与编码策略，兼顾表达力与效率。
- 实验设置（简要）: 多任务操控；指标为成功率与时延。
- 实验结果（2–4条）: 相比朴素token化更高效、更易执行。
- 不足和未来方向: 跨平台一致性与逆映射精度需验证。

## MimicGen A Data Generation System for Scalable.pdf
- filename: MimicGen A Data Generation System for Scalable.pdf
- title: MimicGen: A Data Generation System for Scalable Robot Learning using Human Demonstrations
- date: 2023
- venue: CoRL 2023；arXiv:2310.17596
- 解决的问题（1～2句话）: 少量人类示范扩展到大规模合成数据以训练BC。
- 设计挑战: 多样性与跨实体迁移；真实/模拟一致性。
- 方案介绍: 任务模板与上下文自适应；对象/reset/跨实体增强。
- 实验设置（简要）: >50K示范、18任务。
- 实验结果（2–4条）: 多任务成功率高；与人类示范等量对比性能可比。
- 不足和未来方向: 更广领域与细化管线评估。

## RH20T A Comprehensive Robotic Dataset for Learning Diverse Skills.pdf
- filename: RH20T A Comprehensive Robotic Dataset for Learning Diverse Skills.pdf
- title: RH20T: A Comprehensive Robotic Dataset for Learning Diverse Skills
- date: 不详
- venue: 数据集论文
- 解决的问题（1～2句话）: 构建覆盖多技能的机器人数据集，支持通用策略学习。
- 设计挑战: 技能多样性与标注质量；跨场景一致性。
- 方案介绍: 系统化采集多技能数据与评测协议。
- 实验设置（简要）: 多技能任务基准；指标为成功率。
- 实验结果（2–4条）: 在多技能任务上提供高质量训练与评测基座。
- 不足和未来方向: 需持续扩展与开放。

## ROBOREWARD.pdf
- filename: ROBOREWARD.pdf
- title: ROBOREWARD（奖励/评估数据集/框架）
- date: 不详
- venue: 数据集/框架论文
- 解决的问题（1～2句话）: 针对奖励学习/评估的数据与工具，提升策略训练的反馈质量。
- 设计挑战: 奖励标注一致性与可泛化；偏差控制。
- 方案介绍: 构建奖励数据与评估协议；用于RL/IL训练与分析。
- 实验设置（简要）: 多任务奖励学习评测。
- 实验结果（2–4条）: 通过更好反馈提升策略性能。
- 不足和未来方向: 奖励收集成本与一致性仍是难点。

## RoboAgent.pdf
- filename: RoboAgent.pdf
- title: RoboAgent: Generalization and Efficiency in Robot Manipulation via Semantic Augmentations and Action Chunking
- date: 2023（ICRA 2024）
- venue: ICRA 2024；arXiv:2309.01918
- 解决的问题（1～2句话）: 语义增强与动作分块提升数据效率与泛化。
- 设计挑战: 少量示范下的稳健学习。
- 方案介绍: 语义增强；分块动作；BC训练。
- 实验设置（简要）: 7,500示范、12技能、38任务。
- 实验结果（2–4条）: 未见场景平均提升>40%。
- 不足和未来方向: 扩展更广场景与平台。

## RoboMIND Benchmark on Multi-embodiment.pdf
- filename: RoboMIND Benchmark on Multi-embodiment.pdf
- title: RoboMIND: Benchmark on Multi-Embodiment Robotic Manipulation
- date: 不详
- venue: 基准/数据集论文
- 解决的问题（1～2句话）: 面向多实体操控的评测基准，促进跨平台策略的比较与发展。
- 设计挑战: 动作接口与评测一致性；多实体差异对齐。
- 方案介绍: 统一任务与指标，提供跨实体数据与评测工具。
- 实验设置（简要）: 多平台操控任务与指标。
- 实验结果（2–4条）: 促进跨实体泛化与统一评测。
- 不足和未来方向: 扩展实体与任务覆盖；开放工具链与标准。

