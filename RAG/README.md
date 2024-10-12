# LLM Fine-tuning
In this repository, I will highlight the mainstream methods for fine-tuning LLMs, focusing only on their implementation instead of doing scientific research. Fine-tuning involves training a subset of the parameters of a large pre-trained model to better align with a specific task or dataset. Therefore, fine-tuning can be viewed as a specialized form of training.

## I. Prerequisites
The LLM is trained on a large corpus of data to learn to predict the next tokens from the previous tokens by using the attention mechanism. This self-supervised process is also known as **Pre-training**, which requires a very large amount of data and a lot of computational resources. 

However, only a few companies (e.g. OpenAI, Google, Meta, etc.) can afford to pre-train their own LLMs due to the high cost. Fortunately, we can leverage the some open-source pre-trained LLMs without the need to train from scratch. Therefore, I provide the following resources to help you understand the basic concepts of transformer models. 

- Basic Concepts
  - [ ] Word Embedding
  - [ ] Positional Embedding
  - [ ] Self-Attention Mechanism: Query, Key, Value
  - [ ] Masked Self-Attention
  - [ ] Residual Connection
  - [ ] Encoder-Decoder Attention
- Transformers 
  - [Tutorial Video](https://www.youtube.com/watch?v=zxQyTK8quyY&t=1550s)
- Decoder-only Transformer 
  - [Tutorial Video](https://www.youtube.com/watch?v=bQ5BoolX9Ag)
  - [Demo Notebook](https://github.com/ChengIC/pytorch_tutorials/blob/main/section14_transformers/solutions/Pytorch2_Transformer_Text_Generation.ipynb)
- BERT

## II. Fine-tuning Methods
After pre-training the LLM, we usually face the following issues:
- **Human preferences**: The pre-trained LLM may not align with human preferences due to the data bias.
- **Task-specific**: The pre-trained LLM may not perform well on a specific task or scenario.

The following methods are designed to address the above mentioned issues:

### Parameter-Efficient Fine-Tuning
  - [Hugging Face PEFT Implementations](https://huggingface.co/blog/peft)
  - LoRA
    - [Blogs](https://magazine.sebastianraschka.com/p/practical-tips-for-finetuning-llms?utm_source=profile&utm_medium=reader2)

  - Prompt Tuning
  - P-tuning v2 (Prefix-tuning)
  - P-tuning

### Instruction Fine-tuning
  - [Github](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)

### RLHF
  - [Github](https://github.com/raghavc/LLM-RLHF-Tuning-with-PPO-and-DPO) 
  - [Short Course](https://learn.deeplearning.ai/courses/reinforcement-learning-from-human-feedback/lesson/1/introduction) 
  - [Google Paper](https://arxiv.org/abs/1706.03741) 
  - [OpenAI Paper](https://arxiv.org/abs/2203.02155)

### Distillation
  - [Github](https://github.com/Tebmer/Awesome-Knowledge-Distillation-of-LLMs?tab=readme-ov-file#kd-algorithms)

## III. Recommended Repositories
- [LLM Fine-tuning](https://github.com/ashishpatel26/LLM-Finetuning)
- [Pytorch Tutorials](https://github.com/LukeDitria/pytorch_tutorials) 