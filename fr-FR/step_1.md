You can use a TextMeshPro object to display the value of a variable so that the player can see it. This is useful for displaying variables such as score, points, and lives.

Create a TextMeshPro object in the Hierarchy window.

Add, or update, a script on the GameObject that has the variable you want to display:

--- code ---
---
language: cs
---
using UnityEngine; using TMPro;

public class StarPlayer: MonoBehaviour
{ public int stars = 0; // The variable to display public TMP_Text starText; // The TextMeshPro object to display

  // Update is called once per frame void Update()
  {
    starText.SetText("Stars: " + stars);
  }
} --- /code ---

Drag the TextMeshPro object from the Hierarchy window to the corresponding property in the script.

**Test:** Make sure the variable is displayed and updates when the variable is updated. 
