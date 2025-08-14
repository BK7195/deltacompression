# Delta Compression: An Efficient Lossless Compression Method Using Hypernetwork-Generated Parameter Deltas

This is the official repository for the paper: "Delta Compression: An Efficient Lossless Compression Method Using Hypernetwork-Generated Parameter Deltas".

This repository provides the source code and data to reproduce the experiments presented in the paper using Google Colab.

## Abstract

This paper proposes "Delta Compression," a novel method for achieving efficient lossless compression by encoding information as a hypernetwork-generated parameter delta rather than static data. When applied to a shared, deterministic base model trained for reconstructive decoding, this delta enables perfect recovery of the original input. Our proof-of-concept successfully encoded 978 KB of text data into a single LoRA adapter and restored it with complete fidelity.

## Paper
[Published on Zenodo](https://zenodo.org/records/16870406)

## How to Run the Experiments (Google Colab)

The easiest way to reproduce our results is by using Google Colab. No local setup is required.

### 1B Model Experiment (cyberagent/open-calm-1b)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BK7195/deltacompression/blob/main/1B_open-calm/run_deltacompression_1B.ipynb)

1.  **Open the Notebook:** Click the "Open In Colab" button above.
2.  **Download Data:** Download the supplementary data file here: **[supplementary1B.zip](https://github.com/BK7195/deltacompression/raw/main/supplementary1B.zip)**
3.  **Run and Upload:** In the Colab notebook, run the cells from the top. You will be prompted to upload the `supplementary1B.zip` file you just downloaded.

**Note:** The full fine-tuning process takes approximately **4 hours** on a standard Colab GPU. It is recommended to review the notebook's structure and outputs before running the entire process.

### 8B Model Experiment (Meta-Llama-3-8B)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BK7195/deltacompression/blob/main/8B_llama3/run_deltacompression_8B.ipynb)

1.  **Open the Notebook:** Click the "Open In Colab" button above.
2.  **Download Data:** Download the supplementary data file here: **[supplementary8B.zip](https://github.com/BK7195/deltacompression/raw/main/supplementary8B.zip)**
3.  **Run and Upload:** In the Colab notebook, follow the instructions to upload the `supplementary8B.zip` file when prompted.

**Note:** The full fine-tuning process is computationally intensive and takes approximately **23 hours** on a standard Colab GPU. We recommend reviewing the notebook's logic and outputs before committing to a full run.

## License
This project is licensed under the Apache 2.0 License. See the `LICENSE` file for details.

## Citation
If you find this work useful, please cite our paper:

```bibtex
@misc{BK7195_DeltaCompression_2025,
  author       = {Kazunori Kondo},
  title        = {Delta Compression: An Efficient Lossless Compression Method Using Hypernetwork-Generated Parameter Deltas},
  year         = {2025},
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.16870406},
  url          = {[https://zenodo.org/records/16870406](https://zenodo.org/records/16870406)}
}
