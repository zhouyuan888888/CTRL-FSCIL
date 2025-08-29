# Controllable Relation Disentanglement for Few-Shot Class-Incremental Learning

### Our code and pretrained models are all provided in [Google Drive](https://drive.google.com/drive/folders/1AH2VF4bbn7a3jQFiO3LAmbSp7NVBosAo?usp=sharing), since Google Drive does not have much limitations on the size of files.  

### For testing the performance of our models, please download our code and run the following commands step-by-step.  
#### :dart: Step-I: Download ctrl_fscil.zip from Google Drive and unzip it.
`unzip ctrl_fscil.zip`
#### :dart: Step-II: Prepare environments.
`cd ctrl_fscil`
`conda env create -f environment.yml && conda activate ctrl_fscil`
#### :dart: Step-III: Prepare datasets.
`cd data`
`tar -xzvf ./cifar/cifar-100-python.tar.gz -C ./cifar`
`tar -xvf miniimagenet.tar`
#### :dart: Step-IV: Run evaluation scripts.
`cd ../`
`bash run_ctrl/cifar/ctrl_inc.sh;`
`bash run_ctrl/mini_imagenet/ctrl_inc.sh`

Note that we run the code on an RTX 3090 GPU card with CUDA==11.4. We believe that CUDA==11.7 is also compatible with our code.

:pushpin: If our work is useful for your research, please consider cite our paper:

```@article{zhou2025controllable,
  title={Controllable Relation Disentanglement for Few-Shot Class-Incremental Learning},
  author={Zhou, Yuan and Hong, Richang and Guo, Yanrong and Liu, Lin and Hao, Shijie and Zhang, Hanwang},
  journal={IEEE Transactions on Circuits and Systems for Video Technology},
  year={2025},
  publisher={IEEE}
}```
