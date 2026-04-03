# 根目录论文摘要

## AutoVLA——A Vision-Language-Action Model for End-to-End Autonomous Driving with Adaptive Reasoning and Reinforcement Fine-Tuning_2025.pdf

- filename: AutoVLA——A Vision-Language-Action Model for End-to-End Autonomous Driving with Adaptive Reasoning and Reinforcement Fine-Tuning_2025.pdf
- title: AutoVLA: A Vision-Language-Action Model for End-to-End Autonomous Driving with Adaptive Reasoning and Reinforcement Fine-Tuning
- date: 2025（arXiv v1: 2025-06-16；v3: 2025-11-05）
- venue: NeurIPS 2025；arXiv:2506.13757
- 解决的问题（1～2句话）: 面向端到端自动驾驶的VLA模型，常见动作不可物理执行、推理冗长与效率低的问题；目标是统一感知—推理—规划，直接生成可执行的行动并保留必要的自适应推理。
- 设计挑战: 将语义推理与轨迹规划融入同一自回归解码过程；保证解码动作的物理可行性；避免过长的链式推理影响时延；在多数据集与open/closed-loop任务上同时取得强性能。
- 方案介绍: 统一自回归VLM解码器同时输出推理token与行动token；“物理行动tokenization”将连续轨迹离散为可逆映射的行动词表；双思维SFT训练快/慢两模式（仅轨迹 vs CoT推理+轨迹）；用GRPO进行RFT以优化奖励并缩短不必要推理；行动词表由轨迹片段聚类构建，支持直接解码可执行行动序列。
- 实验设置（简要）: 数据/基准含nuPlan、nuScenes、Waymo E2E挑战、CARLA；任务覆盖open-loop规划与closed-loop仿真；指标含PDMS（Navsim）、Waymo RFS Overall/ADE/Spotlight与运行时效率。
- 实验结果（2–4条）:
  - RFT在NAVSIM上PDMS提升约+10.6%，运行时降低约−66.8%。
  - Waymo榜单在困难场景RFS Spotlight取得领先（项目页声明，具体表格未公开）。
  - 数据扩展持续提升规划质量；结构化CoT在数据充分时更优。
- 不足和未来方向: 多数结果为定性或榜单声明、缺少完整数表；复杂场景下效率与可执行性的量化仍有限；后续将发布模型/数据并拓展评测；探索更高效推理蒸馏与长时复杂场景泛化。

## Hybrid Data Curation for Imitation Learning with Physics-Generated Trajectories.pdf

- filename: Hybrid Data Curation for Imitation Learning with Physics-Generated Trajectories.pdf
- title: Hybrid Data Curation for Imitation Learning with Physics-Generated Trajectories
- date: 2026-03-19
- venue: Applied Sciences, Vol.16(6), Article 2968；DOI:10.3390/app16062968
- 解决的问题（1～2句话）: Imitation Learning对示范质量敏感且专家数据昂贵；需在降低数据采集成本的同时，稳定训练并提升可靠控制。
- 设计挑战: 在大规模轨迹池中筛选高质量、多样且物理可行的示范；控制计算成本，避免冗余样本导致性能不稳。
- 方案介绍: 采用采样式运动规划（如RRT*）生成物理可行的合成轨迹；通过聚类提升多样性、去冗余，再以规则过滤挑选高质量示范；形成“规划+筛选”的混合数据整理管线以减轻专家数据依赖。
- 实验设置（简要）: 机械臂轨迹生成与控制任务；对比“传统过滤方法”；指标含成功率（95%CI）、路径长度、末端距离误差、关节运动幅度等。
- 实验结果（2–4条）:
  - 平均成功率约79.1%（95%CI: 74.3–83.2%）。
  - 相较传统过滤方法，路径更短、末端误差更低、关节运动更小。
  - 整体训练稳定性与数据成本得到改善。
- 不足和未来方向: 公共摘要未详述任务/平台与局限；需在更多任务与机器人上验证、分析规划偏置与复杂环境泛化；与真实数据融合及大规模聚类/过滤的算力效率需评估。

## MimicGen——A Data Generation System for Scalable Robot Learning using Human Demonstrations_2023.pdf

- filename: MimicGen——A Data Generation System for Scalable Robot Learning using Human Demonstrations_2023.pdf
- title: MimicGen: A Data Generation System for Scalable Robot Learning using Human Demonstrations
- date: 2023
- venue: CoRL 2023；arXiv:2310.17596；项目页: mimicgen.github.io
- 解决的问题（1～2句话）: 大规模、跨任务/实体的操控数据采集成本高且慢；以少量人类示范自动扩展到海量多样数据，支撑行为克隆（BC）策略训练。
- 设计挑战: 降低人工成本同时保持任务多样性与长时接触复杂任务可迁移；跨模拟器与真实场景、跨实体一致性与鲁棒性。
- 方案介绍: 用参数化任务模板与上下文自适应，将少量人类轨迹扩展为大规模合成示范；增强覆盖reset分布、对象实例、跨实体重定向、跨模拟器/真实执行；下游使用标准BC训练。
- 实验设置（简要）: 以<200人类示范生成>50,000示范，覆盖18任务（装配/厨房等），含对象与初始状态变化、跨实体（Sawyer、IIWA、UR5e）与跨模拟器/真实；指标为成功率。
- 实验结果（2–4条）:
  - 多任务BC成功率高：如Nut-and-Bolt约96%、Coffee约93%、Stack Three约91%、Kitchen约78%等。
  - 等量数据时MimicGen与人类示范性能可比（如Square 200条：79% vs 84%）。
  - 对“好/差”操作者示范生成的策略表现相近，显示管线鲁棒性。
- 不足和未来方向: 人类数据冗余与增量采集策略仍待研究；管线细节与更广领域验证需加强；未来面向更多任务族与更复杂场景做系统化评估。

## RoboAgent——Generalization and Efficiency in Robot Manipulation via Semantic Augmentations and Action Chunking_2023.pdf

- filename: RoboAgent——Generalization and Efficiency in Robot Manipulation via Semantic Augmentations and Action Chunking_2023.pdf
- title: RoboAgent: Generalization and Efficiency in Robot Manipulation via Semantic Augmentations and Action Chunking
- date: 2023（arXiv），ICRA 2024发表
- venue: ICRA 2024；arXiv:2309.01918
- 解决的问题（1～2句话）: 在有限多模态示范下训练能跨任务/场景泛化的操控agent，同时提升数据效率与鲁棒性。
- 设计挑战: 限数据下避免过拟合于偶然视觉细节；提升语言/目标条件下的稳健执行；在多技能、多场景保持泛化。
- 方案介绍: 语义增强扩充示范（改变对象/布局/扰动以提升覆盖）；将底层控制结构化为动作分块（macro-actions）提高学习效率；管线为“少量示范→语义增强→分块动作表示的BC→语言条件策略”。
- 实验设置（简要）: 约7,500示范训练单一agent；覆盖12技能、38任务变体，厨房相关多场景；指标为成功率与平均性能，对比既有方法。
- 实验结果（2–4条）:
  - 在未见场景的平均表现较既有方法提升超过40%。
  - 以同量数据实现更强泛化；覆盖12技能与38任务，显示规模化与多样性。
- 不足和未来方向: 依赖示范且任务集中在厨房域；需扩展到更广环境与任务族、结合更大数据或微调策略以提升稳健性与泛化。

## Robot Data Curation with Mutual Information Estimators_2025.pdf

- filename: Robot Data Curation with Mutual Information Estimators_2025.pdf
- title: Robot Data Curation with Mutual Information Estimators
- date: 2025
- venue: RSS 2025；arXiv:2502.08623；项目页: jhejna.github.io/demonstration-info
- 解决的问题（1～2句话）: 示范数据“多而不优”会伤害模仿学习；需无监督、逐轨迹的质量评分方法，兼顾状态多样性与动作可预测性，从离线数据中筛选高价值示范。
- 设计挑战: 低数据下准确估计互信息（MI）困难；高维连续状态/动作的密度估计不稳；常见对比/参数化MI估计器在低数据时偏差与不稳定。
- 方案介绍: 以I(S;A)为质量准则，分别训练状态/动作VAE降维，在联合潜空间用kNN-KSG估计逐样本MI贡献并平均成轨迹评分、阈值筛选（DemInf）；与不确定性、兼容性、VIP、InfoNCE、MINE等方法进行对比与消融。
- 实验设置（简要）: 仿真RoboMimic（Lift/Can/Square，3操作者×100示范，图像+状态）；真实Franka（PenInCup 60、DishRack 80，约半专家半低质）；RoboCrowd ALOHA（HiChew/TootsieRoll 40各、HersheyKiss 100半专家）；指标为下游策略成功率/任务评分与与人工标签一致性。
- 实验结果（2–4条）:
  - DemInf在多数据集上排名最佳或并列最佳；RoboMimic平均提升约5–10%，其中Can（图像）提升>10%，且Square只有DemInf能优于“用全部数据”。
  - ALOHA与Franka上，DemInf筛选优于随机50%与未筛选，在匹配数据量下表现更好。
- 不足和未来方向: 偏好低条件动作熵与独特状态可能误排；贪心筛选改变分布且未迭代重估；后续将扩展到多任务条件、Open X-Embodiment/DROID等大规模社区数据，并把整理融入在线采集界面。

