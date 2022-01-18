# Object Tracking Overview
Object tracking is an important and practical topic that has a very long history and has been applied to numerous fields. At a high level, tracking refers to estimating the state of an object (e.g., position and velocity) based on sensor measurements, and predicting its future location. For example, tracking the location of an aircraft based on radar measurements is a typical application of tracking. In the context of computer vision, tracking typically refers to processing video frames and predicting the location of an object (or multiple objects), in future video frames.

In computer vision, this is accomplished using a motion model and an appearance model. The motion model will estimate the position and velocity of an object and use that information to predict the location of an object in future video frames and the appearance model encodes what the object looks like and then search the region around the predicted location from the motion model to then fine-tune the location of the object. So the motion model is an approximation to where the object might be located in a future video frame and the appearance model is used to fine-tune that estimate.

## Tracking Models Available in the OpenCV Tracker Class
OpenCV contains an API Tracker Class that includes several different tracker models which are all based on different algorithms. Depending on the application one model might be better suited than another. 

- BOOSTING
- CSRT
- KCF
- MEDIANFLOW
- MIL
- MOSSE
- TLD

More details at: https://docs.opencv.org/4.5.2/d0/d0a/classcv_1_1Tracker.html

## Output Sample

<img width="966" alt="Screen Shot 2022-01-17 at 10 52 32 PM" src="https://user-images.githubusercontent.com/42128166/149892152-c9c0fbaf-41d9-471f-97c0-5d7b4e5cb42d.png">

(Video Source: https://www.pexels.com/video/drone-footage-of-a-person-riding-a-bicycle-5619700/)

