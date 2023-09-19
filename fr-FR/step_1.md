Tu peux utiliser un objet TextMeshPro pour afficher la valeur d'une variable afin que le joueur puisse la voir. Ceci est utile pour afficher des variables telles que le score, les points et les vies.

Crée un objet TextMeshPro dans la fenêtre Hierarchy.

Ajoute, ou mets à jour, un script sur le GameObject qui possède la variable que tu veux afficher :

--- code ---
---
language: cs
---
using UnityEngine;
using TMPro;

public class JoueurEtoile: MonoBehaviour
{
  public int etoiles = 0; // La variable à afficher
  public TMP_Text texteEtoile; // L'objet TextMeshPro à afficher

  // Update est appelée une fois par image
  void Update()
  {
    texteEtoile.SetText("Étoiles : " + etoiles);
  }
}
--- /code ---

Fais glisser l'objet TextMeshPro de la fenêtre Hierarchy vers la propriété correspondante dans le script.

**Test :** assure-toi que la variable est affichée et se met à jour lorsque la variable est actualisée. 
