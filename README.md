---
license: mit
tags:
- generated_from_trainer
metrics:
- rouge
model-index:
- name: bart_large_summarise
  results: []
---

![SGH logo.png](https://s3.amazonaws.com/moonup/production/uploads/1667143139655-631feef1124782a19eff4243.png)

This model is a fine-tuned version of [facebook/bart-large-cnn](https://huggingface.co/facebook/bart-large-cnn) on the None dataset.
It achieves the following results on the evaluation set:
- Loss: 2.7389
- Rouge1: 0.5297
- Rouge2: 0.3602
- Rougel: 0.3961
- Rougelsum: 0.4821
- Gen Len: 137.9091

## Model description

This model was created to generate summaries of news articles.

## Intended uses & limitations

The model takes up to maximum article length of 1024 characters and generates a summary of maximum length of 512 characters.

## Training and evaluation data

This model was trained on 100+ articles and summaries from SGH.


### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 5e-05
- train_batch_size: 4
- eval_batch_size: 4
- seed: 42
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: linear
- lr_scheduler_warmup_steps: 500
- num_epochs: 10
- label_smoothing_factor: 0.1

### Framework versions

- Transformers 4.23.1
- Pytorch 1.12.1+cu113
- Datasets 2.6.1
- Tokenizers 0.13.1
