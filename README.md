# Training Flappy Bird
## I have a schedule to keep working with `Flappy Bird`
- [x] How to create spirits **lorence_impl_make_spirit**
- [ ] 
- [ ] 
- [ ]
- [ ]
- [ ]
- [ ]
- [ ]
- [ ]
- [ ]
## --------------------------------------------------------------------------------------------
> - **lorence_impl_make_spirit**
- [x] Create new folder with name *LorenceCreateAssetsFolder*
- [x] Import New Asset at position[Mouse click on *LorenceCreateAssetsFolder*]
- [x] Open **Spirit Editor** to separate into small *spirit*
- [x] It's done
- [ ] ... Continue in the feature
Image for description
## --------------------------------------------------------------------------------------------
> - **Observe position of *Camera***
>> - There are two cases here:

    public class CameraController : MonoBehaviour {

      public Transform targetBird;
      public float positionCamera;
      public float positionTargetBird;

      // Update is called once per frame
      void Update () {
        positionCamera = this.transform.position.x;
        positionTargetBird = targetBird.position.x;
        this.transform.position = new Vector3 (targetBird.position.x,0,-10);
      }
    }

![alt text](https://github.com/danisluis4/Training-Flappy-Bird/blob/Training-Game-Basic/Training/1.png)
>> - One case: You don't attach TargetBird to Camera.

    using System.Collections;
    using System.Collections.Generic;
    using UnityEngine;

    public class CameraController : MonoBehaviour {

        public Transform targetBird;
        public float positionCamera;
        public float positionTargetBird;

        // Update is called once per frame
        void Update () {
            positionCamera = this.transform.position.x;
            positionTargetBird = targetBird.position.x;
            this.transform.position = new Vector3 (targetBird.position.x,0,-10);
        }
    }

