# LlamaFineTuning

This project fine-tunes a TinyLlama (or similar LLaMA-style) language model using the Hugging Face Transformers and PEFT/LoRA stack. The notebook walks through loading a base model, preparing a dataset, configuring training, and saving the final fine-tuned checkpoint and tokenizer.

## Features

- Loads a TinyLlama-style base model and tokenizer from Hugging Face.
- Applies parameter-efficient fine-tuning (LoRA/PEFT) to reduce GPU memory usage.
- Preprocesses text data into chat-style prompts and tokenized inputs. 
- Trains the model with `transformers.Trainer` and logs training loss over multiple epochs and steps.
- Saves the fine-tuned model and tokenizer to a local directory for later inference.

## Directory structure

- `LlamaFineTuning.ipynb` – Main notebook containing all code for data loading, training, and evaluation.
- 
## Requirements

Install the required Python packages (adjust versions as needed):

- Python 3.10+
- `torch` with GPU support
- `transformers`
- `datasets`
- `accelerate`
- `peft`
- `bitsandbytes` (if using 4-bit or 8-bit quantization)
- `sentencepiece`

