# Semantic and instance segmentation using Mask R-CNN 

Developed the python script to detect the lane lines in the input images and videos using classic computer vision methods.

## Semantic segmentation on images
1. Input Images

    <img src="https://github.com/Ank-G/Segmentation-using-Mask-R-CNN/blob/main/images/road.png" width=45% height=45%>

2. Converting the input RGB image to the Grayscale and also removing the noise by applying Gaussian filter

    <img src="https://github.com/Ank-G/Segmentation-using-Mask-R-CNN/tree/main/output/semantic_road.png" width=45% height=45%>
    
3. Edge Detection: Apply the canny edge detection algo to enhances the edges in the grayscale image

    ![image](https://user-images.githubusercontent.com/62834697/195821941-16f953a4-d6f4-40aa-bb91-51a1826dd3c2.png)

4. Masking: Masked the region which is not area of interest, then apply the canny edge detector

    ![image](https://user-images.githubusercontent.com/62834697/195822323-44194c02-a987-47ae-8074-232133223ea5.png)

5. Hough Transforms: Detected the lines of interest in the masked image using Hough Transformation.

    ![image](https://user-images.githubusercontent.com/62834697/195822991-530e10e6-c815-49f9-91db-0d065918da17.png)
    
4. Output: 

    ![image](https://user-images.githubusercontent.com/62834697/195823115-2ec5a75d-e63e-44be-891b-e17dbe91ddd5.png)


Applying the same approach on a video (a series of images) and following is the final output:


https://user-images.githubusercontent.com/81529956/179659027-468cc44c-40e4-4d54-80e9-562f33fe7828.mp4
