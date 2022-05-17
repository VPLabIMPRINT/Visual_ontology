# Visual_Ontology

Google drive: https://drive.google.com/drive/folders/1Qx32_feo6rWlZNL3Y1dAyHck5XtTZdYn

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
