# PROJECT OVERVIEW
## D. PROJECT EXECUTION
### Project Design and Coding

![image](https://user-images.githubusercontent.com/122180771/211359684-ffd41939-77a2-44b7-8223-0636348ffdbc.png)

Flowchart Design:

Tumor Detection Implementation Example

# Description of the project and implementation

Coding and function required:

**anisodiff_function.m**

This system require a seperate function that can convert input image, center the distance of the pixels from the image, creating a 2d convulation masks and adapting anisotropic diffusion, also called Perona–Malik diffusion,which is a technique aiming at reducing image noise without removing significant parts of the image content, typically edges, lines or other details that are important for the interpretation of the image

![image](https://user-images.githubusercontent.com/121602144/211653080-764fab0b-001b-4a57-83f1-79566916e4f9.png)
![image](https://user-images.githubusercontent.com/121602144/211653163-eef58649-2e2b-45ed-bc1d-0d40b95e4aa2.png)
![image](https://user-images.githubusercontent.com/121602144/211653226-c402e649-5116-4dd3-bb08-4b64b4204ea3.png)

<br>


**Final_Brain_Tumor.m**

This whole example are the main coding of this system. it consists of %% Input function, %% Filter function, %% thresholding funtion, %% Morphological function, %% Bounding box function, %% Tumor outline function, %% subtracting function, %% inserting the outline function and %% Display function

<br>

![image](https://user-images.githubusercontent.com/121602144/211661137-d0692a91-a765-4ce9-91c6-8f4e7340a066.png)
<br><br>

    The %% Input function is used so that the system can accept input image. It works by user selecting their own image from their folder
    The %% Filter function is used to load the separate anisodiff_function.m to Final_Brain_Tumor.m



![image](https://user-images.githubusercontent.com/121602144/211661267-ce354565-5e79-4a40-948d-5bf44eaec8c9.png)
<br><br>

    The %% Thresholding function is used to segment input images. In digital image processing, thresholding is the simplest method of segmenting images. From a grayscale image, thresholding can be used to create binary images

![image](https://user-images.githubusercontent.com/121602144/211661405-1c9d8133-60ad-4b37-92e1-dc157bbef847.png)

<br><br>

    The %% Morphological function is used to process images based on shapes. In a morphological operation, each pixel in the image is adjusted based on the value of other pixels in its neighborhood. By choosing the size and shape of the neighborhood, we can construct a morphological operation that is sensitive to specific shapes in the input image
    
![image](https://user-images.githubusercontent.com/121602144/211661447-d4d78ec5-4746-4692-ae49-f6a77db2d545.png)

<br><br>

    The %% Bounding box function is used to create a box to mark the tumor
    
![image](https://user-images.githubusercontent.com/121602144/211661504-a3e85804-4cd2-445c-b6d1-9913a8fc456c.png)
![image](https://user-images.githubusercontent.com/121602144/211661682-8394f38c-fcaa-4635-abd8-0972c7d4e280.png)

<br><br>

    The %% Tumor outline function is used to detect the outline of the tumor by using filling, eroding and subtracting method
    
![image](https://user-images.githubusercontent.com/121602144/211661828-268f1f43-1590-4be5-9794-75aae61ed669.png)

<br><br>

    The %% Tumor outline function is used to detect the outline of the tumor by using filling, eroding and subtracting method
    
![image](https://user-images.githubusercontent.com/121602144/211661861-b695d13c-1a71-4dbf-90dd-66957ad9b56b.png)

<br><br>

    The %% Display function is used to display the results of the system and combined it all in one output
    







# Project Result

If tumor was found:
![image](https://user-images.githubusercontent.com/121602144/211649739-7d5fae98-f89d-4e7b-82d2-ac9277604448.png)

<br><br>

If tumor was not found:
![image](https://user-images.githubusercontent.com/121602144/211650270-812b9e1d-84c6-400a-852c-e2516f1e5758.png)
