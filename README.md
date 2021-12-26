# Background_remover
This project aim at removing the background images using the [Computer vision](https://github.com/topics/computer-vision).


## Installation
### Python version:
- Python==3.8
### Set up [Anaconda](https://docs.anaconda.com/anaconda/install/index.html) virtual environment:
- ```conda create -n my_env python=3.8 anaconda```
### Dependencies:
- `pip install --upgrade pip`<br>
- `pip install --upgrade setuptools`<br>
### Install library:
- [numpy==1.19.5](https://numpy.org/devdocs/release/1.19.5-notes.html)<br>
- [opencv-python==4.5.1.48](https://pypi.org/project/opencv-python/)<br>
- [torch==1.7.1](https://pytorch.org/get-started/previous-versions/)<br>
- [torchvision==0.2.2](https://pypi.org/project/torchvision/0.2.2/)<br>


### MODNet - Pre-Trained Models
#### This folder is the model of MODNet:
- You can download them from this [link](https://drive.google.com/file/d/1BgQro5TxRQ99BwjktKEzR-pXeqGRIkqm/view?usp=sharing)
- Extract It and copy the following files in **Background_remover/model** folder:
    -modnet_photographic_portrait_matting.ckpt


## Usage
### Single image:
To use just one image, you must insert your image in the current directory (**/data/sample_image**)
and then run the following command:
- `python BK_remover.py --image image_path`
- Example:
    - `python BK_remover.py --image data/sample_image/my_photo.png`
    - It will generate the output file in **output/** folder
 
 ### Batch images:
 To use more than one images in the same time, you must create a directory or use the current directory (**/data/sample_image**)
 in which you will put all the images and then run the following command:
 - `python BK_remover.py --folder folder_path`
 - Example:
    - `python BK_remover.py --folder data/sample_image/`
    - It will generate the output file in **output/** folder
 
 
 ## Demo
 <table>
<tr align="center">
<td><b>Before removing the background</b></td>
<td><b>After removing the background</b></td>
</tr>
<tr align="center">
<td><img src="data/sample_image/my_photo.jpg" alt="my_photo.jpg" width="460" height="500"/></td>
<td><img src="output/my_photo.png" alt="my_photo.png" width="460" height="500"/></td>
</tr>
<table>

  
## References
- [A Trimap-Free Solution for Portrait Matting in Real Time under Changing Scenes](https://github.com/ZHKKKe/MODNet)
- Sample Male photo by <span> <a href="https://unsplash.com/@erik_lucatero?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Erik Lucatero</a> on <a href="https://unsplash.com/?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Unsplash</a></span>
- [MODNet-BKground](https://github.com/Mazhar004/MODNet-BGRemover)
  
### Contact
email: taieb.jlassi93@gmail.com<br>
LinkedIn: https://www.linkedin.com/in/taiebjlassi/

