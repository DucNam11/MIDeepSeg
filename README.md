## MIDeepSeg: Minimally Interactive Segmentation of Unseen Objects from Medical Images Using Deep Learning 
This repository proivdes a 2D medical image interactive segmentation method for segmentation and annotation.
![image](https://github.com/DucNam11/MIDeepSeg/blob/master/demo_video/pancreas.gif)


## Requirements
Before you can use this package for image segmentation. You should:
* PyTorch version >=1.0.1
* Some common python packages such as Numpy, Pandas, SimpleITK,OpenCV, pyqt5, scipy......
* Install the [GeodisTK][geos_dis_link] for geodesic distance transformation.
* Install the [SimpleCRF][simplecrf_link] for interactive refinement.
## How to use
1, compile the requirement library:

```bash
pip install -r requirements.txt
```
2. launch the GUI
```bash
cd mideepseg
python main.py
``` 
3. load an image for segmentation. Once the image is loaded,  Firstly, give some edge points by left mouse to get an initial interactions, click the Segmentation button to obtain an initial segmentation. Then, press left mouse button to give clicks in under-segmented regions, and press right mouse button to give clicks  in over-segmented region. Then click the Refinement button, and the segmentation will be updated according to the interactions.

4. Note that, the pretrained model is only trained with placenta MR-T2 data. 

