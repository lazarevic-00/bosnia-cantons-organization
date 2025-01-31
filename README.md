
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
```
## Usage
- First, install the package in your JavaScript project using npm:

```
npm i bosnia-cantons-organization
```

### Import the Package

#### Using require (CommonJS):

```
const data = require('bosnia-cantons-organization');
console.log(data); // This will log the entire JSON data
```

#### Using import (ES Modules):

```
import data from 'bosnia-cantons-organization';
console.log(data); // This will log the entire JSON data
```
