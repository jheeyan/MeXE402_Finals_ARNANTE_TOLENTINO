# MeXE402_Finals_ARNANTE_TOLENTINO
This is our  Finals Activity for Electives 2 - Machine Learning using Computer Vision for **"Facial Detection of Ben&Ben Band Members"**.

## **Introduction**

**Facial Detection** is referring to the intructions given to a computer or system where an algorithm is used to detect human faces in digital imagges or videos. Compared to the **Facial Recognition**, which identify or name the individual that is detected, whilst **Facial Detection** focuses on detecting presence and location of the faces.

## **Abstract**

This project, titled "**Facial Detection of Ben&Ben Band Members**", focuses on developing a machine learning-based system to automatically detect and recognize the faces of the members of the popular Filipino band, Ben&Ben, in images. The primary goal of the project is to identify faces of the band members in images that is posted online for fan engagement and media production.

The methodology of this Final Activity is to gather images if the Ben&Ben group photos under different conditions i.e. lighting, facial expression, and facial  orientation. The facial detection process utilizes the **Haar** and **LBP Cascade Classifier** algorithm to detect faces in images, identify its location on the image and comparison of the two algorithms. 

The expexted result of this final activity is to create a reliable system for facial detection and compare the two classifier based on performance of facial recognition and evaluate which algorithm is more suited for our context.

## **Project Methods**
+ ****Pre-Procesing****
First, we will choose images that show real people with faces usually a group of people and in this case we will feature the band "Ben & Ben". The main artists of ben & ben are Benjamin and Benjamin. 
<p align="center">
  
![ben ben1](https://github.com/user-attachments/assets/900627f7-b6f5-418e-a746-1abeafa942a3)
![ben ben2](https://github.com/user-attachments/assets/0cc2a93f-3471-4e2e-a6ad-7409aaab2564)
![ben ben3](https://github.com/user-attachments/assets/8a332c47-e937-4319-a1e4-5c04605e1740)
![ben ben4](https://github.com/user-attachments/assets/fc60f79e-1aed-41a0-9c39-8f63e96e8e1b)
![ben ben5](https://github.com/user-attachments/assets/52587110-058d-48b0-8d6f-e8d01312bc02)


</p>

These images were sourced from online and if there is a need for more pictures, it can be easily done so. Selecting these images are done with this line of code.
<p align="center">
<img width="788" alt="select image" src="https://github.com/user-attachments/assets/6aa625f0-7cdc-4a2a-8c4d-27888dd1cbfa" />
</p>

+ ****Face Detection Algorithm****

  
    ****HAAR Cascade**** - are classifiers based on Haar-like features and are widely used for face detection. It uses a         series of features similar to wavelet transforms, representing differences in intensity values across rectangular            regions of an image. These features are used to identify parts of the image that may correspond to an object 

    ****LBP Cascade (Local Binary Patterns)**** -  is a texture descriptor that can be used for face detection and other         image classification tasks. LBP works by comparing pixel intensities in a local neighborhood to form a binary pattern,       which captures texture information.

    Both techniques are widely used but have their specific strengths and limitations depending on the requirements of the       face detection application. This can be selected with this line of code.


<p align="center">
<img width="739" alt="classifier" src="https://github.com/user-attachments/assets/80652c7d-346b-44d9-bad6-1411316e8e55" />
</p>

+ ****Post-processing****
After the image has been selected and a proper classifier has been selected we can proceed to executing its intended code and highlighting whether it has detected a face. We have chosen to use yellow rectangles to highlight faces of the band Ben & Ben.

<p align="center">
<img width="742" alt="selector" src="https://github.com/user-attachments/assets/ab8c9d17-d676-48f4-aaa7-df99c7bea8e1" />
</p>

If ran successfuly, we will see this image or something similar of your selected image. 

<p align="center">
<img width="953" alt="faces" src="https://github.com/user-attachments/assets/43081e3a-f280-45f1-94b8-6a42067535ba" />
</p>

## **Other Results**
The following results compare Haar cascade (Left) vs LBP Cascade (Right)


<p align="center">
  <img width="45%" alt="faces1" src="https://github.com/user-attachments/assets/58f748a7-0ec7-41da-b75c-b5c522d665ac" />
  <img width="45%" alt="facess1" src="https://github.com/user-attachments/assets/3d0b2023-7a4d-46c1-afdb-b78a42352cc2" />

  <img width="45%" alt="faces2" src="https://github.com/user-attachments/assets/ffeccb69-185c-4d34-80eb-e734a8a136fe" />
  <img width="45%" alt="facess2" src="https://github.com/user-attachments/assets/09ac64d8-b286-483d-8cb3-3fd01e206894" />
  
  <img width="45%" alt="faces3" src="https://github.com/user-attachments/assets/0549ae9d-70b8-4e67-a8b3-b30a54ab6796" />
  <img width="45%" alt="facess3" src="https://github.com/user-attachments/assets/41d69cae-6017-411d-a5c3-0acdf76962de" />

  <img width="45%" alt="faces4" src="https://github.com/user-attachments/assets/7e02dda1-47b4-4126-92d6-195cfd74c115" />
  <img width="45%" alt="facess4" src="https://github.com/user-attachments/assets/cea4b6ae-2d9f-46ac-8351-2ec05c6702a9" />

  <img width="45%" alt="faces5" src="https://github.com/user-attachments/assets/0876f624-5a33-4040-8ec8-74a29802b585" />
  <img width="45%" alt="facess5" src="https://github.com/user-attachments/assets/9de7400d-09b4-49b4-8517-d8dd639c27dc" />

</p>

## **Conclusion**
After testing and comparing haar cascade and lbp cascade we can conclude that haar cascading performs much more effectively in this case since front-facing models such as these pictures benefit haar cascade. Though, it has been said that lbp cascade is more robust in illumination changes in detectng faces it was not able to detect some faces in our case. Therefore, haar cascading is reliable for speedy face detection and it is ideal to have front facing models while lbp cascade is also a good algorithm albeit more complex, sensitive to pose changes, and that it is used often alongside other algorithms

