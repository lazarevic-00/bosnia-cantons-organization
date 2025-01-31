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
      "type": "federation",
      "cantons": [
        {
          "name": "Una-Sana Canton",
          "cities": ["Bihać", "Cazin", ...]
        },
        ...
      ]
    },
    {
      "name": "Republika Srpska",
      "type": "entity",
      "municipalities": ["Banja Luka", "Bijeljina", ...]
    },
    {
      "name": "Brčko District",
      "type": "self-governing",
      "cities": ["Brčko"]
    }
  ]
}
