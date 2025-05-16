# CV_Super_Resolution
In this project, the goal is to enhance input image quality by training a neural network on the super resolution problem.
The super resolution problem is a computer vision challenge that involves training a network to enhance the resolution of input images.
This technology has multiple applications in industry:

- Enhancing old low-quality images
- Video game development: rendering can be done at lower resolution and then enhanced by a network, reducing computational demands
- Medical imaging enhancement
- Satellite imagery improvement

I have implemented and experimented with several small network architectures for this task:

Each pixel is reconstructed by considering itself and the 8 neighboring pixels around it
Training data requirements are minimal since each image has thousands of pixels, allowing effective training with just a few sample images
Considering the RGB channels, we have 27 inputs (3 channels × 9 pixels) and 3 outputs (the enhanced RGB values)

The final architecture used in this project consists of a simple neural network with:
27 inputs → 48 neurons → 32 neurons → 3 outputs
![image](https://github.com/user-attachments/assets/40401995-de28-4a61-92dc-a55ffb6ac347)



Outputs: Left is original (low-resolution image) => Right is the enhanced image
![image](https://github.com/user-attachments/assets/dd30de47-bf98-4b64-95e1-ffd97cec16fc)
![image](https://github.com/user-attachments/assets/7a0ee702-df72-4410-b898-6cbc608bfe61)
![image](https://github.com/user-attachments/assets/cbe50ce3-69e0-4bb5-9bc2-4a6060dd931d)
