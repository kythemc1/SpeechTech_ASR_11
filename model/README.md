## checkpoint model
link: https://huggingface.co/kegacua/whisper-small-vi

## about this model
This model is a fine-tuned version of openai/whisper-medium on the VLSP 10000 dataset. It achieves the following results on the evaluation set:

eval_loss: 0.4817
eval_wer: 20.0226
eval_runtime: 2347.1739
eval_samples_per_second: 0.852
eval_steps_per_second: 0.213
epoch: 2.0
step: 1750

## Model description
More information needed

## Intended uses & limitations
More information needed

## Training and evaluation data
More information needed

## Training procedure
Training hyperparameters
The following hyperparameters were used during training:

learning_rate: 1e-05
train_batch_size: 4
eval_batch_size: 4
seed: 42
gradient_accumulation_steps: 2
total_train_batch_size: 8
optimizer: Use OptimizerNames.ADAMW_TORCH with betas=(0.9,0.999) and epsilon=1e-08 and optimizer_args=No additional optimizer arguments
lr_scheduler_type: linear
lr_scheduler_warmup_steps: 500
num_epochs: 2
mixed_precision_training: Native AMP
Framework versions
Transformers 4.51.3
Pytorch 2.5.1+cu124
Datasets 3.6.0
Tokenizers 0.21.0