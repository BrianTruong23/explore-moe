# Simple Mixture of Experts (MOE) Model for Multi-Task Learning

This project implements and explores a simple Mixture of Experts (MOE) model, focusing on expert network allocation and efficiency. The model is designed to improve task distribution and accuracy, making it suitable for handling diverse inputs in multi-task learning scenarios.

## Project Overview

- **Technical Expertise:** Development and testing of a simple MOE model
- **Model Optimization:** Improved efficiency and accuracy in task distribution
- **Research Contribution:** Enhanced understanding of MOE models' applications, particularly in multi-task learning
- **Potential Applications:** Useful for NLP tasks such as translation and summarization, adaptable to various machine learning problems

## Key Findings

### Model Performance:

- 4 simple experts with 256 hidden dimensions: 58.09% accuracy
- 10 simple experts with 512 hidden dimensions: 50.26% accuracy
- **Conclusion:** Increasing the number of experts and dimensions does not necessarily improve accuracy

### Optimization Techniques:

- Dropout implementation improved accuracy to 66.6%
- 4 experts with 256 hidden dimensions produced comparatively good results

### Advanced Architectures:

- Incorporating RNN and CNN experts did not significantly increase accuracy
- Best accuracy achieved with advanced layers: 66.42% (using 4-6 experts)

## Implementation Details

- **Environment:** Google Colab with GPU acceleration
- **Libraries:** PyTorch, Transformers, Datasets, Matplotlib
- **Dataset:** GLUE MRPC (Microsoft Research Paraphrase Corpus)
- **Model Architecture:** Customizable number of experts, gating network, and output layer

## Future Work

- Further exploration of optimal expert numbers and dimensions
- Investigation of alternative expert architectures
- Application to different NLP tasks and datasets

## Getting Started

To get started with this project, follow the instructions below:

### Setup

1. **Clone the Repository:** `git clone <repository-link>`
2. **Install Dependencies:** `pip install -r requirements.txt`
3. **Open the Colab Notebook:** Use the provided link to open and run the notebook in Google Colab with GPU acceleration.

### Running the Model

1. **Prepare the Dataset:** Ensure the GLUE MRPC dataset is available and properly formatted.
2. **Train the Model:** Execute the training scripts in the Colab notebook to train the MOE model.
3. **Evaluate Performance:** Analyze the model's performance using the provided evaluation metrics and visualizations.

## Contributing

Contributions to improve the model or extend its applications are welcome. Please feel free to submit issues or pull requests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

---
