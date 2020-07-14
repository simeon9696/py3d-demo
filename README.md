# py3d-demo


To get up and running with PyTorch 3D

- Install Detectron2
```
python -m pip install 'git+https://github.com/facebookresearch/detectron2.git'
```

- Install PyTorch3D
```
pip install 'git+https://github.com/facebookresearch/pytorch3d.git'
```

- Install optimizing static compiler
```
pip install -U cython 
```
- Install dependency 

```
pip install "git+https://github.com/philferriere/cocoapi.git#egg=pycocotools&subdirectory=PythonAPI"
```

- Clone MeshR-CNN Repo
```
git clone https://github.com/facebookresearch/meshrcnn.git 
```
- Change directory to downloaded repo 
```
cd meshrcnn
```

- Install packages needed by meshrcnn
``` 
pip install -e .
```
- Place image with object in meshrcnn/demo directory

- Extract mesh
```
python demo/demo.py --config-file configs/pix3d/meshrcnn_R50_FPN.yaml --input demo/table.jpg --output output_demo --onlyhighest MODEL.WEIGHTS meshrcnn://meshrcnn_R50.pth
```
