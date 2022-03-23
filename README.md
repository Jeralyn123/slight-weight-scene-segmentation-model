# slight-weight-scene-segmentation-model
If you want to run the program, you should firstly install dependencies, and also download scene datasets such as cityscape.
## Installation
```
# dependencies
pip install ninja tqdm

# follow PyTorch installation in https://pytorch.org/get-started/locally/
conda install pytorch torchvision -c pytorch

# install PyTorch Segmentation
git clone https://github.com/Jeralyn123/slight-weight-scene-segmentation.git

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

## References
- [PyTorch-Encoding](https://github.com/zhanghang1989/PyTorch-Encoding)
- [maskrcnn-benchmark](https://github.com/facebookresearch/maskrcnn-benchmark)
- [gloun-cv](https://github.com/dmlc/gluon-cv)
- [imagenet](https://github.com/pytorch/examples/tree/master/imagenet)
- [code support](https://github.com/Tramac/awesome-semantic-segmentation-pytorch.git)

<!--
[![python-image]][python-url]
[![pytorch-image]][pytorch-url]
[![lic-image]][lic-url]
--> 

