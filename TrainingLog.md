<!-- markdownlint-disable first-line-h1 -->
<!-- markdownlint-disable html -->

<div align="center">
<h1>
  Yayi-Base 训练日志
</h1>
</div>

- [Yayi-base 1.6B](#yayi-base-16b)
- [Yayi-base 7B](#yayi-base-7b)
- [Tokens 处理速度测试](#tokens-处理速度测试)
- [模型推理效果测试](#模型推理效果测试)
  - [推理速度和显存](#推理速度和显存)
  - [RoPE \& ALiBi 对比实验](#rope--alibi-对比实验)
- [KV-cache \& flashattention 实验](#kv-cache--flashattention-实验)
- [vLLM 可行性测试](#vllm-可行性测试)
- [flashattention 速度测试](#flashattention-速度测试)



# Yayi-base 1.6B

- **实验目的**：训练并评价模型表现
- **负责人**：王品，董垚
- **开始时间**：
- **硬件**：
- **数据集**：
- **模型设置**：
- **预计运行时间**：
- **实验结果**：

# Yayi-base 7B

- **实验目的**：训练并评价模型表现
- **负责人**：王品，董垚
- **开始时间**：
- **硬件**：
- **数据集**：
- **模型设置**：
- **预计运行时间**：
- **实验结果**：
  - loss 曲线
  - checkpoints 评估


# Tokens 处理速度测试
- **实验目的**：计算 7B、13B 和 30B 模型处理 token 速度
- **负责人**：王品
- **开始时间**：
- **硬件**：
- **数据集**：
- **模型设置**：
- **预计运行时间**：
- **实验结论**：

# 模型推理效果测试

## 推理速度和显存


- **实验目的**：测试不同参数量模型在推理阶段实际占用的资源及推理速度
- **负责人**：董垚
- **开始时间**：20230802 1900
- **硬件**：企商，GPU=8 * A100(80G)，ip=172.16.100.1@172.16.10.75
- **数据集**：随机 prompts
```python
speed_prompts = ["Hey, are you conscious? Can you talk to me?",
                "I feel so bad today, what should I do?",
                "I've won an award today, I'm in a good mood",
                ]	
```
- **模型设置**：
  - $\text{yayi-base}^{\text {1.6B}}$: 
  - $\text{yayi-base}^{\text {7B}}$: 
- **预计运行时间**：
- **实验结论**：
  
|Model             | Speed(tokens/s) | Mem(MB)    | GPU-UTL(%) | use_cache | Pwr_usg(W)  | 备注    |
|:-----------:|:---------------:|:----------:|:----------:|:---------:|:-----------:|:-----:|
| Yayi-base7B | 30.76           | 14814.00   | 50         | FALSE     | 132         | 单卡；空载 |
| Yayi-base7B | 30.76           | 14814.00   | 50         | TRUE      | 132         | 单卡；空载 |

## RoPE & ALiBi 对比实验

- **实验目的**：
- **负责人**：董垚
- **开始时间**：
- **硬件**：企商，GPU=8 * A100(80G)，ip=172.16.100.1@172.16.10.75
- **数据集**：
- **模型设置**：
  - $\text{yayi-base}^{\text {1.6B}}$: 
- **预计运行时间**：
- **实验结论**：

# KV-cache & flashattention 实验

- **实验目的**：
- **负责人**：蒋永余
- **开始时间**：
- **硬件**：
- **数据集**：
- **模型设置**：
- **预计运行时间**：
- **实验结论**：

# vLLM 可行性测试

- **实验目的**：
- **负责人**：董垚
- **开始时间**：
- **硬件**：
- **数据集**：
- **模型设置**：
- **预计运行时间**：
- **实验结论**：

# flashattention 速度测试

- **实验目的**：
- **负责人**：王品
- **开始时间**：
- **硬件**：
- **数据集**：
- **模型设置**：
- **预计运行时间**：
- **实验结论**：
