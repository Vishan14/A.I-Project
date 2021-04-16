# FACE MASK DETECTION USING DEEP LEARNING 

## A. PROJECT SUMMARY

**Project Title:** Face Mask Detection using Deep Learning

**Team Members:** 
- Vishan Menan A/L Balakrishnan **(B031910018)**
- Cecilia Chong Ching Nee **(B031910390)**
- Siew Chung Seng **(B031910342)**
- Muhammad Putra Alif bin Ismail **(B031910115)**


- [ ] **Objectives:**
- Reduce man-power in converting old literature into digitized form manually.
- Work and serve as guide in character recognition areas.
- Use Neural signs in literature domain.


##  B. ABSTRACT 

Handwriting recognition is the ability of a machine to receive and interpret handwrit- ten input from multiple sources like paper documents, photographs, touch screen devices etc. Recognition of handwritten and machine characters is an emerging area of research and finds extensive applications in banks, offices and industries.The main aim of this project is to design expert system for , “HCR using Neural Network”that can effectivelly recognize a particular character of type format using the Artificial Neural Network approach.  Neural computing Is comparatively new field, and design components are therefore less well specified than those of other architectures. Neural computers implement data par- allelism. Neural computer are operated in way which is completely different from the oper- ation of normal computers. Neural computer are trained (not Programmed) so that given a certain starting state (data input); they either classify the input data into one of the number of classes or cause the original data to evolve in such a way that a certain desirable property is optimized. 

![Coding](https://github.com/Vishan14/A.I-Project/blob/main/Project/handwriting.png)

Figure 1 shows a handwritten cheque and AI outputs of handwritting recognition from the cheque.


## C.  DATASET

For the purpose of this project, we are using datasets from existing online resources.  

We’ll review the dataset we’ll be using to train our custom handwritten text recognizer.

I’ll then show you how to implement a Python script to train a handwritten text recognizer on our dataset using Keras and TensorFlow.

We’ll use this Python script to train a handwritten text recognizer and review the results.

![Figure 2](https://github.com/Vishan14/A.I-Project/blob/main/Project/Dataset-figure-01.jfif)

Figure 2: Handwritten text recognizer on our dataset using Keras and TensorFlow 


In order to train a custom handwritten text recognizer, we need to break our project into two distinct phases, each with its own respective sub-steps :

- Training: We’ll focus on loading our handwritten text recognition dataset from disk, training a model (using Keras/TensorFlow) on this dataset, and then serializing it to disk.

- Deployment: Once the handwritten text rocognizer is trained, we can then move on to perform handwritten text recognition.





Our COVID-19 face mask detection dataset as shown in Figure 3:

![Figure 3](https://www.pyimagesearch.com/wp-content/uploads/2020/04/face_mask_detection_dataset.jpg)

Figure 3: A face mask detection dataset consists of “with mask” and “without mask” images. 

The dataset we’ll be using here today was created by PyImageSearch reader Prajna Bhandary.

This dataset consists of 1,376 images belonging to two classes:

- with_mask: 690 images
- without_mask: 686 images

Our goal is to train a custom deep learning model to detect whether a person is or is not wearing a mask.

How was our face mask dataset created?
Prajna, like me, has been feeling down and depressed about the state of the world — thousands of people are dying each day, and for many of us, there is very little (if anything) we can do.

To help keep her spirits up, Prajna decided to distract herself by applying computer vision and deep learning to solve a real-world problem:

- Best case scenario — she could use her project to help others
- Worst case scenario — it gave her a much needed mental escape


## D.   ANALYSIS MODEL

**BEHAVIORAL MODEL**

-Use Case Diagram

The use case view models functionality of the system as perceived by outside uses. A use case is a coherent unit of functionality expressed as a transaction among actors and the system.

![Figure 4](https://github.com/Vishan14/A.I-Project/blob/main/Project/Figure%204.1.JPG)

-Sequence Diagram

![Figure 5](https://github.com/Vishan14/A.I-Project/blob/main/Project/Figure%204.2.JPG)

**FUNCTIONAL MODEL**

-Data Flow Diagram

![Figure 6](https://github.com/Vishan14/A.I-Project/blob/main/Project/Figure%204.3.1.JPG)

![Figure 7](https://github.com/Vishan14/A.I-Project/blob/main/Project/Figure%204.3.2.JPG)

-Control Flow Diagram

![Figure 8](https://github.com/Vishan14/A.I-Project/blob/main/Project/Figure%204.4.JPG)



## E   TRAINING THE COVID-19 FACE MASK DETECTION

We are now ready to train our face mask detector using Keras, TensorFlow, and Deep Learning.

From there, open up a terminal, and execute the following command:

- $ python train_mask_detector.py --dataset dataset
- [INFO] loading images...
- [INFO] compiling model...
- [INFO] training head...
- Train for 34 steps, validate on 276 samples
- Epoch 1/20
- 34/34 [==============================] - 30s 885ms/step - loss: 0.6431 - accuracy: 0.6676 - val_loss: 0.3696 - val_accuracy: 0.8242
- Epoch 2/20
- 34/34 [==============================] - 29s 853ms/step - loss: 0.3507 - accuracy: 0.8567 - val_loss: 0.1964 - val_accuracy: 0.9375
- Epoch 3/20
- 34/34 [==============================] - 27s 800ms/step - loss: 0.2792 - accuracy: 0.8820 - val_loss: 0.1383 - val_accuracy: 0.9531
- Epoch 4/20
- 34/34 [==============================] - 28s 814ms/step - loss: 0.2196 - accuracy: 0.9148 - val_loss: 0.1306 - val_accuracy: 0.9492
- Epoch 5/20
- 34/34 [==============================] - 27s 792ms/step - loss: 0.2006 - accuracy: 0.9213 - val_loss: 0.0863 - val_accuracy: 0.9688
- ...
- Epoch 16/20
- 34/34 [==============================] - 27s 801ms/step - loss: 0.0767 - accuracy: 0.9766 - val_loss: 0.0291 - val_accuracy: 0.9922
- Epoch 17/20
- 34/34 [==============================] - 27s 795ms/step - loss: 0.1042 - accuracy: 0.9616 - val_loss: 0.0243 - val_accuracy: 1.0000
- Epoch 18/20
- 34/34 [==============================] - 27s 796ms/step - loss: 0.0804 - accuracy: 0.9672 - val_loss: 0.0244 - val_accuracy: 0.9961
- Epoch 19/20
- 34/34 [==============================] - 27s 793ms/step - loss: 0.0836 - accuracy: 0.9710 - val_loss: 0.0440 - val_accuracy: 0.9883
- Epoch 20/20
- 34/34 [==============================] - 28s 838ms/step - loss: 0.0717 - accuracy: 0.9710 - val_loss: 0.0270 - val_accuracy: 0.9922
- [INFO] evaluating network...

|      |    precision    | recall| f1-score | support |
|------|-----------------|-------|----------|---------|
|with_mask|0.99|1.00|0.99|138|
|without_mask|1.00|0.99|0.99|138|
|accuracy| | |0.99|276|
|macro avg|0.99|0.99|0.99|276|
|weighted avg|0.99|0.99|0.99|276|


![Figure 4](https://www.pyimagesearch.com/wp-content/uploads/2020/04/face_mask_detector_plot.png)

Figure 4: Figure 10: COVID-19 face mask detector training accuracy/loss curves demonstrate high accuracy and little signs of overfitting on the data

As you can see, we are obtaining ~99% accuracy on our test set.

Looking at Figure 4, we can see there are little signs of overfitting, with the validation loss lower than the training loss. 

Given these results, we are hopeful that our model will generalize well to images outside our training and testing set.


## F.  RESULT AND CONCLUSION

Detecting COVID-19 face masks with OpenCV in real-time

You can then launch the mask detector in real-time video streams using the following command:
- $ python detect_mask_video.py
- [INFO] loading face detector model...
- INFO] loading face mask detector model...
- [INFO] starting video stream...

[![Figure9](https://img.youtube.com/vi/PO4hePKWIGQ/0.jpg)](https://www.youtube.com/watch?v=PO4hePKWIGQ "Figure9")

Figure 5: Handwriting recognition sample

In Figure 5, you can see that our face mask detector is capable of running in real-time (and is correct in its predictions as well.



## G.   PROJECT PRESENTATION 

In this project, you learned how to create a COVID-19 face mask detector using OpenCV, Keras/TensorFlow, and Deep Learning.

To create our face mask detector, we trained a two-class model of people wearing masks and people not wearing masks.

We fine-tuned MobileNetV2 on our mask/no mask dataset and obtained a classifier that is ~99% accurate.

We then took this face mask classifier and applied it to both images and real-time video streams by:

- Detecting faces in images/video
- Extracting each individual face
- Applying our face mask classifier

Our face mask detector is accurate, and since we used the MobileNetV2 architecture, it’s also computationally efficient, making it easier to deploy the model to embedded systems (Raspberry Pi, Google Coral, Jetosn, Nano, etc.).

[![demo](https://img.youtube.com/vi/-p7HGwOWxtg/0.jpg)](https://www.youtube.com/watch?v=-p7HGwOWxtg "demo")




