# Hybrid Fake News Detection Model

A hybrid deep learning model for fake news detection using BERT and BiLSTM with attention mechanism. This project was developed as part of the Data Mining Laboratory course under the guidance of Dr. Kirti Kumari.

## Project Overview

This project implements a state-of-the-art fake news detection system that combines the power of BERT (Bidirectional Encoder Representations from Transformers) with BiLSTM (Bidirectional Long Short-Term Memory) and attention mechanisms. The model is designed to effectively identify fake news articles by analyzing their textual content and linguistic patterns.

## Data and Model Files

The project uses the following datasets and model files:

### Datasets
- Raw and processed datasets are available at: [Data Files](https://drive.google.com/drive/folders/1uFtWVEjqupSGV7_6sYAxPG52Je1MAigh?usp=sharing)
  - Contains both raw and processed versions of the datasets
  - Includes LIAR and Kaggle Fake News datasets
  - Preprocessed versions ready for training

### Model Files
- Trained model checkpoints are available at: [Model Files](https://drive.google.com/drive/folders/1d1EXjLlYof56yEa9F6qFDPKqO359vnRw?usp=sharing)
  - Contains saved model weights
  - Includes best model checkpoints
  - Model evaluation results

## Project Structure

```
.
├── data/
│   ├── raw/           # Raw datasets
│   └── processed/     # Processed data
├── models/
│   ├── saved/        # Saved model checkpoints
│   └── checkpoints/  # Training checkpoints
├── src/
│   ├── config/       # Configuration files
│   ├── data/         # Data processing modules
│   ├── models/       # Model architecture
│   ├── utils/        # Utility functions
│   └── visualization/# Visualization modules
├── tests/            # Unit tests
├── notebooks/        # Jupyter notebooks
└── visualizations/   # Generated plots and graphs
```

## Features

- Hybrid architecture combining BERT and BiLSTM
- Attention mechanism for better interpretability
- Comprehensive text preprocessing pipeline
- Support for multiple feature extraction methods
- Early stopping and model checkpointing
- Detailed evaluation metrics
- Interactive visualizations of model performance
- Support for multiple datasets (LIAR, Kaggle Fake News)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/fake-news-detection.git
cd fake-news-detection
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Download the required files:
   - Download datasets from the [Data Files](https://drive.google.com/drive/folders/1uFtWVEjqupSGV7_6sYAxPG52Je1MAigh?usp=sharing) link
   - Download pre-trained models from the [Model Files](https://drive.google.com/drive/folders/1d1EXjLlYof56yEa9F6qFDPKqO359vnRw?usp=sharing) link
   - Place the files in their respective directories as shown in the project structure

2. Prepare your dataset:
   - Place your dataset in the `data/raw` directory
   - The dataset should have at least two columns: 'text' and 'label'
   - Supported formats: CSV, TSV

3. Train the model:
```bash
python src/train.py
```

4. Model evaluation metrics and visualizations will be generated in the `visualizations` directory

## Model Architecture

The model combines:
- BERT for contextual embeddings
- BiLSTM for sequence modeling
- Attention mechanism for focusing on important parts
- Classification head for final prediction

### Key Components:
- **BERT Layer**: Extracts contextual word embeddings
- **BiLSTM Layer**: Captures sequential patterns
- **Attention Layer**: Identifies important text segments
- **Classification Head**: Makes final prediction

## Configuration

Key parameters can be modified in `src/config/config.py`:
- Model hyperparameters
- Training parameters
- Data processing settings
- Feature extraction options

## Performance Metrics

The model is evaluated using:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

## Future Improvements

- [ ] Add support for image/video metadata
- [ ] Implement real-time detection
- [ ] Add social graph analysis
- [ ] Improve model interpretability
- [ ] Add API endpoints for inference
- [ ] Support for multilingual fake news detection
- [ ] Integration with fact-checking databases

## Acknowledgments

I would like to express our sincere gratitude to **Dr. Kirti Kumari** for her invaluable guidance and support throughout the development of this project. Her expertise in data mining and machine learning has been instrumental in shaping this work.

Special thanks to:
- Open-source community for their excellent tools and libraries
- Dataset providers (LIAR, Kaggle)

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

For any queries or suggestions, please feel free to reach out to me. 