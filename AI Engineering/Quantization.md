# Quantization
[**Fundamentals**](https://learn.deeplearning.ai/courses/quantization-fundamentals)
[**In Depth**](https://learn.deeplearning.ai/courses/quantization-in-depth)


## General Idea
- **Pruning**: Removing unnecessary weights from the model.
- **Downsampling**: Reducing the size of the input data. (f32 to f16)
- **Linear Quantization**: Reducing the number of bits used to represent the weights and activations. (fit values into a smaller range)
- **Knowledge Distillation**: Training a smaller model to mimic the behavior of a larger model. (Instructor-Student method)

## Keywords
- **Symmetric Quantization**: The range of values is divided into equal parts, with zero in the middle. (Simpler, need less space)
- **Asymmetric Quantization**: The range of values is divided into parts, with zero not necessarily in the middle.
- **Per Channel, Group, Layer**: Quantization can be applied to different parts of the model.
- **Weight Packing**: Combining multiple weights into a single value.
- **PEFT** Parameter-Efficient Fine-Tuning


## Papers
- **LLM.INT8**
- **QLoRA** Quantization and Low-Rank Adapters LoRA
- **AWQ** Activation-aware Weight Quantization
- **GPTQ** GPT Quantized
- **SmoothQuant** 
- **AQLM** Additive Quantization of Language Models
- **HQQ** Half Qaudratic Quantization
- **QUIP** 
## More Resources

- [**MIT Han Lab**](https://hanlab.mit.edu/)
- [**Reddit Local Llama**](https://www.reddit.com/r/LocalLLaMA/)

**Tags**: Machine Learning, AI