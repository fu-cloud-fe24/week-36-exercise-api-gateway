# Vecka 36 : Övning API Gateway

## Shakespearean Insults API

Använd nedanstående förolämpningar från Shakespeares olika pjäser och skapa ett API där man kan:

* Hämta alla insults
* Hämta en specifik insult med hjälp av en ID-parameter (**inte** query parameter)
* Lägga till en ny insult
* Ersätta en insult med en annan
* Ta bort en insult

Varje ovanstående anrop skall bestå av en egen lambdafunktion, som triggas utav ett HTTPApi från API Gateway.

### Levelup!

* Med hjälp av queryparametern *search* kan man leta upp alla insults som innehåller en viss textsträng
* Med hjälp av queryparametern *play* kan man hitta alla insults som ingår i en specifik pjäs

### Insults

```
const insults = [
  {
    id: 1,
    insult: "Peace! I will not endure thy lies.",
    play: "Much Ado About Nothing"
  },
  {
    id: 2,
    insult: "Thy tongue outvenoms all the worms of Nile.",
    play: "Cymbeline"
  },
  {
    id: 3,
    insult: "Thou crusty batch of nature!",
    play: "Troilus and Cressida"
  },
  {
    id: 4,
    insult: "Thou art a boil, a plague sore!",
    play: "King Lear"
  },
  {
    id: 5,
    insult: "Away, you three-inch fool!",
    play: "Taming of the Shrew"
  },
  {
    id: 6,
    insult: "Thou poisonous bunch-backed toad!",
    play: "Richard III"
  }
];
```
