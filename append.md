**综述类-2**

+ Agentic Environment Engineering for Large Language Models: A Survey of Environment Modeling, Synthesis, Evaluation, and Application
- https://arxiv.org/pdf/2606.12191
* 综述 2026/06/10 arxiv
本论文系统研究了大语言模型（LLM）代理的环境，涵盖环境建模、合成、评估和应用等生命周期。首先，从八个属性和领域的角度介绍了代表性环境，并分析了其发展路径和核心能力。其次，提出了符号合成和神经合成两种自动化环境合成范式，并展示了各范式下的环境评估方法。论文还讨论了代理与环境共同演化的应用，特别是从记忆中心经验演化、工作流演化、轨迹演化和探索演化四个角度分析了代理在动态环境中的演化路径。最后，探讨了未来的研究方向，包括环境即服务、多代理环境和神经符号环境等。

+ Toward Secure LLM Agents: Threat Surfaces, Attacks, Defenses, and Evaluation
- https://arxiv.org/pdf/2606.10749
* 综述 2026/06/09 arxiv
本文探讨了大语言模型（LLM）代理的安全性，分析了安全风险的变化及其对代理行为的影响。通过对247篇文献的综合，提出了一种基于生命周期的系统框架，围绕信息流、授权委托和持久状态的交互建模代理安全。文章组织了关于LLM代理安全的四个关键问题，发现当前的防御措施仍然较弱，且现有基准未能充分代表长期、状态敏感的风险。作者认为，安全的LLM代理需要明确的信任边界、原则性的权限控制和与现实操作环境相一致的评估实践。

**方法类和框架类-16**

+ EvoArena: Tracking Memory Evolution for Robust LLM Agents in Dynamic Environments
- https://arxiv.org/pdf/2606.13681
* 方法类和框架类
本论文介绍了EvoArena，一个基准套件，用于模拟动态环境中的变化，并提出了EvoMem，一种基于补丁的记忆范式，记录记忆演变的结构化更新历史。通过实验，当前代理在EvoArena上的表现不佳，而EvoMem显著提高了性能，表明在评估和记忆建模中考虑环境演变的重要性。

+ MemRefine: LLM-Guided Compression for Long-Term Agent Memory
- https://arxiv.org/pdf/2606.13177
* 方法类和框架类
随着大语言模型（LLM）代理在长期交互中的应用，如何有效管理和压缩记忆成为一个重要问题。论文提出了MemRefine框架，旨在在固定存储预算内优化记忆管理，保留对未来任务有用的信息。该框架利用LLM判断信息的事实内容，迭代进行删除、合并和保留决策，以满足存储预算。实验表明，MemRefine在多个记忆框架和长期对话基准上表现优异，能够在严格预算下保持性能，超越基于规则的基线方法。

+ Getting Better at Working With You: Compiling User Corrections into Runtime Enforcement for Coding Agents
- https://arxiv.org/pdf/2606.13174
* 方法类和框架类
本论文研究了交互式LLM代理在用户偏好遵循方面的不足，提出了TRACE方法，通过将用户的修正编译为运行时检查，显著减少了偏好违反的情况。TRACE方法能够在未来的任务中自动应用用户的修正，提升了LLM代理的易用性和准确性。实验结果表明，TRACE在多个任务中有效降低了偏好违反率，展示了其在记忆和用户交互中的潜力。

+ G-Long: Graph-Enhanced Memory Management for Efficient Long-Term Dialogue Agents
- https://arxiv.org/pdf/2606.13115
* 方法类和框架类
本论文提出了G-Long，一个图增强的内存管理框架，旨在提高长时间对话代理的效率。尽管大语言模型（LLMs）在开放域对话系统中取得了进展，但由于长上下文推理的固有限制，保持长期一致性仍然是一个挑战。现有方法通常依赖于非结构化内存存储，容易导致信息丢失，或依赖计算成本高昂的LLMs，导致高延迟。G-Long通过利用微调的小型语言模型进行结构化三元组提取和关联检索，显著降低了操作成本，并引入了一种新的注意力感知重要性评分机制，以识别显著记忆。实验结果表明，G-Long在响应生成和记忆检索方面均实现了最先进的性能。

+ Multi-Turn Reasoning When Context Arrives in Pieces: Scalable Sharding and Memory-Augmented RL
- https://arxiv.org/pdf/2606.12941
* 方法类和框架类
本论文研究了在多轮对话中，当用户分多次提供关键信息时，大语言模型的准确性会显著下降。为了解决这一问题，作者提出了一种紧凑的滚动记忆机制，替代传统的历史信息处理方式。通过引入低成本的分片管道，将单轮问答数据集转化为多轮碎片信息的情境，显著提高了多轮对话的准确性，并在零-shot情况下对更复杂的数学和长上下文问答任务表现出色。记忆训练的模型在测试时即使获得完整历史信息，仍然优于全历史基线，表明学习压缩信息能增强推理能力。

+ Arbor: Tree Search as a Cognition Layer for Autonomous Agents
- https://arxiv.org/pdf/2606.12563
* 方法类和框架类
Arbor是一个多智能体框架，引入结构化树搜索作为自主智能体在大型状态空间中操作的认知层。与以往的优化系统不同，Arbor维护一个显式的搜索树作为共享工作记忆，随着每次测量而演变。该框架在全栈LLM推理优化中得到了验证，展示了其在性能上的显著提升。Arbor通过协调不同的智能体实现优化，确保系统的稳定性和可重复性，适用于多代硬件平台。

+ Substrate Asymmetry in User-Side Memory: A Diagnostic Framework
- https://arxiv.org/pdf/2606.11712
* 方法类和框架类
本论文提出了一种诊断框架，用于分析大语言模型中的用户侧记忆。研究表明，用户记忆的能力通常被视为单一的“个性化”能力，但实际上隐藏了相反方向的失败。记忆可以分解为至少三个正交轴：行为一致性、事实存在和事实缺失。通过对比不同的记忆模型，发现不同模型在这些维度上表现不一，提出了对记忆模型的诊断框架和实证研究结果，揭示了参数化用户记忆的对齐税和路由分类的发现。

+ Organize then Retrieve: Hierarchical Memory Navigation for Efficient Agents
- https://arxiv.org/pdf/2606.11680
* 方法类和框架类
本研究提出了一种名为HORMA的层次化组织与检索记忆代理，旨在解决大语言模型（LLM）代理在长时间任务中面临的无状态性问题。现有方法往往依赖于损失压缩或基于相似性的检索，无法有效捕捉多步骤任务所需的时间结构和因果依赖。HORMA通过将经验组织成类似文件系统的层次结构，提供高效的访问方式，减少推理成本和延迟。该方法通过结构化记忆构建和基于导航的检索两个阶段，优化了任务相关上下文的获取，显著提高了在长对话任务中的性能和效率。

+ Position: Hippocampal Explicit Memory Is the Cornerstone for AGI
- https://arxiv.org/pdf/2606.11245
* 方法类和框架类
这篇立场论文认为，整合显性记忆是推动大语言模型（LLMs）向人工通用智能（AGI）发展的基石。作者指出，LLMs的学习机制与人类的隐性记忆高度相似，但AGI所需的高级认知功能，如长期战略规划、元认知和符号推理，严重依赖于海马体显性记忆，不能仅依靠隐性统计学习。论文结合神经科学的发现，提出了人工显性记忆系统的计算需求，旨在促进进一步研究并为显性记忆的整合奠定基础。

+ Trace Only What You Need: Structure-Aware On-Demand Hypergraph Memory for Long-Document Question Answering
- https://arxiv.org/pdf/2606.10921
* 方法类和框架类
长文档问答需要大语言模型（LLMs）在冗长文档中推理，答案往往依赖于事件顺序、章节上下文和跨部分证据连接。现有的结构化RAG方法存在知识组织成本高、文档结构利用不足和历史推理经验无法重用等问题。为了解决这些问题，本文提出了DocTrace，一个多agent的RAG框架，支持查询触发的知识组织、文档结构感知和经验指导推理。DocTrace通过轻量级文档结构树索引保持文档层次结构，在推理过程中按需构建agent共享的超图结构工作记忆，并存储成功的推理计划以供未来重用。实验表明，DocTrace在四个长文档QA数据集上表现优异，性能超过最强基线ComoRAG。

+ REAL: A Reasoning-Enhanced Graph Framework for Long-Term Memory Management of LLMs
- https://arxiv.org/pdf/2606.10694
* 方法类和框架类
随着大语言模型（LLMs）在长期交互中的应用日益增加，如何有效管理长期记忆成为关键问题。现有的记忆系统存在多种局限性，如无法有效捕捉记忆之间的关系和信息更新的破坏性。REAL框架通过构建一个时间和置信度感知的有向属性图来管理长期对话记忆，采用非破坏性更新策略，保留事实的多个版本，并通过语义评估引导的混合搜索提取相关记忆子图。实验结果表明，REAL在长期记忆性能上显著优于现有方法，平均提升22.72%。

+ Infini Memory: Maintainable Topic Documents for Long-Term LLM Agent Memory
- https://arxiv.org/pdf/2606.10677
* 方法类和框架类
本论文提出了Infini Memory，一种可维护的基于文本的持久记忆架构，旨在满足长期LLM代理的需求。现有的记忆系统通常将观察结果存储为孤立记录，导致证据聚合和记忆维护困难。Infini Memory将代理记忆视为主题结构文档，每个主题文档作为收集相关证据的语义单元，能够随着时间的推移修订事实。新观察首先在缓冲区中暂存，并定期整合为连贯的文本上下文。在推理时，代理检索过程允许LLM通过迭代工具调用读取记忆，而不是单一步骤检索。

+ ActiveMem: Distributed Active Memory for Long-Horizon LLM Reasoning
- https://arxiv.org/pdf/2606.10532
* 方法类和框架类
本论文提出了ActiveMem，一个分布式主动记忆框架，旨在帮助大语言模型（LLM）代理处理长时间推理任务。现有的记忆机制通常是集中式的，导致推理过程中的上下文过载或信息丢失。ActiveMem通过将代理记忆与核心推理过程解耦，采用高层次的规划者和轻量级的分布式记忆系统并行工作，显著提高了推理的准确性并减少了开销。实验结果表明，ActiveMem在BrowseComp-Plus和GAIA数据集上达到了最先进的准确率。

+ Memory Beyond Recall: A Dual-Process Cognitive Memory System for Self-Evolving LLM Agents
- https://arxiv.org/pdf/2606.09483
* 方法类和框架类
本论文提出了一种名为DCPM的双过程认知记忆系统，旨在改善大语言模型（LLM）代理的长期记忆管理。当前的记忆系统主要依赖于表面回忆，难以处理隐式个性化和用户演变的推理。DCPM通过建立一个认知能力层次结构，组织代理记忆，从原始输入和原子事实到信念轨迹和领域模式，采用双过程理论的架构分裂，分别由同步的白天写入者和异步的夜间引擎驱动。实验结果表明，DCPM在隐式跨会话推理方面表现优异，推动了LLM代理的记忆能力。

+ MemToolAgent: Leveraging Memory for Tool Using Agents Based on Environment and User Feedback
- https://arxiv.org/pdf/2606.07909v2
* 方法类和框架类
现代大语言模型（LLM）代理可以使用外部工具帮助用户解决复杂任务。然而，对于需要从长期历史事件或先前代理-环境交互中学习的问题，LLM代理需要使用记忆机制来存储和检索经验。本文提出了MemToolAgent框架，通过记忆管理改善工具使用能力。该方法包含一个记忆提取模块，将过去的经验处理为结构化的记忆条目，以及一个检索模块，动态选择存储的记忆条目的子集。这使得响应更加个性化和准确，符合用户偏好和反馈，而无需对LLM进行微调。

+ AdMem: Advanced Memory for Task-solving Agents
- https://arxiv.org/pdf/2606.06787
* 方法类和框架类
本论文介绍了一种统一的自动记忆框架，旨在提升大语言模型（LLM）作为任务解决代理的能力。现有的记忆方法主要关注存储事实信息，而本研究通过结合语义、情节和程序记忆，提出了一种双层设计的记忆框架。该框架通过多代理架构实现自动记忆生成、奖励注释和自适应检索，确保长期记忆的管理和持续改进。实验结果表明，该方法在长多轮任务中相较于现有基线表现出更好的鲁棒性和成功率，强调了全面、自适应记忆在推进LLM代理中的重要性。

**数据集和评估基准类-2**

+ Recalling Too Well: Sycophancy Evaluation and Mitigation in Memory-Augmented Models
- https://arxiv.org/pdf/2606.10949
* 基准类
本论文研究了持久记忆系统如何使大语言模型（LLM）在存储用户信念时变得更加有用，但同时也导致模型的准确性下降，系统性地放大了谄媚行为，即模型优先考虑与用户一致性而非准确性。我们首次系统评估了这一效应，介绍了MIST基准，测试了三种最先进的记忆系统和五个模型系列，发现记忆在所有条件下都放大了谄媚行为。基于这些结果，我们提出了两种轻量级的缓解措施，显著减少了谄媚行为，同时在事实回忆方面与记忆系统相匹配或超越。

+ H2HMem: A Multimodal Memory Benchmark for Agents in Human-Human Interactions
- https://arxiv.org/pdf/2606.09461
* 基准类
本论文提出了H2HMem，一个用于评估在复杂人际交互中大语言模型代理记忆能力的多模态基准。现有的记忆基准主要集中在单用户文本交互，未能捕捉多模态和复杂话语现象的挑战。H2HMem包括双人和多方对话，评估代理在记忆回忆、推理和应用等三个维度的表现。实验显示，现有代理在跨模态、参与者和会话中构建、保留和利用记忆方面存在显著局限，强调了下一代LLM代理的改进空间。

**模型和系统类-4**

+ Maestro: Workload-Aware Cross-Cluster Scheduling for LLM-Based Multi-Agent Systems
- https://arxiv.org/pdf/2606.12950v1
* 模型和系统类
本文提出了Maestro，一个针对LLM-MAS（基于大语言模型的多代理系统）的工作负载感知调度系统，旨在解决在资源受限的云环境中部署多代理工作负载所面临的系统挑战。Maestro通过预测每个阶段的输出长度和内存使用，驱动分层调度器，支持动态多模型共存和弹性内存配置。实验结果表明，Maestro显著减少了内存使用并提高了服务水平目标的达成率。

+ Learning What to Remember: A Cognitively Grounded Multi-Factor Value Model for Agentic Memory
- https://arxiv.org/pdf/2606.12945v1
* 模型和系统类
本文提出了一种基于认知心理学的多因素记忆价值模型，旨在解决长时间运行的LLM代理在记忆管理中的挑战。该模型通过七个可解释因素（如情感强度、目标相关性等）来决定在固定记忆预算下的编码、遗忘和检索策略。研究表明，学习的权重在记忆保留和检索效率上优于传统方法，且模型的可解释性强。所有实验在单个CPU上运行，且模型为开源。

+ Rosetta Memory: Adaptive Memory for Cross-LLM Agents
- https://arxiv.org/pdf/2606.07711
* 模型和系统类
本论文提出了一种名为Rosetta Memory的适应性记忆系统，旨在将无状态的大语言模型（LLM）转变为持久、不断发展的智能体。现有的记忆系统通常围绕特定的LLM设计，而用户在不同任务中常常切换LLM。为了解决这一问题，论文从记忆中心的角度出发，设计了两种条件化操作符，优化记忆的存储和呈现方式，以提高任务完成效果。实验结果表明，该模型在多个基准测试中表现优异，且在未见模型替换的情况下依然保持稳健性。

+ Agent Memory: Characterization and System Implications of Stateful Long-Horizon Workloads
- https://arxiv.org/pdf/2606.06448
* 模型和系统类
本论文研究了LLM代理在长时间任务中对状态记忆的需求，提出了一种系统化的分类法来描述代理记忆系统，并构建了一个阶段感知的分析工具来评估记忆系统的成本。通过对十个代表性系统的特征分析，论文揭示了设计选择如何影响写入和读取路径的成本，并提出了十条系统建议，涵盖了构建调度、能力底线、查询量的摊销、新鲜度-延迟权衡及大规模管理等方面。
