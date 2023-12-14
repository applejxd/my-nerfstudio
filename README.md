# nerfstudio in my environement

From [nerfstudio](https://github.com/nerfstudio-project/nerfstudio)

## How to use

1. Launch: `docker compose up -d`
2. SfM: `ns-process-data video --data /datasets/iPhone/IMG_1006.MOV --output-dir ./sfm`
3. Training: `ns-train nerfacto --pipeline.model.predict-normals True --data ./sfm`
4. Export mesh: `ns-export poisson --load-config ./outputs/sfm/nerfacto/date/config.yml --output-dir ./mesh`
