# LLM Fine-tuning
The categoristation of LLM finetuning methods is not very clear compared to other fields like computer vision. In fact, a lot of people cannot tell the difference between 'RAG', 'Fine tuning', 'Prompt Engineering' and 'training'. In this repository, I will highlight the mainstream methods for fine-tuning LLMs, focusing only on their implementation instead of literature review. Fine-tuning involves training a subset of the parameters of a large pre-trained model to better align with a specific task or dataset. Therefore, fine-tuning can be viewed as a specialized form of training.

## Methods
- Parameter-Efficient Fine-Tuning [blogs](https://huggingface.co/blog/peft)
  - LoRA [blogs](https://magazine.sebastianraschka.com/p/practical-tips-for-finetuning-llms?utm_source=profile&utm_medium=reader2)
  - Prompt Tuning
  - P-tuning v2 (Prefix-tuning)
  - P-tuning
- Instruction Fine-tuning [github](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
- RLHF (Reinforcement Learning from Human Feedback) [github](https://github.com/raghavc/LLM-RLHF-Tuning-with-PPO-and-DPO)
- Distillation [github](https://github.com/Tebmer/Awesome-Knowledge-Distillation-of-LLMs?tab=readme-ov-file#kd-algorithms)

## Playground
- [LLM Fine-tuning Playground](https://github.com/ashishpatel26/LLM-Finetuning)