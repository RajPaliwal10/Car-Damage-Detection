# Car-Damage-Detection

---

## Demo 
![car_video](https://user-images.githubusercontent.com/63935255/189545661-c48b0296-29ea-4005-922b-969fc5c20565.gif)

---
## Team members
   - [Prem Jha](https://github.com/tenserebel)
   - [Rana Karn](https://github.com/Rkarn1125)
   - [Rahul Gupta](https://github.com/RahulGupta77)
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
   - I worked on the Data cleaning, preprocessing and annotation part of this project.
   
---
### Model Buliding Procedure 

1. **Data collection and cleaning** : We labelled our own dataset using LabelImg library. The dataset consists of 2000+ images of damaged and undamaged cars. Further the damaged cars are labelled into 4 catogeries (Labels) Dent, Scratch, Broken-glass, Smashed. 

2. **Data preprocessing** : The output from the LabelImg library is an .xml file consisting the co-ordinates of labelled region. Those .xml files were converted .csv files along with their image name. Furhther the .csv files were converted into .record format for feeding into the model. 

3. **Model training** : Two models were trained, 1st to check whether the given car image is damaged or not. If the car is damaged then 2nd model was used to identify the type of damage. 
