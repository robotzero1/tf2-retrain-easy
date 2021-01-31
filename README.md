# TensorFlow Fast and Easy Image Classification
TensorFlow retraining with an image dataset of R2D2, C3PO and Darth Vader. 

This tutorial demonstrations probably the easiest way to create a model for object recognition. Images for the datasets are collected from Google Image Search and uploaded to a script on Google Colab which creates Tensorflow models in SavedModel, TensorFlow.js graph model, TensorFlow Lite format and C array style for microcontrollers.

## Collecting Images
 - In the Chrome browser install this extension: https://chrome.google.com/webstore/detail/fatkun-batch-download-ima/nnjjahlikiabnchcpehcpkdeckfgnohf/

 - In Chrome, use the image search to find images for the dataset: 
 
![google images](https://user-images.githubusercontent.com/60509953/106366365-ab1da880-633b-11eb-80b3-c1e6bfb7ec23.jpg)  

---

 - Select Fatkun Batch Download from the extensions menu in Chrome.  
 - Choose the 'Download [Current Tab] option:  
 
![fatkun download tab](https://user-images.githubusercontent.com/60509953/106366363-aa851200-633b-11eb-891e-d040443c47ff.jpg)  

---

  - Select Rename from the toolbar:  
  
![rename option](https://user-images.githubusercontent.com/60509953/106366369-ac4ed580-633b-11eb-8faf-a8f4facda8f3.jpg) 

 - Click the Download button and wait for the images from the search to be downloaded.  

---

 - Find the downloaded folder in Downloads:  
 
![images downloaded](https://user-images.githubusercontent.com/60509953/106366367-abb63f00-633b-11eb-9873-46cdb83b7160.jpg)  

---

 - Remove any images that aren't required:  
 
![images clean up](https://user-images.githubusercontent.com/60509953/106366366-ab1da880-633b-11eb-91e4-e073e351f503.jpg)  


---

## Creating the Notebook at Colab
 - Open a new notebook at Colab - https://colab.research.google.com/  
 - Choose the Github tab and paste the URL from this repo: https://github.com/robotzero1/tf2-retrain-starwars/blob/main/retrain.ipynb  

 - Open the folders menu on the left and right click to create new folders in the sample_data folder:  

![new folder](https://user-images.githubusercontent.com/60509953/106366368-abb63f00-633b-11eb-885f-e0266ccc226d.jpg) 

 - Create the following structure:  
 
![folder structure](https://user-images.githubusercontent.com/60509953/106366364-aa851200-633b-11eb-8b24-978ddcf7ce86.jpg)  

 - Drag the images from your folders to the folders on Colab:  

![select all and drag to upload](https://user-images.githubusercontent.com/60509953/106366360-a953e500-633b-11eb-8c12-c3021616fbeb.jpg)   

 - When all the images have been uploaded, select 'Runtime' > 'Run all' from the menu

![run all](https://user-images.githubusercontent.com/60509953/106366370-ac4ed580-633b-11eb-8df9-e89eeaeac820.jpg)  

 - The script will run and generate the model in SavedModel, C array style, TensorFlow.js graph model and TensorFlow Lite format. The new files will be in the /tmp folder which can be found my moving up one directory (click the folder with the white arrow) from the /content directory  

![tmp folder](https://user-images.githubusercontent.com/60509953/106389100-f4c0ce80-63e1-11eb-81cb-fb08f0316c55.jpg)  

 - If the True label and Predicted label are giving poor results, try adding more images or removing any that might confuse the classifier algorithm. Also just running the script again with the 'Run all' command can improve things as the training has a random element each time. For example the difficult image below was Predicted as C3PO on one classification run through.  

![test output](https://user-images.githubusercontent.com/60509953/106389102-f5f1fb80-63e1-11eb-9914-78efd57cce50.jpg)

 - I've uploaded a video showing the process running on Colab to YouTube here - https://youtu.be/hrv6yGmS9RE


