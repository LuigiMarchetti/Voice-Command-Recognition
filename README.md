# 🤖🎤 Voice Command Recognition System

A comprehensive machine learning project implementing multiple state-of-the-art algorithms for real-time voice command recognition. This repository demonstrates expertise in audio processing, machine learning model development, and comparative algorithm analysis.

## Project Overview

This project develops and compares **four distinct machine learning approaches** to classify voice commands from short audio samples. Each algorithm brings unique advantages, allowing for performance trade-offs between accuracy, speed, and resource efficiency.

### Key Capabilities

- **Multiple Algorithm Implementations**: Neural Networks, K-Nearest Neighbors (KNN), Support Vector Machines (SVM), and academic research algorithms
- **Real-Time Voice Simulation**: Integrated robotic simulation for live command recognition testing
- **Comprehensive Dataset**: Built on the Speech Commands Dataset v0.02, supporting 8 command classes (forward, backward, left, right, yes, no, stop)
- **Production-Ready Models**: Pre-trained and optimized models with label mapping for immediate deployment
- **Custom Validation Data**: Real-world recordings from team members for practical testing and validation

---

## Project Structure

### `Algorithms/` — Core Machine Learning Implementations

Each algorithm is independently implemented and tested, allowing for easy comparison and benchmarking:

| Algorithm | Description | Best For |
|-----------|-------------|----------|
| **Neural Network** | Deep learning approach with convolutional architecture | High accuracy, complex patterns |
| **SVM** | Support Vector Machine classifier | Robust performance, smaller datasets |
| **KNN** | K-Nearest Neighbors classifier | Simplicity, baseline comparison |
| **Artigo 1** | Research paper-based methodology | Academic rigor, published methods |

- Each algorithm folder contains:
  - `__init__.py` — Main implementation
  - `test.py` — Unit tests and benchmarks
  - `robo.py` (in Artigo 1) — Real-time simulation with live voice command listening

### `files/` — Data, Models & Documentation

#### `dataset/` 
- Speech Commands Dataset v0.02 with 8 command classes
- Organized by command type: `forward/`, `backward/`, `left/`, `right/`, `yes/`, `no/`, `stop/`
- Background noise samples for robust testing
- Training and validation split lists

#### `models/`
- **Pre-trained Models**: Fully trained and ready for inference
  - TensorFlow models (`.pt` files)
  - SVM joblib serialization (`.joblib` files)
  - Label mappings (`.json` files)
- **Specialized Variants**: Yes/No binary classification models for focused applications
- Organized by algorithm for easy access and deployment

#### `docs/`
- Academic paper (IEEE SBC format, 5 pages)
- Seminar presentation (PowerPoint)

#### `recorded/`
- Real-world test recordings from team members
- Raw `.wav` files organized by contributor for validation and overfitting detection

---

## Getting Started

### Prerequisites
- Python 3.7+
- Required libraries: scikit-learn, torch, numpy, scipy

### Running Tests
```bash
# Test Neural Network implementation
python Algorithms/Neural\ Network/test.py

# Test SVM implementation
python Algorithms/SVM/test.py

# Test KNN implementation
python Algorithms/KNN/test.py

# Run real-time voice simulation
python Algorithms/Artigo\ 1/robo.py
```

### Using Pre-trained Models
- Load any `.pt` or `.joblib` file from `files/models/` for immediate inference
- Refer to corresponding `label_mapping.json` for command-to-label translation

---

## Technical Highlights

✅ **Comparative Analysis**: Four different algorithms evaluated on identical datasets  
✅ **Production Models**: Serialized, deployable models ready for integration  
✅ **Real-Time Capabilities**: Live listening simulation for interactive testing  
✅ **Robust Testing**: Custom recordings and validation sets for real-world scenarios  
✅ **Academic Foundation**: Research-backed methodology with published documentation  

---

## Dataset Information

For detailed dataset specifications and download instructions, see [files/dataset/README.md](files/dataset/README.md)

---

## License

See [LICENSE](LICENSE) for details 