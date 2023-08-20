# NeRFs-Datasets
**Contains almost all NeRFs datasets, about types, formats and links.**

In recent years, NeRF has developed rapidly, and various iterative methods and technologies have also shown their prowess. 
Along with it, a large number of corresponding data sets have also appeared. 
In order to facilitate the distinction and use, this paper classifies most of the data sets related to NeRF.
If there is anything missing, welcome to contribute

# 1 Static scenes
## 1.1 single object
https://github.com/lixiaojie-thu/NeRFs-Datasets/assets/40080699/9a3f7cb5-3dc8-429f-a647-f2ec0d72bedc

[2023-OmniObject3D](https://opendatalab.com/OpenXD-OmniObject3D-New/download)
<details> <summary>format</summary>
        OmniObject3D_Data_Root
        ├── raw_scans               
        │   ├── <category_name>
        │   │   ├── <object_id>
        │   │   │   ├── Scan
        │   │   │   │   ├── Scan.obj
        │   │   │   │   ├── Scan.mtl
        │   │   │   │   ├── Scan.jpg
            
        ├── blender_renders         
        │   ├── <category_name>
        │   │   ├── <object_id>
        │   │   │   ├── render
        │   │   │   │   ├── images
        │   │   │   │   ├── depths
        │   │   │   │   ├── normals
        │   │   │   │   ├── transforms.json    
    
        ├── videos_processed       
        │   ├── <category_name>
        │   │   ├── <object_id>
        │   │   │   ├── standard
        │   │   │   │   ├── images
        │   │   │   │   ├── matting
        │   │   │   │   ├── poses_bounds.npy           # raw results from colmap
        │   │   │   │   ├── poses_bounds_rescaled.npy  # rescaled to world-scale
        │   │   │   │   ├── sparse
    
        ├── point_clouds    
        │   ├── hdf5_files
        │   │   ├── 1024
        │   │   ├── 4096
        │   │   ├── 16384
        │   ├── ply_files
        │   │   ├── 1024
        │   │   ├── 4096
        │   │   ├── 16384

</details>

[2020-NeRF](https://drive.google.com/drive/folders/1JDdLGDruGNXWnM1eqY1FNL9PlStjaKWi) 
<details> <summary>format</summary>
    
    dataset
        ├── train
        │   └── r_x.png
            ...
        ├── test
        │   ├── r_x.png
        │   ├── r_x_depth.png
            ...
        ├── val
        │   ├── r_x.png
            ...
        ├── transforms_train.json
        ├── transforms_test.json
        ├── transforms_val.json
    
</details>

[2020-NSVF](https://lingjie0206.github.io/papers/NSVF/)
<details> <summary>format</summary>
    
    dataset
        |-- bbox.txt         # bounding-box file
        |-- intrinsics.txt   # 4x4 camera intrinsics
        |-- rgb
            |-- 0.png        # target image for each view
            |-- 1.png
            ...
        |-- pose
            |-- 0.txt        # camera pose for each view (4x4 matrices)
            |-- 1.txt
            ...
        [optional]
        |-- test_traj.txt    # camera pose for free-view rendering demonstration (4N x 4)
    
</details>


[2019-DeepVoxels](https://www.vincentsitzmann.com/deepvoxels/)
<details> <summary>format</summary> intrinsics/
        
    dataset
        ├── intrinsics
        │   └── 000x.txt
             ...
        ├── rgb
        │   ├── 000x.png
             ...
        ├── pose
        │   ├── 000x.txt
             ...
        ├── intrinsics.txt
    
</details>

[2014-DTU](https://roboimagedata.compute.dtu.dk/?page_id=36)
<details> <summary>format</summary>
    
    
</details>

## 1.2 forward facing scenes
https://github.com/lixiaojie-thu/NeRFs-Datasets/assets/40080699/e8ef1ca7-4b89-4dab-8421-b9eb4ed686c1

[2019-LLFF](https://drive.google.com/drive/folders/14boI-o5hGO9srnWaaogTU5_ji7wkX2S7)
<details> <summary>format</summary>
    
    dataset
        ├── images
        │   └── img_x.jpg
            ...
        ├── images_4
        │   ├── img_x.jpg
            ...
        ├── images_8
        │   ├── img_x.jpg
            ...
        ├── spare
            ├── 0
                ├── cameras.bin
                ├── images.bin
                ├── points3D.bin
        ├── pose_bounds.npy
        ├── simplices.npy
    
</details>

## 1.3 unbounded scenes
![tat_Playground](https://github.com/lixiaojie-thu/NeRFs-Datasets/assets/40080699/bd16da32-73e6-4a0b-b9a8-327baec549d1)

[2022-mipnerf360](https://jonbarron.info/mipnerf360/)

<details> <summary>format</summary>
    
    dataset
        ├── images
        │   └── img_x.jpg
            ...
        ├── images_2
        │   ├── img_x.jpg
            ...
        ├── images_4
        │   ├── img_x.jpg
            ...
        ├── images_8
        │   ├── img_x.jpg
            ...
        ├── spare
            ├── 0
                ├── cameras.bin
                ├── images.bin
                ├── points3D.bin
        ├── pose_bounds.npy
    
</details>

[2020-nerf++](https://github.com/Kai-46/nerfplusplus)
<details> <summary>format</summary>
    
    dataset
        ├── images
        │   └── img_x.jpg
            ...
        ├── images_4
        │   ├── img_x.jpg
            ...
        ├── images_8
        │   ├── img_x.jpg
            ...
        ├── spare
            ├── 0
                ├── cameras.bin
                ├── images.bin
                ├── points3D.bin
        ├── datebase.db
        ├── pose_bounds.npy
        ├── simplices.npy
    
</details>

## 1.3 large scenes
[2019-BlendedMVS](https://github.com/YoYo000/BlendedMVS)
<details> <summary>format</summary>
    
    dataset                 
        ├── BlendedMVG_list.txt                
        ├── BlendedMVS_list.txt                 
        ├── BlendedMVS+_list.txt                
        ├── BlendedMVS++_list.txt              
        ├── ...
        ├── PID0                        
        │   ├── blended_images          
        │   │	├── 00000000.jpg        
        │   │	├── 00000000_masked.jpg        
        │   │	├── 00000001.jpg        
        │   │	├── 00000001_masked.jpg        
        │   │	└── ...                 
        │   ├── cams                      
        │   │  	├── pair.txt           
        │   │  	├── 00000000_cam.txt    
        │   │  	├── 00000001_cam.txt    
        │   │  	└── ...                 
        │   └── rendered_depth_maps     
        │      	├── 00000000.pfm        
        │     	├── 00000001.pfm        
        │     	└── ...                    
        ├── PID1                        
        ├── ...                         
        └── PID501     
    
</details>

# 2 Dynamic scenes
## 2.1 synthetic single dynamic object
https://github.com/lixiaojie-thu/NeRFs-Datasets/assets/40080699/4aa7c6ec-8d24-43e1-a62b-e7ddfad7390a


[2020-D-NeRF](https://www.albertpumarola.com/research/D-NeRF/index.html)
<details> <summary>format</summary>
    
    dataset
        ├── train
        │   └── r_x.png
            ...
        ├── test
        │   ├── r_x.png
        │   ├── r_x_depth.png
            ...
        ├── val
        │   ├── r_x.png
            ...
        ├── transforms_train.json
        ├── transforms_test.json
        ├── transforms_val.json
    
</details>

## 2.2 monocular videos 


https://github.com/lixiaojie-thu/NeRFs-Datasets/assets/40080699/24e656d3-cf23-471b-b828-c2b0cb7b0ee6



[2021-Nerfies](https://nerfies.github.io/)(forward_facing)
<details> <summary>format</summary>
    
    dataset
        ├── camera
        │   └── ${item_id}.json
            ...
        ├── camera-paths
        ├── rgb
        │   ├── ${scale}x
        │   └── └── ${item_id}.png
                ...
        ├── metadata.json
        ├── points.npy
        ├── dataset.json
        └── scene.json
    
</details>


[2021-hypernerf](https://hypernerf.github.io/)(forward_facing)
<details> <summary>format</summary>
    
    dataset
        ├── camera
        │   └── ${item_id}.json
            ...
        ├── camera-paths
        ├── rgb
        │   ├── ${scale}x
        │   └── └── ${item_id}.png
                ...
        ├── metadata.json
        ├── points.npy
        ├── dataset.json
        └── scene.json
    
</details>


[2020-NSFF](https://drive.google.com/drive/folders/1G-NFZKEA8KSWojUKecpJPVoq5XCjBLOV)((forward_facing))
<details> <summary>format</summary>
    
    
</details>


[2020-Nvidia Dynamic Scene Dataset](https://research.nvidia.com/publication/2020-06_novel-view-synthesis-dynamic-scenes-globally-coherent-depths)(forward_facing)

<details> <summary>format</summary>
    
    
</details>


## 2.3 multiple synchronized videos
## 



