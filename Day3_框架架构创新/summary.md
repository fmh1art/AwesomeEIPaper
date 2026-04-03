# Day3_框架架构创新 论文摘要

## 13_PaLM_E.pdf
- filename: 13_PaLM_E.pdf
- title: PaLM-E: An Embodied Multimodal Language Model
- date: 2023
- venue: Google 论文
- 解决的问题（1～2句话）: 将大型语言模型与多模态感知耦合，直接在机器人与环境任务中进行指令理解与行动规划。
- 设计挑战: 视觉/语言/动作多模态对齐；长时任务推理与可执行性。
- 方案介绍: 以PaLM为核心加入视觉与传感输入，端到端产生行动或中间指令；支持工具调用与层次化策略。
- 实验设置（简要）: 机器人操控/导航任务；指标为成功率与泛化。
- 实验结果（2–4条）: 在多任务上表现优于纯语言或纯视觉模型；展现零样本指令理解潜力。
- 不足和未来方向: 低层控制与安全策略仍需强化；多模态鲁棒性待提升。

## 14_Gato_Generalist_Agent.pdf
- filename: 14_Gato_Generalist_Agent.pdf
- title: Gato: A Generalist Agent
- date: 2022
- venue: DeepMind 论文
- 解决的问题（1～2句话）: 训练单一Transformer处理多种任务（语言、视觉、控制），探索“通才agent”的统一建模。
- 设计挑战: 多任务分布/尺度的统一表示；动作与文本联合建模。
- 方案介绍: 将不同任务的数据统一为序列输入输出；用单一模型进行跨领域训练与推理。
- 实验设置（简要）: 覆盖NLP、视觉、机器人等；指标按任务定义。
- 实验结果（2–4条）: 在多领域实现可用性能，验证统一架构的可行性。
- 不足和未来方向: 任务专精与稳定性有限；需要更大规模与更精细动作表示。

## 15_SayCan_Affordances.pdf
- filename: 15_SayCan_Affordances.pdf
- title: SayCan: Grounding Language in Affordances to Determine What to Do
- date: 2022
- venue: Google 论文
- 解决的问题（1～2句话）: 将LLM的语言规划与环境可供性（affordances）结合，以决定可执行的机器人任务步骤。
- 设计挑战: 语言计划的可执行性与环境约束对齐。
- 方案介绍: LLM提出候选步骤，affordance模型评估可行性并筛选执行；闭环迭代。
- 实验设置（简要）: 家居任务执行；指标为成功率与安全性。
- 实验结果（2–4条）: 显著提升可执行性与成功率，减少无效尝试。
- 不足和未来方向: 依赖可供性模型质量；复杂环境知识仍有限。

## 16_VoxPoser_3D_Value_Maps.pdf
- filename: 16_VoxPoser_3D_Value_Maps.pdf
- title: VoxPoser: Composable 3D Value Maps for Robotic Manipulation
- date: 2023
- venue: 论文
- 解决的问题（1～2句话）: 将语言指令解析为3D价值图以进行可组合的操控规划。
- 设计挑战: 语言—空间表示对齐；价值图的可组合与泛化。
- 方案介绍: 从语言生成目标与约束的空间价值图，结合多图实现复杂任务分解。
- 实验设置（简要）: 真实操控与仿真评测；指标为成功率。
- 实验结果（2–4条）: 在复杂分解任务中成功率提高；具可解释空间表示。
- 不足和未来方向: 复杂场景3D理解仍难；与低层控制耦合需要优化。

## 17_Diffusion_Policy.pdf
- filename: 17_Diffusion_Policy.pdf
- title: Diffusion Policy: Visuomotor Policy Learning via Diffusion Models
- date: 2023
- venue: 论文
- 解决的问题（1～2句话）: 用扩散模型学习视觉—动作的条件分布，提升操控策略的生成质量与稳定性。
- 设计挑战: 高维视觉条件下的动作分布建模；采样效率。
- 方案介绍: 条件扩散生成动作序列；结合BC与分布建模提升鲁棒。
- 实验设置（简要）: 仿真与真实操控任务；指标为成功率。
- 实验结果（2–4条）: 相比传统BC在复杂任务上更稳定，成功率更高。
- 不足和未来方向: 采样时延与效率待优化；与VLA/LLM融合空间广阔。

## Emu3 Next-Token Prediction is All You Need.pdf
- filename: Emu3 Next-Token Prediction is All You Need.pdf
- title: Emu3: Next-Token Prediction is All You Need（多模态）
- date: 2024/2025
- venue: 论文/技术报告
- 解决的问题（1～2句话）: 强调统一的“下一token预测”范式可覆盖多模态推理与生成，简化训练与推理管线。
- 设计挑战: 跨模态统一词表与对齐；长序列推理效率。
- 方案介绍: 以单一自回归框架处理图文/音频等；数据混合与指令调优。
- 实验设置（简要）: 多模态基准评测。
- 实验结果（2–4条）: 在多模态任务中展现竞争力；管线更统一。
- 不足和未来方向: 动作/物理约束未直接覆盖；实际部署需进一步工程化。

## LLaMA Open and Efficient Foundation Language Models.pdf
- filename: LLaMA Open and Efficient Foundation Language Models.pdf
- title: LLaMA: Open and Efficient Foundation Language Models
- date: 2023
- venue: Meta AI 论文
- 解决的问题（1～2句话）: 高效训练的大型语言模型，兼顾性能与资源可用性，为下游与多模态提供基座。
- 设计挑战: 数据质量与规模；训练稳定性；开放许可。
- 方案介绍: 训练配方、模型结构与评测；开放研究使用。
- 实验设置（简要）: 标准NLP基准。
- 实验结果（2–4条）: 在多基准具竞争力；资源效率更优。
- 不足和未来方向: 安全与长时能力需后续工作；多模态扩展待完善。

## The Llama 3 Herd of Models.pdf
- filename: The Llama 3 Herd of Models.pdf
- title: The Llama 3 Herd of Models
- date: 2024
- venue: Meta 技术报告
- 解决的问题（1～2句话）: 发布新一代Llama 3模型族，提升推理、编程与对话能力，并优化训练数据与安全。
- 设计挑战: 训练数据质量与对齐；模型族规模管理。
- 方案介绍: 统一训练与对齐流程；安全评估与红队测试；开源生态支持。
- 实验设置（简要）: 多维NLP与对话评测。
- 实验结果（2–4条）: 在多数基准领先或具竞争力；对话安全与实用性提升。
- 不足和未来方向: 工具使用与长时/多步推理仍有空间；多模态版本扩展。

## VOYAGER An Open-Ended Embodied Agent with Large Language Models.pdf
- filename: VOYAGER An Open-Ended Embodied Agent with Large Language Models.pdf
- title: VOYAGER: An Open-Ended Embodied Agent with Large Language Models
- date: 2023
- venue: 论文/项目
- 解决的问题（1～2句话）: 在开放世界（如Minecraft）中利用LLM进行自我探索、技能库积累与任务解决，构建开放式Embodied agent。
- 设计挑战: 开放世界任务定义与自监督学习；技能复用与记忆管理。
- 方案介绍: 任务自动生成/评估、技能抽取与库管理、LLM驱动规划与执行的闭环框架。
- 实验设置（简要）: Minecraft等开放世界环境；指标为进度与技能掌握。
- 实验结果（2–4条）: 展现长期自主探索与技能成长能力；在开放任务上优于基线。
- 不足和未来方向: 安全与失败恢复策略不足；现实场景迁移仍具挑战。

