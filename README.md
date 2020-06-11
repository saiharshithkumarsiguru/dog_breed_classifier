<html>
<h1>How are dogs clssified according to their breeds?</h1>


<h1>Table of Contents</h1>
<pre>
<a href="#Description">Description</a> 	
<a href="#Installation">Installation</a>
<a href="#Project Motivation">Project Motivation</a>
<a href="#File Description">File Description</a>
<a href="#Execution">Execution</a>
<a href="#Results">Results</a>
<a href="#Licensing">Licensing</a>
<a href="#Acknowledgements">Acknowledgements</a>
</pre>
<div id="Description">
<h1>Description</h1>
<pre>
In this project, we will build a pipeline that can be used within a web or mobile app to process real-world, user-supplied images. 

Given an image of a dog, this algorithm will identify an estimate of the canine’s breed.  If supplied an image of a human, the code will identify the resembling dog breed.  
</pre>
	
</div>
<div id="Installation">

<h1>Installation</h1>

 
<pre>
1. Clone the repository and navigate to the downloaded folder.
```	
git clone https://github.com/saiharshithkumarsiguru/dog_breed_classifier.git
cd dog-project
```

2. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/dogImages`. 

3. Download the [human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder. 

4. Donwload the [VGG-16 bottleneck features](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz) for the dog dataset.  Place it in the repo, at location `path/to/dog-project/bottleneck_features`.

5. (Optional) __If you plan to install TensorFlow with GPU support on your local machine__, follow [the guide](https://www.tensorflow.org/install/) to install the necessary NVIDIA software on your system.  If you are using an EC2 GPU instance, you can skip this step.

6. (Optional) **If you are running the project on your local machine (and not using AWS)**, create (and activate) a new environment.

	- __Linux__ (to install with __GPU support__, change `requirements/dog-linux.yml` to `requirements/dog-linux-gpu.yml`): 
	```
	conda env create -f requirements/dog-linux.yml
	source activate dog-project
	```  
	- __Mac__ (to install with __GPU support__, change `requirements/dog-mac.yml` to `requirements/dog-mac-gpu.yml`): 
	```
	conda env create -f requirements/dog-mac.yml
	source activate dog-project
	```  
	**NOTE:** Some Mac users may need to install a different version of OpenCV
	```
	conda install --channel https://conda.anaconda.org/menpo opencv3
	```
	- __Windows__ (to install with __GPU support__, change `requirements/dog-windows.yml` to `requirements/dog-windows-gpu.yml`):  
	```
	conda env create -f requirements/dog-windows.yml
	activate dog-project
	```

7. (Optional) **If you are running the project on your local machine (and not using AWS)** and Step 6 throws errors, try this __alternative__ step to create your environment.

	- __Linux__ or __Mac__ (to install with __GPU support__, change `requirements/requirements.txt` to `requirements/requirements-gpu.txt`): 
	```
	conda create --name dog-project python=3.5
	source activate dog-project
	pip install -r requirements/requirements.txt
	```
	**NOTE:** Some Mac users may need to install a different version of OpenCV
	```
	conda install --channel https://conda.anaconda.org/menpo opencv3
	```
	- __Windows__ (to install with __GPU support__, change `requirements/requirements.txt` to `requirements/requirements-gpu.txt`):  
	```
	conda create --name dog-project python=3.5
	activate dog-project
	pip install -r requirements/requirements.txt
	```
	
8. (Optional) **If you are using AWS**, install Tensorflow.
```
sudo python3 -m pip install -r requirements/requirements-gpu.txt
```
	
9. Switch [Keras backend](https://keras.io/backend/) to TensorFlow.
	- __Linux__ or __Mac__: 
		```
		KERAS_BACKEND=tensorflow python -c "from keras import backend"
		```
	- __Windows__: 
		```
		set KERAS_BACKEND=tensorflow
		python -c "from keras import backend"
		```

10. (Optional) **If you are running the project on your local machine (and not using AWS)**, create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `dog-project` environment. 
```
python -m ipykernel install --user --name dog-project --display-name "dog-project"
```

11. Open the notebook.
```
jupyter notebook dog_app.ipynb
```

12. (Optional) **If you are running the project on your local machine (and not using AWS)**, before running code, change the kernel to match the dog-project environment by using the drop-down menu (**Kernel > Change kernel > dog-project**). Then, follow the instructions in the notebook.


</pre>
</div>

<div id="Project Motivation">

<h1>Project Motivation</h1>
<pre>

It's really interesting to classify dogs based on their breeds and funny to compare which dog face it matches.
This seems funny  but has got many real world applications.     

</pre>
</div>




<div id="File Description">
<h1>File Description</h1>

<pre>

dog_app.ipynb :This is our main jupyter notebbok file after installing the requirements run this file.

images:It contains images 

test_images:It contains test images.

haarcascades: It contains files related to detection.(please download the haarcascades front faces xml and place in this folder after you create this folder before running main file )

saved_models: It contains our saved models.(please add this folder befor you run the main file). 

dog_app.html: This is html version of our jupyter  notebook.

bottleneck_features : It contains ours VG16 model.(please create this folder download the model file here before running the main file)

requirements: file about requirements.

NOTE: The download links are present in the <a href"#Installation">Installation</a> section.    

</pre>
</div>

<div id="Execution">
<pre>
1. Run the jupyter notebbok file that is dog_app.ipynb everything will work fine if you  have met all the requirements.
</pre>
</div>
<div id="Results">
<h1>Results</h1>
 Our model is about to predict the images with more than 80% accuracy for both test and train accuracy.

 we can further improve our model accuracy 

 *by using image augmentation 

 *by using further deep neural networks 

 *by providing more data like more dog breeds etc.   

</div>
<div id="Licensing">
<h1>Licensing</h1>
<pre>
MIT license
</pre>
</div>
<div id="Acknowledgements">
<pre>
<h1>Acknowledgements</h1>
* Thanks UDACITY for providing such a complete Data Science Nanodegree Program
</pre>
</div>



 </html>