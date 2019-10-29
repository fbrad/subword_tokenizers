# Subword Tokenizers

This repo explores the different subword tokenizers.

## Subword tokenizers

| Algorithm | Base unit | Implementations | Paper |Used by|
|-----------|-----------|--------|-------|------|
|Byte-pair encoding (BPE)|Unicode code|[original implementation](https://github.com/rsennrich/subword-nmt), [FastBPE](https://github.com/glample/fastBPE), [SentencePiece repo](https://github.com/google/sentencepiece)|[Neural Machine Translation of Rare Words with Subword Units](https://arxiv.org/pdf/1508.07909.pdf)|
|byte-level BPE|byte|[HuggingFace repo](https://huggingface.co/transformers/_modules/transformers/tokenization_gpt2.html#GPT2Tokenizer), [GPT2 repo](https://github.com/openai/gpt-2/blob/master/src/encoder.py)|[Language Models are Unsupervised Multitask Learners (GPT2)](https://d4mucfpksywv.cloudfront.net/better-language-models/language-models.pdf)|[GPT2](https://d4mucfpksywv.cloudfront.net/better-language-models/language-models.pdf), [RoBERTa](https://arxiv.org/pdf/1907.11692)
|Wordpiece|Unicode code| [BERT repo](https://github.com/google-research/bert/blob/d66a146741588fb208450bde15aa7db143baaa69/tokenization.py) | [Google's Neural Machine Translation System](https://arxiv.org/pdf/1609.08144.pdf)| [Transformers](https://arxiv.org/pdf/1706.03762.pdf), [BERT](https://arxiv.org/pdf/1810.04805.pdf)|
| Unigram Language Model | Unicode code | [SentencePiece repo](https://github.com/google/sentencepiece)| [Subword Regularization: Improving NN Translation Models...](https://arxiv.org/pdf/1804.10959.pdf)| |
|

## Large Pretrained Language Models and their tokenizers:

| Model | Repo | Tokenizer | 
|-------|------|-----------|
|[BERT (Google)](https://arxiv.org/pdf/1810.04805.pdf)|[GitHub link](https://github.com/google-research/bert) | WordPiece |
|[GPT2 (OpenAI)](https://d4mucfpksywv.cloudfront.net/better-language-models/language-models.pdf)|[GitHub link](https://github.com/openai/gpt-2)|byte-level BPE|
|[RoBERTa (Facebook)](https://arxiv.org/pdf/1907.11692)|[GitHub link](https://github.com/pytorch/fairseq/blob/master/examples/roberta/README.md)|byte-level BPE|
|[Transformer-XL (CMU)](https://arxiv.org/pdf/1901.02860.pdf)| [GitHub link](https://github.com/kimiyoung/transformer-xl)| words |
|[XLM (Facebook)](https://arxiv.org/pdf/1901.07291.pdf)|[GitHub link](https://github.com/facebookresearch/XLM)|BPE |
|[XLNet (CMU)](https://arxiv.org/pdf/1906.08237.pdf)|[GitHub link](https://github.com/zihangdai/xlnet)|BPE (from SentencePiece)|
|[CTRL (Salesforce)](https://arxiv.org/pdf/1909.05858.pdf)|[GitHub link](https://github.com/salesforce/ctrl)| BPE (from fastBPE)

