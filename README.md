# Batch processing to video for Fast Style Transfer for Arbitrary Styles

Using the model code in magenta: https://github.com/tensorflow/magenta/tree/master/magenta/models/arbitrary_image_stylization

From the TensorFlow Hub: https://tfhub.dev/google/magenta/arbitrary-image-stylization-v1-256/2

and the publication:
    Exploring the structure of a real-time, arbitrary neural artistic stylization network. Golnaz Ghiasi, Honglak Lee, Manjunath Kudlur, Vincent Dumoulin, Jonathon Shlens, Proceedings of the British Machine Vision Conference (BMVC), 2017.: https://arxiv.org/abs/1705.06830
    
    
### Description:
This notebook uses imageio to feed frames from videos or images from an image sequence into a Fast Style Transfer for Arbitrary Styles model and write the results to a frame in a new video.

### Windows 10 Installation Guide:
There are many installation guides for tensorflow. I was able to install most of them, but only one method allowed tensorflow to recognize my GPU. So I wanted to provide some information about how I managed to get it working in case it's useful for someone- until this instruction also becomes outdated.

This setup guide ended up being the one that worked for me:
https://medium.com/analytics-vidhya/tensorflow-2-3-0-with-gpu-support-on-windows-10-f975a552ea7c

CUDA 10.2 did work with tensorflow like the article suggests, but it would not recognize my GPU. So I tried 10.1.

Versions were really tricky to get right, here are versions I used:

* Anaconda3 2020.11 (Python 3.8.5 64-bit)
* cuda_10.1.243 
* cudnn 10.1 v7.6.5.32 (This exact version was important)
* tensorflow 2.3.0 for Python 3.8

### Example of results 

https://www.instagram.com/p/CEVx4UJhBlS/?utm_source=ig_web_copy_link

https://www.instagram.com/p/CEdVBdQBTks/?utm_source=ig_web_copy_link

https://www.instagram.com/p/CEcwkh8hiFv/?utm_source=ig_web_copy_link

https://www.instagram.com/p/CEWaEqLBKdF/?utm_source=ig_web_copy_link

https://www.instagram.com/p/CEWD0gGBMoP/?utm_source=ig_web_copy_link
