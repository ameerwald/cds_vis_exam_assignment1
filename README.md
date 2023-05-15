
# Assignment 1 - Building a simple image search algorithm

This assignment can be found at my github [repo](https://github.com/ameerwald/cds_lang_exam_assignment1).

The dataset is a collection of over 1000 images of flowers, sampled from 17 different species. The dataset comes from the Visual Geometry Group at the University of Oxford, and full details of the data can be found [here](https://www.robots.ox.ac.uk/~vgg/data/flowers/17/).

For this assignment, we were asked to use  ```OpenCV``` to design a simple image search algorithm. The criteria are as follows:

- Define a particular image to work with 
- For that image
  - Extract the colour histogram using ```OpenCV```
- Extract colour histograms for all of the **other* images in the data
- Compare the histogram of the chosen image to all of the other histograms 
  - For this, use the ```cv2.compareHist()``` function with the ```cv2.HISTCMP_CHISQR``` metric
- Find the five images which are most simlar to the target image
  - Save a CSV file to the folder called ```out```, showing the five most similar images and the distance metric:

|Filename|Distance]
|---|---|
|target|0.0|
|filename1|---|
|filename2|---|


## Repository 

| Folder         | Description          
| ------------- |:-------------:
| Data      | The flowers dataset      
| Notes  | Jupyter notebook with notes, used to create .py script  
| Out  | List of the 5 most similiar flowers to my chosen flower    
| Src  | Py script for the image search alogorithm  
| Utils  | Taken from class notebook, using two functions to show images 

## To run the scripts 

From the command line, at the assignment 1 folder level, run the following chunk of code. If it is run within a folder in assignment 1 the file paths need to be edited. 
``` 
bash setup.sh
bash run.sh
```

This has been run on an ubuntu system on ucloud and therefore could have issues when run another way. 

