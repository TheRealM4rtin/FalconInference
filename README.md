# Text Generation with Quantization & Falcon-7B

This repository contains code for text generation using a language model with quantization. It utilizes the Hugging Face Transformers library to implement a text generation pipeline. Additionally, the model in this repository is quantized using the BitsAndBytes library, which allows for reduced memory and computational requirements while maintaining performance.

## Introduction

Quantization is a technique used to reduce the precision of numerical values in a model. 
➜ This involves lowering the number of bits used to represent model parameters and activations. 
By quantizing the model, we can significantly reduce its memory footprint and speed up inference without sacrificing the overall performance.

## Inference Model

The text generation pipeline in this repository uses the pre-trained language model "falcon-7b-instruct" from the Hugging Face model hub. 
➜ The model has been quantized using the BitsAndBytes library to load parameters and activations in 4-bit format, enabling more efficient computation.

The text generation pipeline takes a query as input and generates coherent text based on the prompt. ➜ The generated text can be controlled using parameters like `max_length`, `top_k`, and `num_return_sequences`.

## Installation

To run the text generation pipeline with quantization, follow these steps:

1. Install the required packages:

```shell
pip install transformers einops accelerate bitsandbytes
```

2. Clone this repo:

```shell
git clone https://github.com/TheRealM4rtin/FalconInference.git
cd FalconInference
```

3. Run

## Usage

To generate text using the provided code, you can follow the example provided in the Python script. The `prompt` function allows you to input your query, and the model will generate corresponding text based on that prompt.

The text generation pipeline can be further customized by adjusting parameters like `max_length`, `top_k`, and `num_return_sequences` to control the length and diversity of the generated text.
