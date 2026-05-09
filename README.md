# Multi-Angle Mosquito Species Dataset

This repository hosts a specialized image dataset of disease-carrying mosquitoes, used in the study **"A Framework for Anatomy Extraction and Classification of Mosquito Images with a Deep Learning Approach"** (*Journal of Modeling in Engineering*, 2022).

The dataset is unique because it includes images captured from **various angles**, providing a comprehensive morphological view of each specimen to improve the robustness of deep learning classification and segmentation models.

## 📊 Dataset Composition

The dataset contains a total of **594 samples** across three primary genera, with detailed geographical sub-categories for *Anopheles*.

| Genus | Sub-category / Location | Samples |
| --- | --- | --- |
| **Culex** | General | 86 |
| **Aedes** | General | 67 |
| **Anopheles** | Bandar-Abbas | 160 |
| **Anopheles** | Chabahar | 216 |
| **Anopheles** | Kazeroon | 65 |
| **Total** |  | **594** |

## 📸 Imaging Characteristics

Unlike standard datasets that may rely on a single top-down view, this collection features:

* **Diverse Perspectives:** Images taken from multiple angles (dorsal, lateral, and ventral) to ensure the model learns to identify anatomical features regardless of the mosquito's orientation.
* **Anatomical Focus:** Specifically curated to support the extraction and identification of the **Thorax, Abdomen, Wings, and Legs**.
* **High Variability:** The inclusion of different viewpoints helps in training models that are resilient to the practical challenges of field-captured images.

## 🧠 Research Application

This data was used to validate a framework combining **Mask R-CNN** and **ResNet101**. By segmenting the mosquito into its anatomical components rather than treating the image as a single unit, the associated research achieved a classification accuracy of **97.84%**.

## 📂 Data Structure

```text
├── dataset/
│   ├── Culex/              # Images from various angles
│   ├── Aedes/              # Images from various angles
│   └── Anofel/
│       ├── Bandar-Abbas/   # Regional variants
│       ├── Chabahar/
│       └── Kazeroon/
├── annotations/            # Segmentation masks and labels
└── README.md

```

## 📝 Citation

If you utilize this dataset in your research, please cite the original publication:

```bibtex
@article{zare2022mosquito,
  title={A Framework for Anatomy Extraction and Classification of Mosquito Images with a Deep Learning Approach},
  author={Zare Nazari, Marzieh and Sardari Zarchi, Mohsen and Emadi, Sima and Pourmohammadi, Hadi},
  journal={Journal of Modeling in Engineering},
  volume={20},
  number={70},
  pages={107--120},
  year={2022},
  publisher={Semnan University},
  doi={10.22075/jme.2022.26235.2222}
}

```

## 📜 License

[Insert License Type, e.g., MIT or CC BY 4.0]
