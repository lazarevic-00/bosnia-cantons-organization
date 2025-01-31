![Bosnia and Herzegovina Map](https://upload.wikimedia.org/wikipedia/commons/thumb/b/bf/Flag_of_Bosnia_and_Herzegovina.svg/255px-Flag_of_Bosnia_and_Herzegovina.svg.png)  
*Flag map of Bosnia and Herzegovina ([Source](https://commons.wikimedia.org/wiki/File:Flag-map_of_Bosnia_and_Herzegovina.svg))*

---

## Features
- **Machine-readable JSON** data for entities, cantons, and municipalities.
- Covers both the **Federation of Bosnia and Herzegovina** (10 cantons) and **Republika Srpska** (municipalities).
- Includes cities split between entities (e.g., Sarajevo, Doboj).
- **Self-governing Brčko District** as a separate unit.

---

## Data Structure
### Example JSON

```json
{
  "entities": [
    {
      "name": "Federation of Bosnia and Herzegovina",
      "key": "federation-of-bosnia-herzegovina",
      "type": "federation",
      "cantons": [
        {
          "name": "Una-Sana Canton",
          "key": "una-sana-canton",
          "places": ["Bihać", "Cazin", ...]
        },
        ...
      ]
    },
    {
      "name": "Republic of Srspka",
      "key": "republic-srspka",
      "type": "entity",
      "cantons": [
        {
          "name": "Banjalučka",
          "key": "banja-luka",
          "places": ["Banja Luka", "Čelinac"...]
        },
        ...
    },
    {
      "name": "Brčko District",
      "key": "brcko-district",
      "type": "self-governing",
      "cantons": [
        {
          "name": "Brčko",
          "key": "brcko",
          "places": ["Brčko"]
        },
    },
  ]
}
