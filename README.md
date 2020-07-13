# py3d-demo

```
python -m pip install 'git+https://github.com/facebookresearch/detectron2.git'
pip install 'git+https://github.com/facebookresearch/pytorch3d.git'
pip install -U cython 
pip install "git+https://github.com/philferriere/cocoapi.git#egg=pycocotools&subdirectory=PythonAPI" 
git clone https://github.com/facebookresearch/meshrcnn.git 
cd meshrcnn 
pip install -e .
python demo/demo.py --config-file configs/pix3d/meshrcnn_R50_FPN.yaml --input /demo/table.jpg --output output_demo --onlyhighest MODEL.WEIGHTS meshrcnn://meshrcnn_R50.pth

```
