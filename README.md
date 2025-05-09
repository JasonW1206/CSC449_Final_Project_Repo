# Explicit-Content-Detection-in-Images

Automated detection of explicit imagery is a critical component of modern content moderation, forensic investigation, and child protection. Over the past three
decades, research in this field has advanced from heuristic skin filters and classical
machine learning to deep convolutional neural networks, region-aware detectors,
and emerging multimodal approaches. Yet, the deployment of such systems raises
substantial challenges involving fairness, legal compliance, dataset ethics, and
human reviewer well-being. This survey provide general reviews on explicit image
detection, classification, and identification. It organizes the past literature along
three axes: algorithmic technique, application domain, and ethical and regulatory framing. For each axis, it examines the evolution of methods, benchmark
limitations, and contextual trade-offs. This survey provides a balanced synthesis
that integrates technical advances with legal constraints and social impact. It outlines open research questions in benchmark design, fairness auditing, multimodal
modeling, and trauma-aware system design. This survey is to provide a comprehensive reference for researchers, developers, and policymakers working on safe
and accountable visual AI systems.

## table of contents

* [datasets](https://github.com/JasonW1206/CSC449_Final_Project_Repo#datasets)
* [related works](https://github.com/JasonW1206/CSC449_Final_Project_Repo#techniques)

## datasets

| name | paper/url | year | size | task | labels |
|--- |--- |--- |--- |--- |--- |
| LSPD | [paper](https://inass.org/wp-content/uploads/2021/09/2022022819-4.pdf) | 2022 | 50,000 images | Binary Classification | Porn, Normal, Sexy, Hentai, Drawings |
| NudeNet | [github](https://github.com/notAI-tech/NudeNet) | 2019 | ~20GB images | Multi-class | Safe, Sexy, Nude |
| Adult dataset | [Paper](https://arxiv.org/abs/1612.09506) | 2017 | 81,306 images| Multi-class | Safe, Adult |

## techniques

| Paper Name | url | Algorithmic Class | Method | Dataset | Task | Reported Matrix |
|--- |--- |--- |--- |--- |--- |--- |
| Obscene image detection algorithm using high- and low-quality images | [paper](https://ieeexplore.ieee.org/document/5488562) | Heuristic | Skin color threshold dectection | custom 1k web images | binary classification | Acc: 86.8% |
| IMAGE GUARDER: AN INTELLIGENT DETECTOR FOR ADULT IMAGES | [paper](https://www.researchgate.net/publication/246418434_IMAGE_GUARDER_AN_INTELLIGENT_DETECTOR_FOR_ADULT_IMAGES) | Machine Learning | Support Vector Machine for skin detection | Custom 121k images | binary classification | Acc: 95.5% |
| four-phases methodology to pro-pose anti-pornography system based on neural and Bayesian methods of artificial intelligence. | [paper](https://www.worldscientific.com/doi/abs/10.1142/S0218001414590010) | Machine Learning | Skin segmentation + Bayesian classifier | Custom images | binary classification | TPR: 96.0% |
| Using transfer learning to classify pornographic images | [paper](https://ieeexplore.ieee.org/document/9044231) | Deep CNN | ResNet | Custom dataset | binary classification | Acc: 97.1% |
| A Novel Pornographic Visual Content Classifier based on Sensitive Object Detection | [paper](https://thesai.org/Downloads/Volume12No5/Paper_91-A_Novel_Pornographic_Visual_Content_Classifier.pdf) | Deep CNN | YOLOv3 | Custom 100k images | binary classification | Acc: 94.0% |
|Pornographic Image Recognition via Weighted Multiple Instance Learning |[paper](https://arxiv.org/abs/1902.03771) |Deep MIL | Weighted MIL under CNN |Custom 200k images | binary classification |TPR: 97.5% |
|Multilevel fusion of multimodal deep features for porn streamer recognition in live video |[paper](https://www.sciencedirect.com/science/article/pii/S0167865520303469) |Multimodal |BERT + multiple CNNs | Custom live-stream dataset |multi-class classification |Acc: 82.3% |
