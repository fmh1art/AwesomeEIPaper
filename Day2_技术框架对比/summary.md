# Day2_技术框架对比 论文摘要

## 00_LLaMA_Foundation_Model.pdf
- filename: 00_LLaMA_Foundation_Model.pdf
- title: LLaMA: Open and Efficient Foundation Language Models（纲要/资料）
- date: 2023
- venue: Meta AI 技术报告/论文
- 解决的问题（1～2句话）: 通过高效训练策略与数据整理，构建参数规模跨度大的通用语言模型，为下游任务与多模态扩展提供基础。
- 设计挑战: 训练数据质量与覆盖；计算效率与稳定性；对齐与安全。
- 方案介绍: 分层参数规模与训练配方；高质量语料清洗；开放研究使用协议；为多模态与下游适配提供基座。
- 实验设置（简要）: 语言任务基准评测（推理、理解、知识问答等）。
- 实验结果（2–4条）: 在广泛NLP基准上表现强劲；较同规模模型具更优效率与性能平衡。
- 不足和未来方向: 数据透明与开源度受限于许可证；多模态与工具使用需后续扩展。

## 01_Llama2_Chat_Models.pdf
- filename: 01_Llama2_Chat_Models.pdf
- title: Llama 2: Open Foundation and Fine-Tuned Chat Models（Chat模型）
- date: 2023
- venue: Meta AI 技术报告
- 解决的问题（1～2句话）: 构建开源可商用的Chat模型，通过SFT与RLHF提升对话安全与实用性。
- 设计挑战: 安全对齐、指令遵循与有害内容规避；保持通用能力。
- 方案介绍: 指令微调+人类反馈强化（RLHF）；安全基线与拒答策略；评测覆盖实用对话场景。
- 实验设置（简要）: 多维度对话/安全基准评测。
- 实验结果（2–4条）: 对话质量与安全性优于前代开源模型；在多数评测中具竞争力。
- 不足和未来方向: 对齐代价高；跨领域工具使用与长时互动需强化。

## 07_RT1_Robotics_Transformer.pdf
- filename: 07_RT1_Robotics_Transformer.pdf
- title: RT-1: Robotics Transformer
- date: 2022/2023（项目线）
- venue: 项目/论文（Google Robotics）
- 解决的问题（1～2句话）: 用Transformer在大规模多任务机器人示范上训练通用操控策略，提升跨任务泛化与数据效率。
- 设计挑战: 多任务融合与动作表示；长时依赖；数据采集标准化。
- 方案介绍: 将多任务示范统一到Transformer序列建模；动作以token或参数化形式表达；持续扩展数据规模与任务覆盖。
- 实验设置（简要）: 真实与仿真操控任务；指标为成功率。
- 实验结果（2–4条）: 大规模数据显著提升多任务成功率；对未见变体有更强鲁棒性。
- 不足和未来方向: 动作可执行性与精细控制仍需特别设计；跨实体泛化有待增强。

## 08_RT2_VLA_Model.pdf
- filename: 08_RT2_VLA_Model.pdf
- title: RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control
- date: 2023
- venue: Google DeepMind/Robotics 论文
- 解决的问题（1～2句话）: 将web-scale VLM知识迁移到机器人控制，通过VLA将视觉—语言知识转化为可执行行动，提高零样本泛化。
- 设计挑战: 跨模态对齐与行动映射；知识迁移的可靠性与安全。
- 方案介绍: 将网页/图文数据训练的VLM与动作输出层耦合；用指令条件与场景感知生成可执行行动。
- 实验设置（简要）: 多任务真实操控评测，指标为成功率与泛化到新对象/指令。
- 实验结果（2–4条）: 零样本表现提升，相对RT-1更强的跨域指令理解与执行能力。
- 不足和未来方向: 对低层控制与物理约束仍需专门模块；安全与失败恢复策略需加强。

## 09_OpenVLA An Open-Source Vision-Language-Action Model.pdf
- filename: 09_OpenVLA An Open-Source Vision-Language-Action Model.pdf
- title: OpenVLA: An Open-Source Vision-Language-Action Model
- date: 不详
- venue: 开源项目/论文
- 解决的问题（1～2句话）: 开源VLA模型，实现跨任务/跨实体的指令到行动映射，降低研究门槛。
- 设计挑战: 动作token化与可执行性；跨数据集一致性与评测。
- 方案介绍: 提供开源训练配方与评测套件，支持语言条件策略与通用动作表示。
- 实验设置（简要）: 多数据集/多任务对比评测；指标为成功率与泛化。
- 实验结果（2–4条）: 在开源基准上取得具竞争力的结果；提升复现与扩展性。
- 不足和未来方向: 需与更多真实数据与实体集成；标准化动作接口待完善。

## 10_X-VLA Soft-Prompted Transformer as Scalable Cross-Embodiment Vision-Language-Action Model.pdf
- filename: 10_X-VLA Soft-Prompted Transformer as Scalable Cross-Embodiment Vision-Language-Action Model.pdf
- title: X-VLA: Soft-Prompted Transformer as Scalable Cross-Embodiment Vision-Language-Action Model
- date: 不详
- venue: 论文/项目
- 解决的问题（1～2句话）: 通过soft prompt等条件化机制实现跨实体可扩展的VLA模型，减少对单一平台的过拟合。
- 设计挑战: 实体差异导致的状态—动作映射变化；软提示与策略稳定性。
- 方案介绍: 使用软提示/条件化编码器适配不同实体与任务；统一Transformer框架学习视觉—语言—行动。
- 实验设置（简要）: 跨实体多任务评测；指标为成功率与迁移性能。
- 实验结果（2–4条）: 在跨实体任务上较基线更鲁棒；策略迁移更稳定。
- 不足和未来方向: 软提示设计与泛化边界需进一步验证；与现实平台的接口标准化。

## Open X-Embodiment——Robotic Learning Datasets and RT-X Models.pdf
- filename: Open X-Embodiment——Robotic Learning Datasets and RT-X Models.pdf
- title: Open X-Embodiment: Robotic Learning Datasets and RT-X Models
- date: 2023/2024
- venue: 多机构合作数据集与模型论文
- 解决的问题（1～2句话）: 通过跨机构数据集与RT-X模型，提升跨任务与跨实体的泛化能力，推动开源社区资源共享。
- 设计挑战: 数据标准化与标注一致性；跨平台动作接口；隐私与合规。
- 方案介绍: 构建大规模跨实体操控数据集与统一模型RT-X；提供基准与评测协议。
- 实验设置（简要）: 多平台多任务评测；指标为成功率/泛化能力。
- 实验结果（2–4条）: 在跨任务/跨实体基准上显著提升；促进社区复现与扩展。
- 不足和未来方向: 数据质量与覆盖仍需提升；持续更新与更广平台支持。

