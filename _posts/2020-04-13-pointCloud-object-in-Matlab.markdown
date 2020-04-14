---
layout: post
title:  "pointCloud in Matlab"
date:   2020-04-13 00:03:49 -0400
categories: jekyll update
---
### pointCloud
Matlab provides an object for storing 3D point cloud.



here is an pointCloud example:

```
ds_pointcloud = 

pointCloud with properties:

   Location: [30×40×3 double]
      Color: [30×40×3 uint8]
     Normal: []
  Intensity: []
      Count: 1200
    XLimits: [-0.7151 0.9876]
    YLimits: [-0.4939 0.5317]
    ZLimits: [0.6847 1.8204]
```

![example][pointcloud]


Check out the [matlab-pointCloud-page][matlab-pointCloud-page] for more info on this.

[matlab-pointCloud-page]:https://www.mathworks.com/help/vision/ref/pointcloud.html

[pointcloud]: /img/pointcloud/ds_pointcloud.png "example"


