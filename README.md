# RAG-MathStar 智数星

基于 RAG（检索增强生成）与大语言模型的算术与数学问题智能解答系统

---

## 项目简介

RAG-MathStar 智数星是一套专为数学问题解答场景设计的智能系统，融合了大语言模型和检索增强技术（RAG），聚焦提升模型在数学推理、知识整合与解答准确性等方面的表现。系统支持多学段（小学、初中、高中）知识库，面向教育、培训与智能问答等多类应用场景。  
我们发布了自有高质量数学推理模型，并联合社区作者提供了多种量化模型版本，极大方便了本地与边缘设备部署。

- 原始模型仓库：[Mrpsy/RAG-MathStar](https://huggingface.co/Mrpsy/RAG-MathStar)
- 量化模型仓库：[mradermacher/RAG-MathStar-GGUF](https://huggingface.co/mradermacher/RAG-MathStar-GGUF)

---

## 项目背景

近年来，AI与深度学习推动自然语言处理和知识获取飞速发展，但数学自动解答依然面临诸如高质量数据缺乏、推理复杂、传统RAG检索效率与精度有限等痛点。  
本项目旨在结合自研数据集、高效模型训练和知识库检索，构建面向数学领域的高性能智能问答系统，为教育和科研提供坚实技术支撑。

---

## 技术方案

### 数据收集与知识库

- 多渠道收集、筛选和构建高质量数学问答数据集，涵盖小学、初中、高中全学段。
- 支持个性化知识库增删与私有数据上传，满足定制化需求。

### 模型训练与优化

- 采用 Qwen2.5-3B-Instruct 作为基础模型，针对数学推理领域进行高质量 SFT（监督微调）。
- 引入组相对策略优化（GRPO）强化学习，对难点问题和答案格式进行双重优化。

### RAG 智能体创新

- 在传统 RAG 框架基础上，集成智能 Agent 处理模块，动态监控和优化检索与生成。
- 多知识库支持，检索更高效、答案更精准。

### WebUI 与交互体验

- 提供现代化 Web 前端，支持对话式问答、思维链路展示和链式推理可视化。
- 多模态输入支持（文本/语音），知识库内容可管理。

---

## 核心功能

- 算术与数学问题一键解答
- 多学段知识库智能问答
- 推荐式内容推送与推理链路透明化
- 个性化知识库管理和私有文件上传
- 本地、在线双模式灵活部署

---

## 模型下载与使用

### 原始模型

- 仓库地址：[Mrpsy/RAG-MathStar](https://huggingface.co/Mrpsy/RAG-MathStar)
- 适合科研开发、二次训练与高性能服务器推理。

### GGUF 量化模型

- 仓库地址：[mradermacher/RAG-MathStar-GGUF](https://huggingface.co/mradermacher/RAG-MathStar-GGUF)
- 由社区知名作者 mradermacher 基于原始模型高效量化，提供 Q2_K、Q4_K_S、Q6_K、Q8_0、f16 等多版本。
- 适用于 GGML/GGUF 框架，在本地、轻量设备也能高效运行。

**使用提示**：  
如不了解如何加载 GGUF 文件，建议参考 [Hugging Face GGUF 文档](https://huggingface.co/docs/transformers/gguf) 或 [TheBloke 使用指南](https://huggingface.co/TheBloke)。

---

## 应用对象与场景

- **学生/教师**：课内外辅导、数学问题讲解
- **教育机构**：智能答疑、个性化学习平台
- **开发者/企业**：AI 数学产品与服务集成
- **科研人员**：数学自动推理、数据增强

---

## 环境与工具

- **后端**：Python, PyTorch, Docker, Nginx
- **前端**：Svelte, Node.js
- **推荐硬件**：普通 CPU/GPU 即可，根据量化模型自由适配
- **环境示例**：Ubuntu 20.04, Intel i7-6850K, Nvidia 1080Ti 11GB, 32GB RAM

---

## 在线体验

- [智数星·RAG-MathStar 在线体验地址](http://starvii.tpddns.cn:9001/info)

---

## 致谢

- **智数星团队**：原始模型训练与系统开发
- **mradermacher**：模型量化与社区分发支持

---

> 本项目持续开源，欢迎 Issues、PR 及各类合作交流！

