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
git clone https://github.com/shinya7y/WaymoCOCO.git
cd WaymoCOCO

``` bash
# convert val
python convert_waymo_to_coco.py \               
    --tfrecord_dir ${HOME}/data/waymotfrecord/validation/ \
    --work_dir ${HOME}/data/waymococo_full/ \
    --image_dirname val2020 \
    --image_filename_prefix val \
    --label_filename instances_val2020.json \
    --add_waymo_info
```

``` bash
# with frames_with_keypoints.tfrecord in waymo_open_dataset/tutorial
python convert_waymo_to_coco.py \			
    --tfrecord_dir ./data/ \
    --work_dir ./data/waymococo_full/ \
    --image_dirname train2020 \
    --image_filename_prefix train \
    --label_filename instances_train2020.json \
    --add_waymo_info
```
