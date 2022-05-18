# Visual_Ontology
## Prerequisites
Java 15

Python 2.7, 3.6.2

Backend Frameworks: Flask 1.1.2, Spring Boot 2.4.2

Protege Ontology Editor: OWL DL

OWL Plugins: SWRL, SQWRL, SPARQL

Jena API 3.16.0

CUDA: 9.0

Torch 1.1.0

Torchvision 0.2.0

OS Version: Ubuntu 16.04 LTS

## Steps:

Google drive: https://drive.google.com/drive/folders/1BMh_i_Idncnk44_IjCpUWNSbf2ORFR5u?usp=sharing

Clone this respository.

Download jdk-15.0.2.zip and vis_ont.zip. Extract them in the repository directory. 

Download Revisiting_Single_Depth_Estimation.zip, FactorizableNet.zip and pretrained_model.zip. Extract them to survOntFlaskApp directory.

Run:

```
cd Visual_Ontology/survOntFlaskApp/FactorizableNet/lib
make all
```

This will make all the required libraries for FactorizableNet specific the the current system.
Alternatively, you can also download lib.zip and extract to survOntFlaskApp/FactorizableNet. 

Then open two terminals. On the first terminal, run the backend from MTP_Ontology using:

```
cd Visual_Ontology/MTP_Ontology_Backend
sh backend.sh
```

On the other terminal, Activate the virtual environment and run frontend:

```
cd Visual_Ontology/survOntFlaskApp
source venv2/bin/activate
sh frontend.sh
```

Open a browser and goto the following link to use the app

http://localhost:7000

Upload image and click Upload and run code button.

**Note: Path to repository should not have any spaces for the backend to work.**

## References:
[1] **FactorizableNet:** Li, Yikang, et al. "Factorizable net: an efficient subgraph-based framework for scene graph generation." Proceedings of the European Conference on Computer Vision (ECCV). 2018.

Github: https://github.com/yikang-li/FactorizableNet

[2] **Revisiting Single Image Depth Estimation:** Hu, Junjie, et al. "Revisiting single image depth estimation: Toward higher resolution maps with accurate object boundaries." 2019 IEEE Winter Conference on Applications of Computer Vision (WACV). IEEE, 2019.

Github: https://github.com/JunjH/Revisiting_Single_Depth_Estimation
