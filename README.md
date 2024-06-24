# object-identifier-and-camera-to-object-and-object-to-object-distance-estimator
Identifies different object classes(coco dataset), calculates camera to object distance and object to object distance.

Part 1: detects objectes defined in https://cocodataset.org/#home along with confidence score of each object.
SSD MobileNet architecture of dnn used.

Part 2: calculates distance between camera to object.
Haar-cascade-classifier(for frontal face detection) used.
for this part, instead of lena.png, use a captured image at a distance of 30 Inches(can be changed) from camera and measure the face width at that point.
similar to the below description:


The output for Part 1 and Part 2 is shown below:



Part 3: calculates the midpoint of each bounding box and euclidean distance is calculated between two object midpoints:



For single object identified: 



Final output:

https://user-images.githubusercontent.com/75139237/123779034-5e8cc800-d8ef-11eb-9d60-da0dc9882615.mp4


