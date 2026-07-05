---
base_model: mistralai/Mixtral-8x7B-Instruct-v0.1
library_name: peft
license: apache-2.0
tags:
- adaption
- autoscientist
- peft
- lora
- mixtral
- instruction-tuning
---

# Market Analysis AI - LoRA Adapter

## Model Description

This repository contains a LoRA adapter fine-tuned using Adaption AutoScientist on top of **Mixtral-8x7B-Instruct-v0.1**. The model was trained using Adaption's automated training pipeline and optimized for instruction-following tasks.

### Model Details

- **Developed by:** Tanya Garg
- **Platform:** Adaption AutoScientist
- **Model Type:** LoRA Adapter (PEFT)
- **Base Model:** mistralai/Mixtral-8x7B-Instruct-v0.1
- **Framework:** PEFT
- **License:** Apache-2.0
- **Language:** English

## Training Information

### Dataset ID

```
a91f43bb-3470-4ba6-a054-f3ebef391cf9
```

### Training Model ID

```
adaption_mixtral_8x7b_instruc_missing_input_refusals_645c1458
```

### Training Method

- AutoScientist
- Supervised Fine-Tuning (SFT)
- LoRA Fine-tuning

### Hyperparameters

| Parameter | Value |
|-----------|-------|
| Epochs | 1 |
| Learning Rate | 0.0001 |
| LoRA Rank | 8 |
| LoRA Alpha | 8 |
| Scheduler | Cosine |
| Warmup Ratio | 0.1 |
| Target Modules | q_proj, v_proj |

## Training Results

### Win Rate Improvement

| Metric | Base | Fine-tuned |
|--------|------|------------|
| Dataset Win Rate | 40% | 61% |
| General Win Rate | 36% | 64% |

The model demonstrated a measurable improvement over the baseline after AutoScientist optimization.

## Intended Use

This model is intended for:

- Instruction following
- Research
- Educational purposes
- Fine-tuning experiments

## Repository Contents

- adapter_model.safetensors
- adapter_config.json
- tokenizer.json
- tokenizer_config.json
- config.json
- trainer_state.json

## Acknowledgements

This project was developed as part of the **Adaption AutoScientist Challenge** in partnership with **HackIndia**.

Base Model:
https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1

## Citation

If you use this model, please cite the Adaption AutoScientist Challenge and the Mixtral base model.
