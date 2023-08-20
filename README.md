# NeRFs-Datasets
**Contains almost all NeRFs datasets, about types, formats and links.**

In recent years, NeRF has developed rapidly, and various iterative methods and technologies have also shown their prowess. 
Along with it, a large number of corresponding data sets have also appeared. 
In order to facilitate the distinction and use, this paper classifies most of the data sets related to NeRF.
If there is anything missing, welcome to contribute

# 1 Static scenes
## 1.1 synthetic single object
https://github.com/lixiaojie-thu/NeRFs-Datasets/assets/40080699/9a3f7cb5-3dc8-429f-a647-f2ec0d72bedc
### format
    dataset
        ├── train
        │   └── r_x.png
        ├── test
        │   ├── r_x.png
        │   ├── r_x_depth.png
        ├── val
        │   ├── r_x.png
        ├── transforms_train.json
        ├── transforms_test.json
        ├── transforms_val.json
see more [NeRF](https://github.com/bmild/nerf#generating-poses-for-your-own-scenes)
### datasets
- [2020-NeRF](https://drive.google.com/drive/folders/1JDdLGDruGNXWnM1eqY1FNL9PlStjaKWi)
- [2023-OmniObject3D](https://opendatalab.com/OpenXD-OmniObject3D-New/download)

## 1.2 realistic single object
### format
### datasets
- [2023-OmniObject3D](https://opendatalab.com/OpenXD-OmniObject3D-New/download)

## 1.3 forward facing scenes
https://github.com/lixiaojie-thu/NeRFs-Datasets/assets/40080699/e8ef1ca7-4b89-4dab-8421-b9eb4ed686c1
### format
    dataset
        ├── images
        │   └── img_x.jpg
        ├── images_4
        │   ├── img_x.jpg
        ├── images_8
        │   ├── img_x.jpg
        ├── spare
            ├── 0
                ├── cameras.bin
                ├── images.bin
                ├── points3D.bin
                ├── project.ini
        ├── datebase.db
        ├── pose_bounds.npy
        ├── simplices.npy
see more [LLFF](https://github.com/fyusion/llff)
### datasets
- [2019-LLFF](https://drive.google.com/drive/folders/14boI-o5hGO9srnWaaogTU5_ji7wkX2S7)

## 1.3 unbounded scenes

### format
### datasets


