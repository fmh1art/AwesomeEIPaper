# VLA数据准备技术论文 论文摘要

## AgiBot-World_Large-Scale_Dataset_2025.pdf
- filename: AgiBot-World_Large-Scale_Dataset_2025.pdf
- title: AgiBot-World: Large-Scale Dataset for Robotic Manipulation
- date: 2025（推测）
- venue: 数据集论文/项目
- 解决的问题（1～2句话）: 提供大规模多任务操控数据集，支持VLA/BC/RL等训练，提升跨任务与复杂场景的泛化。
- 设计挑战: 多源数据一致性与高质量标注；跨平台动作接口；隐私与合规。
- 方案介绍: 统一采集与标注协议，覆盖多视角/对象/任务；面向下游策略与评测开放。
- 实验设置（简要）: 多任务基准与跨实体评测；指标为成功率与泛化。
- 实验结果（2–4条）: 展现数据规模对性能的正向提升；在复杂任务上优于小规模数据训练。
- 不足和未来方向: 需更广实体接入与持续数据更新；开放工具链完善。

## AutoVLA——A Vision-Language-Action Model for End-to-End Autonomous Driving with Adaptive Reasoning and Reinforcement Fine-Tuning_2025.pdf
- filename: AutoVLA——A Vision-Language-Action Model for End-to-End Autonomous Driving with Adaptive Reasoning and Reinforcement Fine-Tuning_2025.pdf
- title: AutoVLA: A Vision-Language-Action Model for End-to-End Autonomous Driving with Adaptive Reasoning and Reinforcement Fine-Tuning
- date: 2025
- venue: NeurIPS 2025；arXiv:2506.13757
- 解决的问题（1～2句话）: 端到端驾驶中统一视觉—语言—行动并保证动作可执行与推理效率。
- 设计挑战: 动作token物理可行性；推理—规划统一解码；效率与性能兼顾。
- 方案介绍: 统一自回归解码器、物理行动词表、SFT双模式与GRPO强化微调。
- 实验设置（简要）: nuPlan/nuScenes/Waymo/CARLA；PDMS、RFS、ADE等。
- 实验结果（2–4条）: PDMS约+10.6%，运行时约−66.8%；困难场景榜单领先。
- 不足和未来方向: 结果表格有限；复杂场景量化不足；后续开放与更广评测。

## DROID_Distributed_Data_Collection_2024.pdf
- filename: DROID_Distributed_Data_Collection_2024.pdf
- title: DROID: Distributed Data Collection for Robotic Manipulation
- date: 2024
- venue: 数据采集平台论文
- 解决的问题（1～2句话）: 构建分布式、规模化的真实示范采集平台，降低成本并提升多样性。
- 设计挑战: 标注一致性与数据质量；设备异构与同步；隐私合规。
- 方案介绍: 云—边协同采集、统一协议与质量控制；面向下游策略的可复用格式。
- 实验设置（简要）: 多任务真实示范；指标为成功率与数据覆盖。
- 实验结果（2–4条）: 显著提升采集效率与数据多样性；促进跨机构协作。
- 不足和未来方向: 平台维护与质量监控成本；开放数据共享政策。

## Hybrid Data Curation for Imitation Learning with Physics-Generated Trajectories.pdf
- filename: Hybrid Data Curation for Imitation Learning with Physics-Generated Trajectories.pdf
- title: Hybrid Data Curation for Imitation Learning with Physics-Generated Trajectories
- date: 2026-03-19
- venue: Applied Sciences, Vol.16(6), 2968；DOI:10.3390/app16062968
- 解决的问题（1～2句话）: 以规划生成+聚类/规则过滤的混合管线，降低专家示范成本并稳定训练。
- 设计挑战: 高质量筛选与多样性；计算成本控制。
- 方案介绍: 规划（如RRT*）生成、聚类去冗余与规则过滤；形成混合整理管线。
- 实验设置（简要）: 机械臂轨迹任务；成功率/路径长度/末端误差等。
- 实验结果（2–4条）: 平均成功率约79.1%（95%CI: 74.3–83.2%）；路径更短、误差更低。
- 不足和未来方向: 更广任务验证与算力效率评估；与真实数据融合。

## MimicGen——A Data Generation System for Scalable Robot Learning using Human Demonstrations_2023.pdf
- filename: MimicGen——A Data Generation System for Scalable Robot Learning using Human Demonstrations_2023.pdf
- title: MimicGen: A Data Generation System for Scalable Robot Learning using Human Demonstrations
- date: 2023
- venue: CoRL 2023；arXiv:2310.17596
- 解决的问题（1～2句话）: 以少量人类示范自动生成海量多样数据，支撑BC训练。
- 设计挑战: 跨任务/实体/模拟器与真实的自适应生成；长时复杂任务覆盖。
- 方案介绍: 参数化任务模板与上下文自适应；增强reset分布/对象实例/跨实体重定向/跨模拟器—真实。
- 实验设置（简要）: <200人类→>50K示范、18任务；指标为成功率。
- 实验结果（2–4条）: 多任务成功率高（如Nut-and-Bolt≈96%、Coffee≈93%等）；等量数据下与人类示范性能可比。
- 不足和未来方向: 数据冗余与增量采集策略研究；更广领域系统化评估。

## ObjectVLA_Cross-Modal_Alignment_2025.pdf
- filename: ObjectVLA_Cross-Modal_Alignment_2025.pdf
- title: ObjectVLA: Cross-Modal Alignment for Vision-Language-Action
- date: 2025（推测）
- venue: 论文
- 解决的问题（1～2句话）: 面向对象级别的跨模态对齐，提升指令到可执行行动的精度与可解释性。
- 设计挑战: 对象提取与指令对齐；动作映射与物理约束。
- 方案介绍: 引入对象级对齐模块与动作表达，加强语言—视觉—行动的对应关系。
- 实验设置（简要）: 多任务操控；指标为成功率与对齐精度。
- 实验结果（2–4条）: 相比无对象对齐基线表现更优。
- 不足和未来方向: 对象检测/跟踪误差影响；复杂场景扩展。

## RoboAgent——Generalization and Efficiency in Robot Manipulation via Semantic Augmentations and Action Chunking_2023.pdf
- filename: RoboAgent——Generalization and Efficiency in Robot Manipulation via Semantic Augmentations and Action Chunking_2023.pdf
- title: RoboAgent: Generalization and Efficiency in Robot Manipulation via Semantic Augmentations and Action Chunking
- date: 2023（ICRA 2024）
- venue: ICRA 2024；arXiv:2309.01918
- 解决的问题（1～2句话）: 通过语义增强与动作分块提升数据效率与未见场景泛化。
- 设计挑战: 少量示范下的稳健学习；语言条件执行。
- 方案介绍: 语义增强扩充示范；分块动作表示；BC训练语言条件策略。
- 实验设置（简要）: 约7,500示范、12技能、38任务变体。
- 实验结果（2–4条）: 未见场景平均提升>40%。
- 不足和未来方向: 厨房域偏重；需扩展到更广任务与平台。

## Robot Data Curation with Mutual Information Estimators_2025.pdf
- filename: Robot Data Curation with Mutual Information Estimators_2025.pdf
- title: Robot Data Curation with Mutual Information Estimators
- date: 2025
- venue: RSS 2025；arXiv:2502.08623
- 解决的问题（1～2句话）: 用互信息估计对示范逐轨迹评分，筛选高价值数据以改进下游策略。
- 设计挑战: 低数据下MI估计不稳；高维连续变量密度估计困难。
- 方案介绍: 状态/动作VAE降维；KSG估计逐样本MI贡献，阈值筛选（DemInf）。
- 实验设置（简要）: RoboMimic/Franka/ALOHA多数据集；成功率与任务评分。
- 实验结果（2–4条）: 平均提升≈5–10%，Can（图像）>10%；Square仅DemInf优于全部数据训练。
- 不足和未来方向: 对低条件熵/独特状态偏好会误排；需迭代重估与大规模扩展。

## Scizor_Self-Supervised_Data_Curation_2025.pdf
- filename: Scizor_Self-Supervised_Data_Curation_2025.pdf
- title: Scizor: Self-Supervised Data Curation for Robotics
- date: 2025（推测）
- venue: 论文
- 解决的问题（1～2句话）: 自监督评分/过滤提升机器人数据集质量，降低人工标注与专家依赖。
- 设计挑战: 无监督评分稳定性；与任务相关性。
- 方案介绍: 自监督表示学习+质量度量，自动剔除低质/冗余样本。
- 实验设置（简要）: 多任务数据集；指标为下游成功率。
- 实验结果（2–4条）: 相比随机/简单过滤取得更好下游性能。
- 不足和未来方向: 评分与任务耦合需加强；现实部署与规模化评估。

## UrbanNav_Robot-Compatible_Data_Filtering_2025.pdf
- filename: UrbanNav_Robot-Compatible_Data_Filtering_2025.pdf
- title: UrbanNav: Robot-Compatible Data Filtering for Urban Navigation
- date: 2025（推测）
- venue: 论文/项目
- 解决的问题（1～2句话）: 城市导航场景的数据过滤与质量控制，提升下游规划/控制的可靠性。
- 设计挑战: 城市场景噪声与长尾；与导航指标对齐。
- 方案介绍: 基于规则/学习的过滤器，剔除不合格或不可执行样本，面向导航策略训练。
- 实验设置（简要）: 城市导航数据与评测；指标为规划质量与安全性。
- 实验结果（2–4条）: 过滤后训练更稳定、指标更优。
- 不足和未来方向: 与真实车载系统接口与闭环验证需加强；跨城市泛化。

