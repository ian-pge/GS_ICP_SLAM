<div align=center>

# RGBD GS-ICP SLAM (100FPS Gaussian Splatting SLAM)

[Seongbo Ha](https://riboha.github.io), [Jiung Yeon](https://humdrum-balance-b8f.notion.site/Jiung-Yeon-6754922a22814c9a95af88801a96fb4b), Hyeonwoo Yu

<h3 align="center"> ECCV 2024 </h3>

[Paper](https://arxiv.org/abs/2403.12550) | [Video](https://www.youtube.com/watch?v=e-bHh_uMMxE&t)

![github (1)](https://github.com/Lab-of-AI-and-Robotics/GS_ICP_SLAM/assets/34827206/5722e8f4-165d-4093-8064-a7ed5d9ea008)

</div>

This repository is intended to substantiate the results reported in the paper. Additional features including visualization tools will be updated soon!

## Environments
Install [pixi](https://pixi.sh/latest/#installation) (if you haven't already):
```bash
curl -fsSL https://pixi.sh/install.sh | bash
```

Then install the environments and submodules with:
```bash
pixi install
```

## Dataset
Download and configure the **Replica** dataset:
```bash
pixi run download-replica
```

## Run
Run the SLAM system on the Replica dataset:
- **Limited to 30 FPS:**
    ```bash
    pixi run replica
    ```
- **Unlimited tracking speed:**
    ```bash
    pixi run replica-unlimit
    ```

## Real-time demo
You can visualize the map reconstruction and trackable Gaussians using the `rerun.io` viewer. Start the viewer by running:

```bash
pixi run viewer
```

![Rerun Viewer Demo](https://github.com/Lab-of-AI-and-Robotics/GS_ICP_SLAM/assets/34827206/b4715071-2e4a-4d17-b7a2-612bbd32dbd0)
