# DefectTest

'''
결함 수정이지롱
'''

``` bash
pip3 install --upgrade pip
python3 -m pip install "waymo_open_dataset_tf_2_6_0==1.4.3"
python3 -m pip install "notebook>=5.3" "ipywidgets>=7.5"
python3 -m pip install --upgrade jupyter_http_over_ws>=0.0.7 && \
jupyter serverextension enable --py jupyter_http_over_ws
jupyter notebook
```

``` bash
conda create -n waymococo python=3.7
conda activate waymococo
pip install tensorflow==2.1.0
git clone https://github.com/shinya7y/WaymoCOCO.git
cd WaymoCOCO
```
