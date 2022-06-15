# TrajNet++ Model Zoo

[TrajNet++](https://github.com/vita-epfl/trajnetplusplusbaselines) is an open source framework for training trajectory forecasting models.

The TrajNet++ Model Zoo is a collection of pre-trained, state-of-the-art models for the TrajNet++ challenge. Accompanying each model is the description of model training and the command to train the model.

## Trajnetplusplusbaselines Models

This collection of models can be directly trained using the [TrajNet++](https://github.com/vita-epfl/trajnetplusplusbaselines) repository.

### Interaction Encoders

|Interaction Class |Reference |Command | Description |
|-|-|-|-|
|<b>Occupancy LSTM</b>|[Alahi et al.](https://openaccess.thecvf.com/content_cvpr_2016/html/Alahi_Social_LSTM_Human_CVPR_2016_paper.html)|`sh scripts/interaction/occupancy.sh`|Occupancy Grid|
|<b>Social LSTM</b>|[Alahi et al.](https://openaccess.thecvf.com/content_cvpr_2016/html/Alahi_Social_LSTM_Human_CVPR_2016_paper.html)|`sh scripts/interaction/social.sh`|Social Grid|
|<b>Directional LSTM</b>|[Kothari et al.](https://ieeexplore.ieee.org/document/9408398)|`sh scripts/interaction/directional.sh`|Directional Grid|


### External Models

This collection of models can be trained using modifications of other open-source model repositories to TrajNet++ format.

|Model |Reference |Command |Repository |
|-|-|-|-|
|<b>Trajectory Transformer</b>|[Giuliari et al.](https://arxiv.org/pdf/2003.08111.pdf)|`./trajnet_scripts/trajnet_run.sh`|[repository link](https://github.com/vita-epfl/Trajectory-Transformer)|
|<b>STGAT</b>|[Huang et al.](https://openaccess.thecvf.com/content_ICCV_2019/papers/Huang_STGAT_Modeling_Spatial-Temporal_Interactions_for_Human_Trajectory_Prediction_ICCV_2019_paper.pdf)|`./trajnet_scripts/trajnet_run.sh`|[repository link](https://github.com/vita-epfl/STGAT)|
|<b>Social-STGCNN</b>|[Mohamed et al.](https://openaccess.thecvf.com/content_CVPR_2020/papers/Mohamed_Social-STGCNN_A_Social_Spatio-Temporal_Graph_Convolutional_Neural_Network_for_Human_CVPR_2020_paper.pdf)|`./trajnet_scripts/trajnet_run.sh`|[repository link](https://github.com/vita-epfl/Social-STGCNN)|
|<b>CausalHTP</b>|[Chen et al.](https://openaccess.thecvf.com/content/ICCV2021/papers/Chen_Human_Trajectory_Prediction_via_Counterfactual_Analysis_ICCV_2021_paper.pdf)|`./trajnet_scripts/trajnet_run.sh`|[repository link](https://github.com/vita-epfl/CausalHTP)|
|<b>SocialWays</b>|[Amirian et al.](https://openaccess.thecvf.com/content_CVPRW_2019/papers/Precognition/Amirian_Social_Ways_Learning_Multi-Modal_Distributions_of_Pedestrian_Trajectories_With_GANs_CVPRW_2019_paper.pdf)|`./trajnet_scripts/trajnet_run.sh`|[repository link](https://github.com/vita-epfl/socialways)|
|<b>SR-LSTM</b>|[Zhang et al.](https://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_SR-LSTM_State_Refinement_for_LSTM_Towards_Pedestrian_Trajectory_Prediction_CVPR_2019_paper.pdf)|`./trajnet_scripts/trajnet_run.sh`|[repository link](https://github.com/vita-epfl/SR-LSTM)|

## Results

The folowing numbers are obtained using the officially released hyperparameters in the respective repositories. We are still in the process of tuning hyperparameters to optimize performance on TrajNet++

|Model |ADE/FDE |Top-3 ADE/FDE|Collisions |AIcrowd submission |
|-|-|-|-|-|
|<b>Trajectory Transformer</b>|1.22/2.57|0.70/1.45|13.86|[submission link](https://www.aicrowd.com/challenges/trajnet-a-trajectory-forecasting-challenge/submissions/180765)|
|<b>STGAT</b>|0.88/1.85|0.65/1.35|11.28|[submission link](https://www.aicrowd.com/challenges/trajnet-a-trajectory-forecasting-challenge/submissions/180750)|
|<b>Social-STGCNN</b>|0.80/1.52|0.61/1.18|16.78|[submission link](https://www.aicrowd.com/challenges/trajnet-a-trajectory-forecasting-challenge/submissions/180812)|
|<b>CausalHTP</b>|0.85/1.78|0.65/1.35|10.87|[submission link](https://www.aicrowd.com/challenges/trajnet-a-trajectory-forecasting-challenge/submissions/189076)|
|<b>SocialWays*</b>|2.57/4.69|2.56/4.67|0.57|[submission link](https://www.aicrowd.com/challenges/trajnet-a-trajectory-forecasting-challenge/submissions/189097)|
|<b>SR-LSTM</b>|0.80/1.58|0.80/1.58|10.84|[submission link](https://www.aicrowd.com/challenges/trajnet-a-trajectory-forecasting-challenge/submissions/189098)|

<b>*</b> - unreliable official implementation, yields unreliable evaluation results

# License

[MIT License](LICENSE)

# Citation

If you find this code useful in your research then please cite

```
@article{Kothari2020HumanTF,
  author={Kothari, Parth and Kreiss, Sven and Alahi, Alexandre},
  journal={IEEE Transactions on Intelligent Transportation Systems},
  title={Human Trajectory Forecasting in Crowds: A Deep Learning Perspective},
  year={2021},
  volume={},
  number={},
  pages={1-15},
  doi={10.1109/TITS.2021.3069362}
 }
```
