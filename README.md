# segmentation

### install in win10
- create conda env
```python
conda create -n mmseg python=3.8
conda activate mmseg
```
- create cuda env
```python
CUDA_PATH                      C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v10.2
CUDA_PATH_V10_1                C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v10.1
CUDA_PATH_V10_2                C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v10.2
MMCV_WITH_OPS                  1
TORCH_CUDA_ARCH_LIST           7.5
```
- install torch
```python
pip install torch==1.9.1+cu111 torchvision==0.10.1+cu111 torchaudio==0.9.1 -f https://download.pytorch.org/whl/torch_stable.html
```
- install mmcv
```python
git clone https://github.com/open-mmlab/mmcv.git
cd mmcv
python setup.py build_ext
python setup.py develop
pip list
```
- install mmdetection
```python
cd ..
git clone https://github.com/open-mmlab/mmdetection.git
cd mmdetection
python setup.py develop
pip list
```
- install mmsegmentation
```python
cd ..
git clone https://github.com/open-mmlab/mmsegmentation.git
cd mmsegmentation
python setup.py develop
pip list
```
if download slow, can use gitee.com
