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

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# bart_large_summarise

This model is a fine-tuned version of [facebook/bart-large-cnn](https://huggingface.co/facebook/bart-large-cnn) on the None dataset.
It achieves the following results on the evaluation set:
- Loss: 2.7389
- Rouge1: 52.9676
- Rouge2: 36.0168
- Rougel: 39.6093
- Rougelsum: 48.2053
- Gen Len: 137.9091

## Model description

More information needed

## Intended uses & limitations

encoder_max_length = 1024
  
decoder_max_length = 512

## Training and evaluation data

More information needed

## Training procedure

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

### Training results



### Framework versions

- Transformers 4.23.1
- Pytorch 1.12.1+cu113
- Datasets 2.6.1
- Tokenizers 0.13.1
