---
title: Parameters and settings
description: 
published: true
date: 2023-04-15T16:06:04.994Z
tags: 
editor: markdown
dateCreated: 2023-04-12T21:16:14.146Z
---

# Parameters and settings

## General

**Epochs** - the cycle of examining each of the instance dataset images once ([source](https://www.reddit.com/r/StableDiffusion/comments/y6gjjz/question_about_training_epochs/))

**Training steps** \- the # of steps taken in fine tuning the model. The number of displayed training steps is roughly **(**\# of images in training set) x (# of epochs) / (batch size). Each batch effectively counts as a single training step (confirm this). 

**Batch size** - the number of images processed at once during training ([source](https://github.com/AUTOMATIC1111/stable-diffusion-webui/discussions/4814), [source](https://github.com/victorchall/EveryDream-trainer)). Increasing speeds up training at the cost of increased VRAM usage.

**CFG** \- stands for classifier free guidance. Forces the generation to better match the prompt potentially at the cost of image quality or diversity ([source](https://huggingface.co/blog/stable_diffusion)) 

**Sampler** - the method used to estimate noise at each step in the denoising process, which gradually produces a final image from an initial noisy image. There is often a trade-off between speed and accuracy of denoising. ([source](https://stable-diffusion-art.com/samplers/#What_is_Sampling))

## LoRAs specifically

**LoRA** \- stands for low-rank adaptation, a mathematical technique to reduce the number of parameters that are trained. Results in a smaller model which is also faster to train. Technique can be applied to different types of models, but has been especially popular for text-to-image models like Stable Diffusion ([source](https://replicate.com/blog/lora-faster-fine-tuning-of-stable-diffusion)).

**Rank** \- 

**Alpha**

**LoCon**