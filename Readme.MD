## Description
This repository provides on-road and off-road models for the 1/5th scale Hunter SE robot to help you get started with Project Varuna.

## File Organization

> **Note**  
> - For off-road applications, use the models in the `Hunter-SE-Offroad-Models` folder.
> - For on-road applications, use the models in the `Hunter-SE-Onroad-Models` folder.

Files in this repository follow a standardized naming convention: `platform_MMPK_num-models_control-horizon`

When using the provided models or creating new ones, this naming structure will help maintain consistency.

- **platform**: Specifies the UGV platform type (e.g., F1Tenth, Hunter-SE, Custom).
- **num-models**: Represents the number of models in the MMPK framework.
- **control-horizon**: This parameter is the one you set for MPC control horizon in the GUI. It defines the preview horizon used to calculate curvature, which in turn affects how training data is segmented for model identification.

> **Important:**  
> Ensure the `control-horizon` parameter aligns with your desired preview horizon when deploying the model. This setting influences the model's behavior and accuracy during deployment.
