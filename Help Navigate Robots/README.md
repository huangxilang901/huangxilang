This is the competition from kaggle `Help Navigate Robots`  
In this competition, we are going to help robots recognize the floor surface that they're standing on using data collected from 10 sensor(position, velocity, acceleration)  

Although we have got the sensor data, but it's necessary to create new features for the classification task, as that can be the critical factor to predict the surface which robots are standing on.

# Data  
![image](https://github.com/huangxilang901/huangxilang/blob/master/Help%20Navigate%20Robots/images/캡처.JPG)  
row_id: The ID for this row.  
series_id: ID number for the measurement series.  
measurement_number: Measurement number within the series.  
orientation_X, orientation_Y,... : The 10 sensor channels describe the oriented as a quaternion, angular velocity, and acceleration.  
As analyzing the given data, we can find that there are 4 coordinates: X,Y,Z,W  
Usually we have X,Y,Z - Euler Angles. So it's necessary to convert quaternions to euler which we are more familiar with.
