# slight-weight-scene-segmentation-model

## Installation
```
# dependencies
pip install ninja tqdm

# follow PyTorch installation in https://pytorch.org/get-started/locally/
conda install pytorch torchvision -c pytorch

# install PyTorch Segmentation
git clone https://github.com/Tramac/awesome-semantic-segmentation-pytorch.git

# the following will install the lib with symbolic links, so that you can modify
### Train
-----------------
- **training**
```
python train.py --model swnet --backbone resnet50 --dataset cityscape --lr 0.0001 --epochs 50
```

### Evaluation
-----------------
```
# for example, evaluate propsoed-net_cityscape
python eval.py --model swnet --backbone resnet50 --dataset cityscape
```
```
### Demo
```
cd ./scripts
python demo.py 
```
note: you also can train a reconstructed model by yourself. Then, you should add this net into "train". 
