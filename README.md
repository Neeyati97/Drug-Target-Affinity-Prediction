**💊 Drug-Target Affinity Prediction**

Developed by: Neeyati Vijjeswarapu

**🧠 Overview**

This project utilizes Graph Neural Networks (GNNs)—specifically the GraphSAGE architecture—to predict the binding affinity between drug molecules and target proteins. The model is trained on the KIBA dataset and deployed as a user-friendly Flask web application, enabling real-time predictions via drug and protein name inputs.

**🚀 Project Highlights**

- Model Type: Graph Neural Network (GraphSAGE)
- Dataset: KIBA – Kinase Inhibitor BioActivity
- Deployment: Flask Web App
- APIs Used: PubChem, UniProt

**🧪 Performance Metrics**

| Metric                 | Value   |
|------------------------|---------|
| Mean Squared Error     | 0.0859  |
| Root Mean Squared Error| 0.2931  |
| Mean Absolute Error    | 0.1961  |
| R² Score               | 0.8792  |
| Pearson Correlation    | 0.9381  |
| Spearman Correlation   | 0.9094  |

**🧬 Input Handling**

- Drug Name → SMILES: Fetched via PubChem REST API
- Protein Name → Sequence: Retrieved via UniProt REST API

**🌐 Web Application**

**🔧 How to Run**

1. Install dependencies

   > pip install -r requirements.txt

2. Start the Flask server

   > python app.py

3. Visit in browser

   > http://127.0.0.1:5000/

**💡 How to Use**

- Input:

   - Drug Name (e.g., Palbociclib)
   - Protein Name (e.g., HER2)

- Output:

   - Affinity Score (numeric)
   - Affinity Percentage

- Affinity Category (Low, Moderate, High)

**📁 Directory Structure**

├── pycache/                # Compiled Python files

├── data/                   # Raw and processed datasets

├── model/                  # GraphSAGE model architecture

├── models/                 # Saved model checkpoints (.pth)

├── plots/                  # Evaluation metric visualizations

├── static/                 # Static assets (CSS, images)

├── templates/              # HTML templates for Flask

├── utils/                  # API and preprocessing utilities

├── executed_outputs/       # Screenshots and demo videos

├── app.py                  # Flask app main file

├── evaluate.py             # Evaluation script

├── generate_graph_data.py  # Convert raw input to graph format

├── graphsage_affinity_model.pth  # Trained model weights

├── predict.py              # Inference logic

├── train.py                # Model training script

├── requirements.txt        # Python dependencies

**📸 Executed Outputs**

The executed_outputs/ folder contains:

Screenshots demonstrating prediction examples for all affinity levels.
A demo video showcasing the full prediction pipeline and web interface.
