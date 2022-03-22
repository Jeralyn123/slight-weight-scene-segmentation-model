# slight-weight-scene-segmentation-model

## Installation
```
# dependencies
pip install ninja tqdm

# follow PyTorch installation in https://pytorch.org/get-started/locally/
conda install pytorch torchvision -c pytorch

# install PyTorch Segmentation
git clone https://github.com/Jeralyn123/slight-weight-scene-segmentation.git

# the following will install the lib with symbolic links, so that you can modify
### Train
-----------------
- **training**
```
python train.py --model swnet --backbone resnet50 --dataset cityscape --lr 0.0001 --epochs 50
```

### Evaluation
```
# for example, evaluate swnet_cityscape
python eval.py --model swnet --backbone resnet50 --dataset cityscape
```
```
### Demo
```
python demo.py 
```
note: you also can train a reconstructed model by yourself. Then, you should add this net into "train". 
### evaluation metric

![image](https://user-images.githubusercontent.com/43395674/159432544-e37ea05a-61e9-4f9d-b0ec-e381845ad900.png)
![image](https://user-images.githubusercontent.com/43395674/159432566-4e79d269-f4ad-4b99-b0e6-ecd7d21a8255.png)

### results

![image](https://user-images.githubusercontent.com/43395674/159432651-2365cf4c-a06d-46d1-83df-994ddd0769fb.png)
![image](https://user-images.githubusercontent.com/43395674/159432664-732faf8e-1f7a-49f1-9c54-607a9270aa1e.png)
### experiment 
a simulative experiment on real scene based on jetson series.
![image](https://user-images.githubusercontent.com/43395674/159433770-ea19dea9-d0ab-45f0-b006-a5c6a028447a.png)

