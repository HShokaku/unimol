# Personal usage of UniMol
This repository is a personal usage of [UniMol](https://github.com/deepmodeling/Uni-Mol)

## 🔧 Environment Setup
```bash
mamba create -n unimol python==3.10
mamba activate unimol
pip install torch --index-url https://download.pytorch.org/whl/cu121
pip install rdkit==2022.9.5
pip install unimol_tools
pip install huggingface_hub

# Download the pretrained model
export HF_ENDPOINT=https://hf-mirror.com
huggingface-cli download --resume-download dptech/Uni-Mol-Models --local-dir path/to/your/conda/envs/unimol/lib/python3.10/site-packages/unimol_tools/weights --local-dir-use-symlinks False
```