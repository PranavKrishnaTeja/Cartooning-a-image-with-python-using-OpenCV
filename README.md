# Cartooning-a-image-with-python-using-OpenCV
This a funtime project just to get familiar with the cv2 commands

please read before this because if you do not have any idea about the commands in the code and you just mess with the code your desired image may not be there also the image must be in the same directory where you save your python or ipynb files.

// code explanation

cv2.imshow('output name of the photo',input of the pic)//it means the output window should have a name you desire and the input should be the variable you declare inside the code i.e i have used variable like color,gray,edges

edges = cv2.adaptiveThreshold(gray, 255, cv2.ADAPTIVE_THRESH_MEAN_C, cv2.THRESH_BINARY, 9, 5)/// the maximum adaptive threshold of the gray color is 255 you can increase the number but there will be no change, and if you need the edges with broader lines you need to increase the first value of THRESH_BINARY and the second value must be less for recognising more of the edges(meaning if you increase the value beyond a certain number you can notice the actual  final image being blurred) 

gray = cv2.medianBlur(gray, 5)// the number cannot exceed beyond 9 and be aware that if the value is at 9 meaning the image sharpness will be reduced  so choose the number which suits you

color = cv2.bilateralFilter(img, x, y, z)// we use bilateralFilter because we need to keep the edges and at the same time blur effect so we use bilateralFilter and  the x in this part of the code is the block size of the image for which we need to apply the filter and y,z are the values that give you the cartoonish effect the higher the value the more cartoonish is image and less sharpness the image has.


/////// do follow me in github and give a star for the repository if you like the content and my hard work///////
