# Ex.No: 3  Basic movements in Unity 
### DATE:                                                                            
### REGISTER NUMBER : 212223240047
### AIM: 
 To learn the basic movements translation,scaling and rotation of game objects through code.
### Procedure:
1. Setup the Scene
2. Open Unity and create a 3D Scene.
3. Add three objects:Cube → Rename to Object1 (for movement),Sphere → Rename to Object2 (for rotation).Capsule → Rename to Object3 (for scaling).
4. Add the Script,Create a C# Script → Name it TransformOperations.cs.
5. Write the code for translation,scaling and rotation,save and close the script
6. Save the script
7. Select any empty GameObject (or create one: GameObject → Create Empty).
8. Attach the TransformOperations script to it.
9. In the Inspector, assign Object1 → Drag the Cube,Object2 → Drag the Sphere.Object3 → Drag the Capsule.
10. Run the Scene Press Play ▶️ in Unity
11. Stop the program.
### Program 
```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;
public class EXP_3 : MonoBehaviour
{
    public Transform o1;
    public Transform o2;
    public Transform o3;
    // Start is called before the first frame update
    void Start()
    {
    
    }

    // Update is called once per frame
    void Update()
    {
        if (Input.GetKeyUp(KeyCode.X))
        {
            o1.Translate(0.2f, 0, 0);
        }
        if (Input.GetKeyUp(KeyCode.Y))
        {
            o2.Rotate(0.9f, 0, 0);
        }
        if (Input.GetKeyUp(KeyCode.Z))
        {
            o3.localScale += new Vector3(0, 0.2f, 0);
        }
    }
}

```
### Output:

### Initial Position of objects
<img width="905" height="934" alt="Screenshot 2026-03-09 210407" src="https://github.com/user-attachments/assets/c16c3650-d9b5-422f-98ac-f6c894d5aa7e" />

### After movement
<img width="909" height="967" alt="Screenshot 2026-03-09 210437" src="https://github.com/user-attachments/assets/fd38b416-9ef8-41d3-a984-e6bd1f2e58d3" />

### Result:
Thus the basic movement is learned through scripting
