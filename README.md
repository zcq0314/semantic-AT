# SADAT: Semantic-Aware Dual-Granularity Adversarial Training

This repository provides the official implementation of **SADAT**, a Semantic-Aware Dual-Granularity Adversarial Training framework proposed for improving the adversarial robustness of Chinese NLP models. 

## Directory Structure

```
SADAT/
├── sadat.py                    # Main training class with SADAT implementation
├── run_sadat.py                # Main program to run
├── candidate_pool.py           # candidate pool generation
├── sparse_delta.py             # Gradient Sparse perturbation
├── homologous.py               # Perturbation operations
└── transform.py                # Transform token to another character\word
```



## Usage

```bash
# Example training command
python run_sadat.py \
  --task_name task_name \
  --output_dir outputs \
  --load_model_path model_path \
  --data_dir data_dir \
  --sadat
```

## Dependencies

* Python ≥ 3.8
* PyTorch ≥ 1.10
* HuggingFace Transformers
* scikit-learn
* jieba
* HowNet Toolkit (for Chinese synonym mining)

Install dependencies via:

```bash
pip install -r requirements.txt
```

