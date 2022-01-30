# HeadPoseEstimation

I have used the tensorflow.js model <a href="https://github.com/tensorflow/tfjs-models/tree/master/facemesh">MediaPipe Facemesh</a> to estimate 
the head pose in real time using the device's camera as used in <a href="https://github.com/paruby/snake-face">snake-face</a>.
The direction in which the head is pointing at start is estimated as a reference point. 
Subsequent estimates are compared to this to angle.


The head direction is estimated by calculating the vectors connecting
the centre of the lips to the left and right cheeks. These two vectors lie
on a plane that approximates the surface of the face. The cross product of these
vectors is normal to this plane and thus points approximately in the direction
of the head.


https://user-images.githubusercontent.com/64319078/151691938-e1ef764c-ccbb-4ece-b319-4d6dbe6f1ed7.mov

https://user-images.githubusercontent.com/64319078/151691966-02900362-eb42-4815-8b9f-a5ebfa6a4d43.mov

https://user-images.githubusercontent.com/64319078/151691994-1b7711f7-af4b-45ce-bfcc-7d6718df629f.mov

https://user-images.githubusercontent.com/64319078/151692025-82589f65-8d5f-46bf-8332-357f94808b5a.mov

