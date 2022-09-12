# **Car-damage-detection**

---

## Demo 
![car_video](https://user-images.githubusercontent.com/63935255/189545661-c48b0296-29ea-4005-922b-969fc5c20565.gif)

---
## Team members
   - [Prem Jha](https://github.com/tenserebel)
   - [Rana Karn](https://github.com/Rkarn1125)
---
## Tech Stack used 

   - Python
   - React (for frontend)
   - Flask API (for model deployment) 
   
---
## Libraries used 
   - Tensorflow
   - LabelImg
   - Matplotlib
   - Pandas 
   - Numpy
 
---
## Project Description

   - This is a Car damage detection web app which detects the type of car damage in a given image
   - The model automatically generates bounding boxes around the damaged area. 
   - I worked on the Machine Learning side of the project.
   
---
### Model Buliding Procedure 

1. **Data collection and cleaning** : We labelled our own dataset using LabelImg library. The dataset consists of 2000+ images of damaged and undamaged cars. Further the damaged cars are labelled into 4 catogeries (Labels) Dent, Scratch, Broken-glass, Smashed. 

2. **Data preprocessing** : The output from the LabelImg library is an .xml file consisting the co-ordinates of labelled region. Those .xml files were converted .csv files along with their image name. Furhther the .csv files were converted into .record format for feeding into the model. 

3. **Model training** : Two models were trained, 1st to check whether the given car image is damaged or not. If the car is damaged then 2nd model was used to identify the type of damage. Both models were trained using transfer learning. Ssd_resnet_50 model from [here](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf1_detection_zoo.md) was used as a pretrained model. 

--- 
### Output 

1. **Tensorboard for damaged classification model:**

![damage model](https://user-images.githubusercontent.com/63935255/189546365-558946c2-3d63-41c8-afda-dfbdea69f7f5.png)

2. **Tensorboard for Undamaged classification model:**

![Undamaged model](https://user-images.githubusercontent.com/63935255/189546401-ff8de498-d185-436a-abcf-fec0a4543e1c.png)

3. **Undamage prediction:**

![detection_output2](https://user-images.githubusercontent.com/63935255/189546488-97b29041-c33c-4397-b29f-3a8886c00662.png)

4. **Damage prediction:**

![detection_output4](https://user-images.githubusercontent.com/63935255/189546594-cace959c-8f8a-402e-8081-f8e238a7df1c.png)

![detection_output12](https://user-images.githubusercontent.com/63935255/189546604-7df738dc-a25f-43cc-8bd2-54357d934380.png)

![detection_output6](https://user-images.githubusercontent.com/63935255/189546618-e34a723b-ae82-4ece-805f-41a195817de0.png)

![detection_output17](https://user-images.githubusercontent.com/63935255/189546631-a1f72939-321f-4fed-82e5-b0aa9d95293c.png)




