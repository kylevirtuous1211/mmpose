### `mmpose` Submodule: Pose Estimation

Our project uses the **`mmpose`** toolbox for real-time 2D pose estimation (e.g., RTMPose).

**Note:** We use `mmpose` **only for inference**. Our project does not contain any custom modifications to the `mmpose` submodule itself.

#### Setting Up Checkpoints

To run the pose estimation demos, you must download the pre-trained model weights (checkpoints) from the official `mmpose` repository.

1.  **Find a Model:** Visit the [MMPose Model Zoo](https://mmpose.readthedocs.io/en/latest/model_zoo.html) to find the checkpoint you need.
    * *Example:* `rtmpose-l_simcc-aic-coco_pt-aic-coco_420e-2S26x192-f016ffe0_20230126.pth`

2.  **Create Directory:** Create a `checkpoints/` folder inside the `mmpose/` submodule directory.

3.  **Place Checkpoint:** Download the `.pth` file and place it inside the new folder.

The final file structure should look like this:

```
FIAS-.../
├── mmpose/
│   ├── checkpoints/
│   │   └── rtmpose-l_simcc-aic-coco_pt-aic-coco_420e-256x192-f016ffe0_20230126.pth
│   ├── mmpose/
│   ├── tools/
│   └── ... (other mmpose files)
│
├── mmaction2/
└── ... (your project's main files)
```