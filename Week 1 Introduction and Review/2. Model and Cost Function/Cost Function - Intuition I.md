If we try to think of it in visual terms, our training data set is scattered on the x-y plane. We are trying to make a straight line (defined by $h_\theta(x)$) which passes through these scattered data points.

Our objective is to get the best possible line. The best possible line will be such so that the average squared vertical distances of the scattered points from the line will be the least. Ideally, the line should pass through all the points of our training data set. In such a case, the value of $J(\theta_0,\theta_1)$ will be 0. The following example shows the ideal situation where we have a cost function of 0.

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/_B8TJZtREea33w76dwnDIg_3e3d4433e32478f8df446d0b6da26c27_Screenshot-2016-10-26-00.57.56.png?expiry=1653350400000&hmac=DUFb0iRlGPBVkDVzny_Itvea2gqq4EvyVj_BaYtcKIY)

When $\theta_1=1$, we get a slope of 1 which goes through every single data point in our model. Conversely, when $\theta_1=0.5$, we see the vertical distance from our fit to the data points increase.

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/8guexptSEeanbxIMvDC87g_3d86874dfd37b8e3c53c9f6cfa94676c_Screenshot-2016-10-26-01.03.07.png?expiry=1653350400000&hmac=pyUoC9hbQCC-Oisuj881Tap2aP5JY88CB-Qz4Gol8B0)

This increases our cost function to 0.58. Plotting several other points yields to the following graph:

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/fph0S5tTEeajtg5TyD0vYA_9b28bdfeb34b2d4914d0b64903735cf1_Screenshot-2016-10-26-01.09.05.png?expiry=1653350400000&hmac=oY4mej7orofuUuHuanTiYnPqtyyP6aGvbhZDGQkqZf4)

Thus as a goal, we should try to minimize the cost function. In this case, $\theta_1=1$ is our global minimum.