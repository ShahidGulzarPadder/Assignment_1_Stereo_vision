# Assignment_1_Stereo_vision
First assignment of 3DSSF

Design and implementation of these stereo-matching schemes:
> Naive stereo matching.
          with Normal and Parallel execution
> Dynamic programming approach.
          with Normal and Parallel execution 
          
> Comparison of solution to an existing implementation

> Displaying the output disparity images (e.g. using OpenCV).
    
> Given the input camera parameters conversion of the disparities to 3D point cloud.

    saved it in a file .xyz format as suggested and can be found in outputs folder of each data,
    
Input data

I have used Middlebury stereo datasets with standard focal length 3740 and 160mm baseline.

I have uploaded only one output folder of Aloe pair with name OP-Aloe, due to size limitation on Github I cannot upload more than 25MB but I will discuss everything in the documentation

# ALOE
<img width="761" alt="ALOE" src="https://user-images.githubusercontent.com/80226882/142281527-bd99edb9-e265-49f6-a694-0b1b883e6cc0.png">

# BABY1
<img width="766" alt="BABY1" src="https://user-images.githubusercontent.com/80226882/142281255-3d70a61d-480e-46c7-bae4-fe1f62cbe46c.png">

# BOOKS
<img width="778" alt="BOOKS" src="https://user-images.githubusercontent.com/80226882/142282881-3f7d3ccc-6fa2-4e5c-bffd-c196bb95ac24.png">

# CONES
<img width="781" alt="CONES" src="https://user-images.githubusercontent.com/80226882/142283877-1e5c2308-8d01-4c11-b176-026f47d7e226.png">

# TEDDY
<img width="776" alt="Teddy" src="https://user-images.githubusercontent.com/80226882/142284993-7b258f72-51cd-4f4e-9152-98f833637e0b.png">

# ART
<img width="772" alt="ART" src="https://user-images.githubusercontent.com/80226882/142286726-08cbdfd6-822f-4f05-9828-95e5721a13d8.png">

| WINDOW = 3                   | ART            | BOOKS        | CONES      | TEDDY      | BABY1      | ALOE      |
| -------------                |  ------------- | ------------ | ---------- | ---------- | ---------- | --------- |
| Naive Computation time (s)   | 24.7           | 24.13        | 1.22       | 1.25       | 3.00       | 3.15      |
| Dynamic computation time (s) | 36.2           | 36.64        | 1.33       | 1.42       | 3.77       | 4.07      |
| WINDOW = 5                   |                |              |            |            |            |           |
| Naive Computation time (s)   | 51.15          | 51.70        | 2.24       | 2.34       | 5.71       | 6.12      |
| Dynamic computation time (s) | 106.7          | 110.63       | 2.39       | 2.28       | 6.79       | 7.30      |
| WINDOW = 7                   |                |              |            |            |            |           |
| Naive Computation time (s)   | 88.13          | 88.78        | 3.33       | 3.68       | 9.04       | 10.07     |
| Dynamic computation time (s) | 175.5          | 105.9        | 3.73       | 3.68       | 10.77      | 11.60     |

