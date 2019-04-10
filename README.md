# EM-method-for-exposing-image-forgeries
Using Expectation-Maximization for exposing image forgeries by revealing inconsistencies in shadow geometry
 -----------------------------------------------------------

 main codes of proposed method are in folder: Shadow_EM(final version)

guidance:

1- Extract folders :Shadow_EM(final version)", "Im"  and  "PontData".

2- in the folder "Shadow_EM(final version)".

3- rum "Main_Shadow_EM_1_1.m" and "Main_Shadow_EM_1_N.m" codes.

4- if you want to run the program by all database run loop version.

5- more information in correspondinding paper and All rights reserved.

  -----------------------------------------------------------
 paper title:
Using Expectation-Maximization for exposing image forgeries by revealing inconsistencies in shadow geometry
  -----------------------------------------------------------
referencing format:

M Nasiri, A Behrad, "Using Expectation-Maximization for exposing image forgeries by revealing inconsistencies in shadow geometry"
journal of Visual Communication and Image Represention(JVCIR), 58,December 2018, DOI:10.1016/j.jvcir.2018.12.007.
 

  This codes estimate shadow vanishing point.
  inputs are match points and initial values for Vp = [Xc, Yc]
  the program optimize [Xc, Yc] based on EM method.
  we determine tampered images based on outlayer number of shadow matches
 
  All parameters are:
 
  MaxIter: Maximum iterition times.
 
  ecr: The minimum limitation of the energy change rate in the iteration
  process.
 
  SigThr: The minimum limitation of the  variance of errors of inliers
  matches(sig2).
 
  Lambda: Percentage of inliers in the samples. This is an inital value
  for EM iteration.
 
  LambdaMinMax: this paprameter limits Maximum and minimum of the variance 
  of errors of inliers matches(sig2). 
 
  Pthr: If the posterior probability of a sample being an inlier is
      larger than theta, then it will be regarded as an inlier.
 
 diagonal: Paramerter of the uniform distribution.
 We assume that the outliers obey a uniform distribution.


  model :
  
  ay+bx+c=0
  
  y - y1 = (y1-y2/x1-x2) * ( x - x1 )
  
  (x2-x1)(yc) + (y1-y2) (xc) + (y2-y1) (x1) +(x1-x2) (y1)=0
  
  a (yc) + b (xc) + c = 0                                            
	
 -----------------------------------------------------------
                                                       
 Copyright (C) 2019 Morteza Nasiri. All rights reserved.  
                   mo.nasiri@shahed.ac.ir              
-----------------------------------------------------------

