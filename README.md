# Hybrid Fake News Detection Model

A hybrid deep learning model for fake news detection using BERT and BiLSTM with attention mechanism.

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
│   └── utils/        # Utility functions
├── tests/            # Unit tests
└── notebooks/        # Jupyter notebooks
```

## Features

- Hybrid architecture combining BERT and BiLSTM
- Attention mechanism for better interpretability
- Comprehensive text preprocessing pipeline
- Support for multiple feature extraction methods
- Early stopping and model checkpointing
- Detailed evaluation metrics

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

1. Prepare your dataset:
   - Place your dataset in the `data/raw` directory
   - The dataset should have at least two columns: 'text' and 'label'

2. Train the model:
```bash
python src/train.py
```

3. Model evaluation metrics will be logged during training

## Model Architecture

The model combines:
- BERT for contextual embeddings
- BiLSTM for sequence modeling
- Attention mechanism for focusing on important parts
- Classification head for final prediction

## Configuration

Key parameters can be modified in `src/config/config.py`:
- Model hyperparameters
- Training parameters
- Data processing settings
- Feature extraction options

## Future Improvements

- [ ] Add support for image/video metadata
- [ ] Implement real-time detection
- [ ] Add social graph analysis
- [ ] Improve model interpretability
- [ ] Add API endpoints for inference

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details. 