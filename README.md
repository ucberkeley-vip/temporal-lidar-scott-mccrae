Temporal LiDAR object detection network, VIP Lab UC Berkeley

The bulk of this project is forked from this repo by github user traveller59: https://github.com/traveller59/second.pytorch. 
You can follow the installation instructions on that page to get set up and install requirements. 

The LSTM is modified from this project: https://github.com/ndrplz/ConvLSTM_pytorch/blob/master/convlstm.py

We used the nuScenes dataset, available at www.nuScenes.org. (Or, you could try other datasets, like Waymo or Lyft Level 5, although we have not tested this with those datasets.)

You can find our paper, published in ICIP 2020, [here](http://www-video.eecs.berkeley.edu/papers/mccrae/ICIP_Extended_Results_9_23_Revision.pdf).
The all.pp.mida.config setup was used to generate results for our paper, and should be the starting point for reproducing them.

You can train a model with commands like this:
`python ./pytorch/train.py train --config_path=./configs/<your_config> --model_dir=<path_to_your_model_directory>`
