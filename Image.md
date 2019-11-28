## opencv 和 PIL.Image 图像格式转换
~~~
        import cv2
        import numpy
        from PIL import Image
        
  # OpenCV To PIL.Image
        opencv_img = cv2.imread('1.jpg')
        PIL_img = Image.fromarray(cv2.cvtColor(opencv_img, cv2.COLOR_BGR2RGB))
        
  # PIL.Image To Opencv
        PIL_img = Image.open('1.jpg')
        opencv_img = cv2.cvtColor(numpy.asarray(image), cv2.COLOR_RGB2BGR)
        
~~~
