Je kunt een TextMeshPro-object gebruiken om de waarde van een variabele weer te geven, zodat de speler deze kan zien. Dit is handig voor het weergeven van variabelen zoals score, punten en levens.

Maak een TextMeshPro-object in het Hierarchy venster.

Voeg een script toe of update het op het GameObject dat de variabele bevat die je wilt weergeven:

--- code ---
---
language: cs
---
using UnityEngine;
using TMPro;

public class SterSpeler: MonoBehaviour
{
  public int sterren = 0; // De variabele die moet worden weergegeven
  public TMP_Text sterTekst; // Het TextMeshPro-object dat moet worden weergegeven

  // Update wordt één keer per frame aangeroepen
  void Update()
  {
    sterTekst.SetText("Sterren: " + sterren);
  }
}
--- /code ---

Sleep het TextMeshPro-object vanuit het Hierarchy venster naar de overeenkomstige eigenschap in het script.

**Test:** Zorg ervoor dat de variabele wordt weergegeven en de waarde wordt bijgewerkt wanneer de variabele wordt bijgewerkt. 
