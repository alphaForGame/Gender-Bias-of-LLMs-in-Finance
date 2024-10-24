# 本项目是论文《金融决策中大型语言模型运用的性别偏见：伦理视角》的WEAT实验部分
	1.	其中 results 包含了论文所有运行的研究数据，可以直接使用 plot.ipynb 进行图表制作。
	2.	bert_full.ipynb 是运行 BERT 系列模型的 notebook，把 model_configs 参数换成需要测试的 BERT 系列模型。
	3.	llama.ipynb 是运行 LLaMA 系列模型的 notebook，把 model_configs 参数换成需要测试的 LLaMA 系列模型。
	4.	7B-8B LLMs 建议使用 2*48G 以上 GPU 运行，70B 建议使用 4*48G 以上 GPU 运行，BERT 系统可以在一般性能电脑上运行。

## 测试模型列表

| 名称           | 规模（B） | HuggingFace上的模型名称                     | 特征                                        |
|----------------|----------|---------------------------------------------|---------------------------------------------|
| bert-base      | 0.11     | bert-base-uncased                           | 广泛应用于商用微调，适合小规模任务            |
| bert-large     | 0.34     | bert-large-uncased                          | 参数规模更大，适合复杂任务的微调              |
| LLaMA-3.1-8B   | 8        | meta-llama/Meta-Llama-3.1-8B                | 开源模型，性价比较高，适合中型任务            |
| LLaMA-3.1-70B  | 70       | meta-llama/Meta-Llama-3.1-70B               | 适合大型任务的微调，逐渐普及                  |
| FinancialBert  | 0.11     | ahmedrachid/FinancialBERT-Sentiment-Analysis| 针对金融领域微调，适用于情感分析等任务        |
| FinBert        | 0.11     | yiyanghkust/finbert-tone                    | 经济金融文本分析的首选，具有专业语料训练优势  |
| LLaMAFin       | 7        | AdaptLLM/finance-chat                       | 在众多金融任务上媲美BloombergGPT-50B         |
