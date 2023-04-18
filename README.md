# Tensorflow-simple-object-detection
A simple image-based object detection tensorflow app in Python
Originally forked from [here](https://github.com/diegocavalca/machine-learning).

## Instructions:

This is a Python application for object detection using Tensorflow. It is designed to detect objects in images and videos, making it a useful tool for various applications such as security, surveillance, and object tracking. The application is easy to use and can be set up quickly by following the instructions provided in the documentation.

To get started, you will need to have Python 3.6.2 or higher and Tensorflow installed on your system. If you do not have Python installed, it is recommended that you download the Anaconda distribution and use the corresponding installer from Anaconda's website. Once you have Python installed, you can install Tensorflow by following the installation guide on the Tensorflow website. For this application, it is recommended to install Ubuntu TensorFlow with CPU support via `pip install`.

The "object_detection" module from Tensorflow is not installed by default and needs to be downloaded from the Tensorflow Github repo and placed in the Tensorflow home directory. To download the module, you can clone or download the Tensorflow models repository from Github and extract the object_detection folder. Then, place the folder in PATH_TO_YOUR_TF>/models. If you're unsure about the location of your Tensorflow installation, you can use the command `pip show tensorflow` to find the installation path.

To make the `object_detection` libraries available, you need to add the path to the `models` and `models/slim` directories to your Python path. You can do this by adding the following lines of code to your Python script:
```
import sys
sys.path.append('<PATH_TO_TENSORFLOW>/models')
sys.path.append('<PATH_TO_TENSORFLOW>/models/slim')
from object_detection.utils import label_map_util
from object_detection.utils import visualization_utils as vis_util
```
If you installed Python through Anaconda, the `<PATH_TO_TENSORFLOW>` will look like `/home/YOUR_USER>/anaconda3/lib/python3.6/site-packages/tensorflow`.

In addition to Tensorflow, the application uses the "moviepy" and "ffmpeg" libraries for image processing. To install these libraries, you can use the following commands:
```
pip install moviepy
sudo apt-get install ffmpeg

```
Once you have installed the necessary dependencies and set up the Python environment, you can run the application by navigating to the directory containing the script and running the command 
```python tf_simple_object_detection.py``` 
The application will detect objects in the images or videos specified in the script and output the results to a new file.

Overall, this Python application for object detection using Tensorflow is a powerful tool that can be used for various applications. With its easy-to-use interface and simple setup process, it is a great choice for anyone looking to get started with object detection.



