# AI PC Remote Lab 实验环境

## 📖 概述

AI PC Remote Lab 是基于 AMD Ryzen AI 370 和 395 系列 AI PC 构建的教学集群，旨在为学员提供真实的 AI PC 开发体验环境。

远程访问地址：212.129.248.110:8090

注意：请选择默认的20分钟使用时间，使用结束后请关闭Jupyter Lab

## 🖥️ 硬件资源

### Ryzen AI 处理器型号对比

| 规格项目               | Ryzen AI 9 HX 370 | Ryzen AI 9 HX 395 |
| ---------------------- | ----------------- | ----------------- |
| **CPU核心**      | 12核心/24线程     | 16核心/32线程     |
| **NPU算力**      | 50 TOPS           | 50 TOPS           |
| **iGPU型号**     | Radeon 890M       | Radeon 890M       |
| **iGPU核心数**   | 16 CU             | 40 CU             |
| **iGPU基础频率** | 2900 MHz          | 2900 MHz          |
| **显存**         | 64G共享系统内存   | 128G共享系统内存  |
| **TDP功耗**      | 28W               | 54W               |

> **注意**: 虽然两款处理器的iGPU规格相似，但395系列在更高的TDP下可以维持更高的持续性能表现。

### Ryzen AI 异构处理器特性

Ryzen AI PC 处理器集成了三大计算单元：

- **CPU**: 传统中央处理器，负责通用计算任务
- **NPU**: 神经网络处理单元，专门优化AI推理工作负载
- **iGPU**: 集成图形处理器，支持并行计算和图形渲染

### 计算单元性能特点

#### 🧠 NPU (Neural Processing Unit)

- **AI专用加速**: 针对AI推理任务优化的专用处理器
- **低功耗高效**: 相比CPU/GPU在AI任务上功耗更低
- **支持框架**: ONNX Runtime, DirectML等主流AI框架
- **算力差异**: 370系列50 TOPS vs 395系列55 TOPS

#### 🎮 iGPU (Integrated Graphics Processing Unit)

- **并行计算**: 1024个流处理器支持大规模并行操作
- **ROCm支持**: 兼容AMD ROCm开放计算平台
- **深度学习**: 支持PyTorch、TensorFlow等深度学习框架
- **功耗管理**: 根据TDP动态调整性能表现

## 🧪 实验环境配置

### 环境1: iGPU + PyTorch + ROCm 深度学习环境

#### 🎯 目标

使用集成显卡(iGPU)体验PyTorch深度学习框架，通过ROCm后端进行GPU加速计算。

#### 🔧 技术栈

- **深度学习框架**: PyTorch
- **GPU计算后端**: ROCm (Radeon Open Compute)
- **计算设备**: AMD Radeon iGPU
- **编程语言**: Python

#### 💡 适用场景

- 深度学习模型训练与推理
- 计算机视觉应用开发
- 自然语言处理实验
- GPU并行计算优化

---

### 环境2: NPU + Ryzen AI 软件栈开发环境

#### 🎯 目标

展示卷积神经网络(CNN)直接部署在NPU上的完整开发流程，体验专用AI加速器的性能优势。

#### 🔧 技术栈

- **AI软件栈**: Ryzen AI Software Stack
- **计算设备**: XDNA NPU
- **模型格式**: ONNX
- **开发工具**: Vitis AI, Quantizer

#### 💡 适用场景

- CNN模型NPU部署优化
- 边缘AI推理加速
- 低功耗AI应用开发
- 模型量化与优化

---

### 环境3: Lemonade Server + 本地大模型环境

#### 🎯 目标

通过Ryzen AI软件栈运行Lemonade Server，提供本地OpenAI API兼容接口，支持本地大模型的RAG(检索增强生成)和Agent应用开发。

#### 🔧 技术栈

- **服务器**: Lemonade Server
- **API标准**: OpenAI API Compatible
- **大模型引擎**: 本地部署LLM
- **应用场景**: RAG, AI Agent
- **计算后端**: Ryzen AI 软件栈

#### 💡 适用场景

- 本地大模型部署与调用
- RAG(检索增强生成)应用开发
- AI Agent智能助手构建
- 隐私保护的AI应用开发

## 🚀 实验特色

### 🔬 多样化计算体验

- **CPU通用计算**: 传统算法与数据处理
- **iGPU并行加速**: 深度学习训练与推理
- **NPU专用加速**: 高效AI推理优化

### 🛠️ 完整开发流程

- 模型开发与训练
- 模型优化与量化
- 部署与性能调优
- 应用集成与测试

### 📊 性能对比分析

- 不同计算单元性能评估
- 功耗效率对比
- 应用场景适配分析

## 📞 技术支持

如在实验过程中遇到技术问题，请联系：

- **邮箱**: fpgacamp.cn@outlook.com
- **技术支持**: AMD技术团队

---

*AMD Ryzen AI PC Remote Lab*
*2025年新工科联盟暑期学校*
