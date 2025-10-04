In lab2, I fine-tuned a generative language model for dialogue summarization using three approaches — the original model, a fully fine-tuned (instruct) model, and a PEFT (Parameter-Efficient Fine-Tuning) model.
Performance was evaluated using ROUGE metrics to measure summary quality against human-written baselines.

Original Model: ROUGE-1 = 0.23

Instruct Model: ROUGE-1 = 0.42

PEFT Model: ROUGE-1 = 0.41

The PEFT model showed a ~17% improvement over the original model and performed within 1–2% of the fully fine-tuned model, while requiring significantly less compute and memory resources (trainable on a single GPU).

This demonstrates that PEFT offers an efficient trade-off between performance and resource cost for large language model fine-tuning.
