# TrajNet++ Model Zoo

[TrajNet++](https://github.com/vita-epfl/trajnetplusplusbaselines) is an open source framework for training trajectory forecasting models.

The TrajNet++ Model Zoo is a collection of pre-trained, state-of-the-art models for the TrajNet++ challenge. Accompanying each model is the description of model training and the command to train the model.

## Trajnetplusplusbaselines Models

This collection of models can be directly trained using the [TrajNet++](https://github.com/vita-epfl/trajnetplusplusbaselines) repository.

### Interaction Encoders

|Interaction Class |Reference |Command | Description |
|-|-|-|-|
|<b>Occupancy LSTM</b>|[Alahi et al.](https://openaccess.thecvf.com/content_cvpr_2016/html/Alahi_Social_LSTM_Human_CVPR_2016_paper.html)|`python -m trajnetbaselines.lstm.trainer --type occupancy --augment`|Occupancy Grid|
|<b>Social LSTM</b>|[Alahi et al.](https://openaccess.thecvf.com/content_cvpr_2016/html/Alahi_Social_LSTM_Human_CVPR_2016_paper.html)|`python -m trajnetbaselines.lstm.trainer --type social --augment`|Social Grid|
|<b>Directional LSTM</b>|[Kothari et al.](https://ieeexplore.ieee.org/document/9408398)|`python -m trajnetbaselines.lstm.trainer --type directional --augment`|Directional Grid|


### External Models

This collection of models can be trained using modifications of other open-source model repositories to TrajNet++ format.

|Model |Reference |Command |Repository |
|-|-|-|-|
|<b>Trajectory Transformer</b>|[Giuliari et al.](https://arxiv.org/pdf/2003.08111.pdf)|`./trajnet_scripts/trajnet_run.sh`|[repository link](https://github.com/vita-epfl/Trajectory-Transformer)|
|<b>STGAT</b>|[Huang et al.](https://openaccess.thecvf.com/content_ICCV_2019/papers/Huang_STGAT_Modeling_Spatial-Temporal_Interactions_for_Human_Trajectory_Prediction_ICCV_2019_paper.pdf)|`./trajnet_scripts/trajnet_run.sh`|[repository link](https://github.com/vita-epfl/STGAT)|
|<b>Social-STGCNN</b>|[Mohamed et al.](https://openaccess.thecvf.com/content_CVPR_2020/papers/Mohamed_Social-STGCNN_A_Social_Spatio-Temporal_Graph_Convolutional_Neural_Network_for_Human_CVPR_2020_paper.pdf)|`./trajnet_scripts/trajnet_run.sh`|[repository link](https://github.com/vita-epfl/Social-STGCNN)|


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
