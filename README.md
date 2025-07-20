# mlops-artifact-pipeline

# Clone locally:

     git clone https://github.com/chndsrnvs/mlops-artifact-pipeline.git
     cd mlops-artifact-pipeline
Download anocoda - https://www.anaconda.com/download and follow on screen instructions to install it
# Create Conda Environment & Install Dependencies
   Create environment:
   
      conda create -n mlops python=3.8 -y
      conda init
      conda activate mlops
   requirements.txt:

      scikit-learn
      joblib
      pytest
   Install requirements:
   
      pip install -r requirements.txt
# Project Structure

    mlops-artifact-pipeline/
    ├── src/
    │   ├── train.py
    │   ├── inference.py
    │   └── utils.py
    ├── config/
    │   └── config.json
    ├── tests/
    │   └── test_train.py
    ├── .github/
    │   └── workflows/
    │       ├── train.yml
    │       ├── test.yml
    │       └── inference.yml
    ├── requirements.txt
    └── README.md
# Branching Strategy

      main: Initial branch with only README.
      classification: For training code/workflows.
      test: For unit tests and testing workflow.
      inference: For inference script and full pipeline workflow.
