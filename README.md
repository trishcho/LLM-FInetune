# LLM-FInetune


## LLaMA-2 7B Chat Model Fine-Tuning with LoRA


![download](https://github.com/user-attachments/assets/ccaab291-4f76-4802-ad5d-0552796780ec)
![download2](https://github.com/user-attachments/assets/5708bdbf-5649-4d85-b2a6-f9a6a9b10389)




This repository contains the fine-tuned version of the LLaMA-2 7B Chat model using the timdettmers/openassistant-guanaco dataset. 

The model has been fine-tuned using the LoRA (Low-Rank Adaptation) technique to optimize performance while maintaining lower memory and computational requirements. 

### The fine-tuned model is stored in the Hugging Face repository 

codertrish/Llama-2-7b-chat-finetune.

### Model Overview

Pre-trained Model
The model that was fine-tuned is based on

Base model: NousResearch/Llama-2-7b-chat-hf
Dataset used for fine-tuning: mlabonne/guanaco-llama2-1k


Fine-tuned Model
The fine-tuned model is available as:

Fine-tuned model name: codertrish/Llama-2-7b-chat-finetune

### Loading the Model
To load the fine-tuned model and tokenizer:

from transformers import AutoTokenizer, AutoModelForCausalLM

tokenizer = AutoTokenizer.from_pretrained("codertrish/Llama-2-7b-chat-finetune")
model = AutoModelForCausalLM.from_pretrained("codertrish/Llama-2-7b-chat-finetune")


### Acknowledgments
Dataset: timdettmers/openassistant-guanaco
Hugging Face model: codertrish/Llama-2-7b-chat-finetune
