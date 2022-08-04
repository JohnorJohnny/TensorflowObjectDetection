# TensorflowObjectDetection

This project is for training and leveraging your own custom object detection model using the Tensorflow Object Detection API and OpenCV.
The main goal was practice with Tensorflow Object Detection API, so my model is very raw (because it has few input images), but you can create your own and train it well by adding more images.

<img src='https://i.imgur.com/n2bDTjM.png'>

## Requirements

<b>After you create your venv install all packages from requirements.txt.<b/>
You can do this by run next command
<pre>
pip install -r TensorflowObjectDetection/requirements.txt
</pre>

## To test my model follow these steps:
<b>Step 1.</b> Clone this repository: https://github.com/JohnorJohnny/TensorflowObjectDetection.git
<br/><br/>
<b>Step 2.</b> Create a new virtual environment 
<pre>
python -m venv tfod
</pre> 
<br/>
<b>Step 3.</b> Activate your virtual environment
<pre>
source tfod/bin/activate # Linux
.\tfod\Scripts\activate # Windows 
</pre>
<br/>
<b>Step 4.</b> Install dependencies and add virtual environment to the Python Kernel (don't foget about requirments!!!)
<pre>
python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=tfodj
</pre>
<br/>
<b>Step 5.</b> Install Jupyter Notebook and run it
<pre>
pip install jupyter
jupyter notebook
</pre>
<br/>
<b>Step 5.</b>  Run <a href="https://github.com/JohnorJohnny/TensorflowObjectDetection/blob/main/Original.ipynb">Original.ipynb</a> 
If you want to test your image don't foget to add it to image_test and replace image_name in code

## To train and leverage your own model follow these steps:
<br />
<b>Step 1.</b> Clone this repository: https://github.com/JohnorJohnny/TensorflowObjectDetection.git (if you don't do this yet)
<br/><br/>
<b>Step 2.</b> Create a new virtual environment 
<pre>
python -m venv tfod
</pre> 
<br/>
<b>Step 3.</b> Activate your virtual environment
<pre>
source tfod/bin/activate # Linux
.\tfod\Scripts\activate # Windows 
</pre>
<br/>
<b>Step 4.</b> Install dependencies and add virtual environment to the Python Kernel
<pre>
python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=tfodj
</pre>
<br/>
<b>Step 5.</b> Collect images (ensure you change the kernel to the virtual environment as shown below)
<img src="https://i.imgur.com/6FKjrWG.png"> 
<br/><br/>
<b>Step 6.</b> Manually divide collected images into two folders train and test. So now all folders and annotations should be split between the following two folders. <br/>
\TFODCourse\Tensorflow\workspace\images\train<br />
\TFODCourse\Tensorflow\workspace\images\test
<br/><br/>
<b>Step 7.</b> Setup all Path, download model from Tensorflow Model Zoo and install it. Then create a label map, update config and now you can train and evaluate your own model.
<br/>
Note: During this process the Notebook will install Tensorflow Object Detection. You should ideally receive a notification indicating that the API has installed successfully at Step 8 with the last line stating OK.  
<img src="https://i.imgur.com/BZmmTYE.png">
<br /> <br/>
<b>Step 8.</b> Finally you can test your model using other images or by your camera in real time
<img src="https://i.imgur.com/hjWfFPi.png">
