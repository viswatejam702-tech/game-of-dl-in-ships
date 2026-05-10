🚢 DeepShip: Maritime Vessel Classification
📌 Project Overview
DeepShip is a high-performance Computer Vision pipeline designed to classify maritime vessels into five distinct categories: Cargo, Military, Carrier, Cruise, and Tankers. Leveraging Transfer Learning via the ResNet-18 architecture, this project automates the identification of ships from satellite and coastal surveillance imagery—a critical task for maritime traffic management, port security, and environmental monitoring.

🛠 Tech Stack
Deep Learning Framework: PyTorch

Architecture: ResNet-18 (Pre-trained on ImageNet)

Data Manipulation: Pandas, NumPy

Visualization: Matplotlib, Seaborn

Image Processing: PIL (Pillow), Torchvision

📊 Analytical Pipeline
The project is structured into 15+ modular stages to ensure data integrity and model robustness:

Metadata Integration: Merging disparate test and sample submission files into a unified master ledger.

Semantic Mapping: Translating numerical class IDs into descriptive maritime labels.

Exploratory Data Analysis (EDA): Deep dive into class distribution, filename complexity, and format consistency.

Advanced Augmentation: Implementation of RandomResizedCrop, HorizontalFlip, and ColorJitter to simulate varying oceanic lighting and weather conditions.

Transfer Learning: Re-architecting the Fully Connected (FC) layer of ResNet-18 for 5-way softmax classification.

Performance Dashboard: A unified visual summary of data health and model metrics.

🚀 Key Features
Zero-Footprint Data Cleaning: Automated duplicate detection and stratification logic.

Custom Dataset Engine: Memory-efficient DataLoader implementation using PyTorch Dataset class.

Inference Pipeline: A ready-to-use function for predicting ship types from single raw images.

Portfolio Dashboard: High-impact visualizations designed for dark-themed IDEs.

📁 Project Structure
Bash

├── Game of dl in ships.ipynb   # Main Jupyter Notebook with 17-cell analysis
├── master_ship_data.csv        # Integrated metadata file
├── ship_model_final.pth        # Trained model weights (state_dict)
├── test_ApKoW4T.csv            # Original image registry
└── sample_submission_ns2btKE.csv # Target format schema
📈 Results & Insights
The model utilizes a stratified split to maintain class balance across training and validation sets. Initial analysis identifies Cargo ships as the most frequent class, while Carriers represent a rare class, necessitating specific augmentation techniques to prevent model bias.

🔧 Installation & Usage
Clone the repository:

Bash

git clone https://github.com/yourusername/DeepShip.git
Install dependencies:

Bash

pip install torch torchvision pandas matplotlib seaborn scikit-learn pillow
Run the analysis: Open Game of dl in ships.ipynb in Jupyter or VS Code and execute the master cell.

📜 License
Distributed under the MIT License. See LICENSE for more information.

Commit Suggestion
docs: add professional README with architecture and analysis details
