# Face_ID
* AIM
  To create a simple and reliable Face Recognition program (For this VIDEO) by using Tensorflow in the Python Programming Language.
  
  
* Setup
  You will need to install Tensorflow and Python on your Machine.
  To install tensorflow, hit the following in the terminal:
  
      pip install tensorflow
      
  That's enough for (this)[] video.
  Also, you need to clone this Repository, to do so, hit the following:
     
      git clone https://github.com/MauryaRitesh/Face_ID
      
* Gathering Images
  You will need a lot of images of your(or the one for whom you are creating the Face ID) Faces, i.e., go ahead and take hundreds of
  thousands of selfies and fill all those in the Images folder of this repository. You will need to create a Folder and rename as your
  name. E.g., Create a folder named Ritesh and another as Not Ritesh.

* ReTraining
  To train the model, hit the following:
  
      python -m scripts.retrain \
      --output_graph=tf_files/retrained_graph.pb \
      --output_labels=tf_files/retrained_labels.txt \
      --architecture=mobilenet_v1_224 \
      --image_dir=tf_files/images
