# 📷 Image Classification
A high-performance ML inference API built in C++ with LibTorch for real-time image classification with sub-50ms latency. Deployed on AWS with Docker containerization and auto-scaling to handle 100+ concurrent requests.

## Features
- Real-time image inference using pre-trained LibTorch models
- REST API with JSON responses for classification predictions
- Multi-threaded architecture for concurrent request handling
- Docker containerization for seamless cloud deployment
- Auto-scaling infrastructure on AWS for handling traffic spikes
- Support for multiple image formats

## Tech Stack
- **Language**: C++17
- **ML Framework**: LibTorch
- **API**: REST APIs (Crow/cpp-httplib)
- **Deployment**: Docker, AWS EC2
- **Data Format**: JSON

## Getting Started
**Prerequisites**
- C++17 compatible compiler
- LibTorch library
- Docker
- AWS account

**Installation**
```bash
git clone https://github.com/yourusername/image-classification.git
cd image-classification
mkdir build && cd build
cmake ..
make
```
**Setup**
1. Download the pre-trained LibTorch model and place it in the models/ directory
2. Run the application:

```bash
./image_classifier
```
## Usage
- API runs on http://localhost:8080
- Send POST requests to /predict with image files
- Receive JSON responses with classification results and confidence scores
