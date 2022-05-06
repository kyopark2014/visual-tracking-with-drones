# Visual Tracking with Drones

여기서는 드론을 이용하여 물체를 Targeting을 하고, 두개 이상의 드론이 하나의 물체를 보았을때 이를 기반으로 정확한 위치를 특정합니다. 이후 물체가 이동방향이나 거리를 예측하는 Tracking Algorithm을 이용하여, 이동하는 Object의 다음 위치를 예측함으로, 드론들이 좀 더 정확하게 해당 물체를 추적할 수 있도록 돕습니다. 

아래와 같이 2대의 드론이 Object Detection을 통해 같은 물체임을 인지하면, 드론의 GPS 위치와 카메라의 물체 좌표를 이용하여 물체의 위치를 Location Extraction 방법으로 알 수 있습니다. 이후 Tracking 알고리즘을 이용해 물체의 다음 위치를 예측하여 드론의 위치를 조정 할 수 있습니다. 이와 같이 얻어진 정보는 AWS Cloud Infrastructure를 이용하여 Sharing이 가능합니다.

<img width="710" alt="image" src="https://user-images.githubusercontent.com/52392004/167048892-aa59253d-62a6-48b8-888f-1abaab3dd81a.png">

물체의 형상은 Amazon Rekognition을 이용하여 수행합니다. 이때, 2대 이상의 드론이 하나의 물체를 잡으면, [Visual Localization Algorithm](https://github.com/kyopark2014/Visual_Localization)을 이용하여 물체의 정확한 좌표를 알 수 있습니다. 또한 [Obejct Tracking Algorithm](https://github.com/kyopark2014/Object_Tracking_Algorithm)을 이용하며 이동하는 물체의 다음 위치를 예상할 수 있습니다. 이 2가지 알고리즘을 이용하면, 움직이는 물체의 다음 위치를 기반으로 지속적인 트래킹을 가능하게 하여 정확도를 높일 수 있습니다.


