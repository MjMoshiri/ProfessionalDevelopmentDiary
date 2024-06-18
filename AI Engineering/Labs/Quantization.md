# Quantization

## Techniques to Reduce Model Size

- **Pruning**: Removing unnecessary weights from the model.
- **Downsampling**: Reducing the size of the input data. (f32 to f16)
- **Linear Quantization**: Reducing the number of bits used to represent the weights and activations. (fit values into a smaller range)
- **Knowledge Distillation**: Training a smaller model to mimic the behavior of a larger model. (Instructor-Student method)

## Keywords

- **LLM.INT8**
- **QLoRA** Quantization and Low-Rank Adapters LoRA
- **AWQ** Activation-aware Weight Quantization
- **GPTQ** GPT Quantized
- **SmoothQuant** 
- **AQLM** Additive Quantization of Language Models
- **HQQ** Half Qaudratic Quantization
- **QUIP** 

- **PEFT** Parameter-Efficient Fine-Tuning