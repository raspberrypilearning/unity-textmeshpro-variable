Tu peux utiliser un objet TextMeshPro pour afficher la valeur d'une variable afin que le joueur puisse la voir. Ceci est utile pour afficher des variables telles que le score, les points et les vies.

Crée un objet TextMeshPro dans la fenêtre Hierarchy.

Ajoute, ou mets à jour, un script sur le GameObject qui possède la variable que tu veux afficher :

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

Fais glisser l'objet TextMeshPro de la fenêtre Hierarchy vers la propriété correspondante dans le script.

**Test :** assure-toi que la variable est affichée et se met à jour lorsque la variable est actualisée. 
