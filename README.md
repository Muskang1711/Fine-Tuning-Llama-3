# Fine-Tuning Llama 3 Notebooks

This repository contains two Jupyter notebooks for fine-tuning Llama 3 models using different approaches.

## Notebooks

### 1. FineTune-Llama-3-with-SFTTrainer.ipynb
This notebook demonstrates how to fine-tune Llama 3 using Hugging Face's SFTTrainer (Supervised Fine-Tuning Trainer). The SFTTrainer is part of the TRL (Transformer Reinforcement Learning) library and provides a simplified interface for supervised fine-tuning of language models.

**Key Features:**
- Uses Hugging Face Transformers and TRL libraries
- Implements supervised fine-tuning with SFTTrainer
- Suitable for instruction tuning and task-specific adaptation
- Includes data preprocessing and training configuration

### 2. Fine-Tune-Llama3-with-unsloth.ipynb
This notebook shows how to fine-tune Llama 3 using Unsloth, a library designed for efficient and faster fine-tuning of large language models.

**Key Features:**
- Leverages Unsloth for optimized training
- Reduced memory usage and faster training times
- Supports LoRA (Low-Rank Adaptation) and QLoRA techniques
- Ideal for resource-constrained environments

## Requirements

- Python 3.8+
- CUDA-capable GPU (recommended)
- Jupyter Notebook or JupyterLab

## Installation

```bash
# Clone the repository
git clone <repository-url>
cd <repository-name>

# Install required packages
pip install -r requirements.txt
```

## Usage

1. Open the desired notebook in Jupyter:
   ```bash
   jupyter notebook
   ```

2. Follow the step-by-step instructions within each notebook

3. Modify the configuration parameters according to your needs:
   - Dataset path
   - Model parameters
   - Training hyperparameters
   - Output directory

## Dataset Format

Both notebooks expect datasets in a conversational or instruction-following format. Common formats include:
- Alpaca-style format
- ShareGPT format
- Custom JSON/CSV formats

Refer to each notebook for specific data preprocessing steps.

## Notes

- Ensure you have sufficient GPU memory for the model size you're working with
- Consider using gradient checkpointing or quantization for larger models
- Monitor training metrics to avoid overfitting
- Save checkpoints regularly during training

## License

MIT License

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.