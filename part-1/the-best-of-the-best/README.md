# De bästa av de bästa

- C-nivå
- [GitBook](https://coursepress.gitbooks.io/1dv021/content/ovningsuppgifter/del1/de-basta-av-de-basta/)

>__VIKTIGT!__ Innan du börjar arbeta med övningsuppgiften är det viktigt att du följer guiden [Att komma igång med en övningsuppgift](https://coursepress.gitbooks.io/1dv021/content/guider/att-komma-igang-med-en-ovningsuppgift/) för att lägga till övningsuppgiftens repo till ditt repo för övningsuppgifter.

Hämta hem övningsuppgiftens repo och lägg tillen .gitignore-fil. Öppna filen `winner.js` och komplettera funktionerna `getFrequencyInArray`, `getHighestValueInFrequency` och `sortStringAscending`.

I denna uppgift finns fyra funktioner varav du ska komplettera tre av dem. Den fjärde är tänkt att i slutändan anropa de tre tidigare för att få ett slutresultat.

Bland kursledarna finns en återkommande tävling där vinnarens namn i varje omgång läggs in i en array.

```js
// Exempel
['mats', 'John', 'john', 'Johan', 'Jacob']
```

Själva applikationen går ut på att utifrån en liknande array avgöra antalet förekomster av varje namn, sedan sortera dessa i storleksordning (den med flest förekomster först) avgöra vinnaren/vinnarna och presentera dessas namn i en array som sorterats i bokstavsordning.

För att lösa detta problem används alltså fyra olika funktioner, varav tre behöver kompletteras.

## Funktioner

### getFrequencyInArray

Funktionen analyserar en array och försöker avgöra förekomsten av namnen (_"case-insensitiv"_ - d.v.s. stor eller liten bokstav i början av namnet ska inte spela roll). Resultatet ska vara på en viss form vilket framgår av kommentarerna i koden. Uppbyggnaden av objekten kan vara lite konstig då namnen används som nyckel. Det är dock för att förenkla programmeringen i uppgiften då det handlar om hantering av en frekvenstabell.

```js
let obj = winner.getFrequencyInArray(['mats', 'John', 'john', 'Johan', 'Jacob'])

// obj should be
/*
{
mats: 1,
john: 2,
johan:1,
jacob: 1
}
*/
```

### getHighestValueInFrequency

Funktionen tar ett objekt i samma form som funktionen `getFrequencyInArray` returnerar, sorterar denna och returnerar en array innehållande de namn som förekommer flest gånger.

```js
let obj = {
mats: 1,
john: 2,
johan: 1,
jacob: 1
}

let arr = winner.getHighestValueInFrequency(obj)
// arr should be ["john"]
```

### sortStringAscending

Tar en array med textsträngar och sorterar i stigande ordning.

```js
let arr = winner.sortStringAscending(['john', 'johan', 'jacob'])
// arr should be ['jacob', 'johan', "john']
```

### getWinner

Denna är färdigskriven och bör fungera och ge gröna tester när du väl implementerat
de tre funktionerna ovan.

## Tips

Genom att köra testerna som kommer med övningsuppgiften kan du undersöka om koden du skrivit löst uppgiften (i alla fall enligt testet...).

Funktioner, metoder, etc. som _kan_ komma till användning beroende hur du väljer att lösa uppgiften.

- [String.toLowerCase](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/toLowerCase)
- [Object.keys](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/keys)
- [Array.sort](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)
- [Array.filter](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)

## Lösningsförslag

- [https://github.com/1dv021/exercise-solution-proposals/tree/master/part-1/the-best-of-the-best](https://github.com/1dv021/exercise-solution-proposals/tree/master/part-1/the-best-of-the-best)
