# JS grundläggande övningar

## Syntax n stuff
### Datatyper
**1** Vilka datatyper finns det i JS? Svara i form av en array.

```javascript
let datatypes = []
```

**2** Är följande if sats *true* eller *false*?

```javascript
let a = 1;
let b = '1';
if(a == b) // true or false
```

**3** Vad är den *tekniska* skillnaden ( förutom var, let ) på dessa två deklarationer?

```javascript
let name = 'Greta Thunberg';
var name = 'Greta Thunberg';
```

**4.** Hur tar man reda på vad en variabel har för datatyp?

### Block 

**5** Vilken av följande tecken visar ett ```kodblock```?

```javascript
[] // A 
() // B
{} // C
```

**6** Vad i följande kod är ```blocket``` som *exekveras*?

```javascript
el.on('click', () => {
    alert('Ariba!');
})
```

**7**
Vad kommer stå i ```console.log()```?

```javascript
var greeting = 'Good bye world!';

{
    let greeting = 'Hello World';
}

console.log(greeting);
```

### Strings

**8** Vilken av följande syntax är korrekt sätt att skriva strängar.

```javascript
"Hello World" // A
'Hello World' // B
`Hello World` // C
```

**9** Räkna antal tecken i strängen nedan.

    let sentence = "If you're having code problems I feel bad for you son. I got 99 problems, but a glitch ain't one."

**10** Gör en *template string* där ```N``` ersätts med variabeln ```name```.

```javascript
let name = '<Ditt namn>' 
`Hej N din gamle knasboll!`
```

### Arrays

**11** Gör en array med 5 frukter i.

**12** Lägg till en frukt *i början* och en frukt *i slutet* på arrayen.

**13**
I ovanstående fruktarray, plocka bort *första* och *sista* frukten.

**14** I följande array, sätt in två nya frukter på *index 2*.

```javascript
let fruits = ['apple', 'orange', 'pear', 'kiwi']
```

**15** Klona följande array och ändra första frukten till ```pineapple```.

```javascript
let fruits = ['apple', 'orange', 'pear', 'kiwi']
```

**16** Sortera följande array i *fallande ordning*.

```javascript
let num = [1,5,78,7,122,3,4,65,40,2,8]
```

**17** Lägg ihop följande arrayer.

```javascript
let a = [1,2,3];
let b = [4,5,6];
```

**18** Mixa följande arrayer där varannan är från array ```a``` och varanan från array ```b```.

```javascript
let a = ['My', 'has', 'many', 'open'];
let b = ['brain', 'to', 'tabs', '!'];
```

**19** Merga in array ```a``` i array ```b``` på *index 2*. 

```javascript
let a = [1,2,7,8,9,10];
let b = [3,4,5,6];
```

**20** Gör alla namn i array ```names``` till *versaler*.

```javascript
let names = ['sixten', 'Eva', 'Ali', 'Kim', 'Greger', 'Alicia'];
```

**22** Skriv koden för att undersöka om arrayen ```names``` innehåller namnet *Ewa*. Ditt svar ska vara ```true``` eller ```false```.

```javascript
let names = ['sixten', 'Eva', 'Ali', 'Kim', 'Greger', 'Alicia'];
```

### Objects
**28** Skapa en ett objekt som heter ```book``` och som har egenskaperna *title*, *author* och *genres*. De två första egenskaperna ska vara strängar och den sista en array.

**29** ```console.log()``` endast egenskapen *city* i följande objekt.

```javascript
let person = {
    name: 'Sixten Faceplant',
    email: 'sixten.faceplant@zocom.se',
    role: 'ninjah',
    adress: {
        street: 'Karatevägen 3',
        zip: '41477',
        city: 'Kablam City'
    }
}
```

**30** Klona ett objekt.

**31** Skapa objektet ```dog``` med egenskaperna *name*, *breed* och metoden *bark* som ska returnera "Woff, jag heter ```N```!" där ```N``` ska ersättas med egenskapen *name* i samma objekt.

### Functions 
**33** Skriv en funktion som *adderar* två numeriska argument (```x``` och ```y``` ) och returnerar.

**34** Skriv en *anonym funktion* som returnerar en ```sträng``` som förklarar skillnaden på *namnade-* och *anonyma* funktioner.

**35** Skriv en funktion som *plockar ut året* från en sträng i datumformat. Funktionen ska ta ett argument, som ska vara en sträng. Strängen ska alltid ha 10 tecken och följa mönstret 'YYYY-MM-DD'.

```javascript
getYear('2019-10-14') // 2019
```

<details>
    <summary>hint</summary>
    Använd substring(startIndex, endIndex).
</details>


**36** Skriv en funktion som tar tre parametrar. De första två är två tal och den sista är en *aritmetisk operator* d.v.s antingen '+', '-', '/', '*'.

```javascript
calcThis(1,2,'+') // 3
```

### Conditionals

**37** Skriv en funktion som jämför om två tal är likadana och returnerar true / false.

```javascript
compareThis(1,1) // true
campareThis(3,1) // false
```

**38** Skriv en funktion som kollar om ett tal är mellan *20* och *40* och returnerar true / false.

```javascript
between(30) // true
between(50) // false
```

**39** Skriv en funktion som jämför *längden* på två arrayer och returnerar den längsta.

```javascript
getMeTheLongestArr([1,2], ['A','B','C']) // ['A','B','C']
```


### Math object
**40** Avrunda talet ```1337.51``` *nedåt* till närmaste heltal med hjälp av *Math object*.

**41** Avrunda talet ```1337.48``` *uppåt* till närmaste heltal med hjälp av *Math object*.

**42** Avrunda talet ```1337.497``` *till närmaste heltal* med hjälp av *Math object*.

**43** Skriv en funktion ( ```random(max)``` ) som tar ett *numerisk argument* ( ```max``` ). Funktionen ska returnera ett slumpat tal mellan 0 och *argumentet*.

```javascript
random(10000) // 1337
```

**44** Skriv en funktion ( ```randomPassword(n)``` ) som tar ett numerisk argument ( ```n``` ). Funktionen ska returnera ett slumpat lösenord bestående av bokstäver och siffor med längden *n*.

```javascript
randomPassword(7) // 4w3s0m3
```

**45** Skriv en funktion ( ```randomName(names)``` ) som tar en array som argument ( ```names``` ). Funktionen ska returnera ett slumpat namn från arrayen.

```javascript
const names = ['sixten', 'Eva', 'Ali', 'Kim', 'Greger', 'Alicia']

randomName(names) // Greger
```

### Program flow
**46** Vad är skillnaden på följande två funktioner?

```javascript
let getData = function(url) {};
function getData() {};
```

**47** I vilken ordning kommer följande funktioner att exekveras?

```javascript
// Execute
HelloAgainAgain();

function hello(){  
    console.log('Hello!') 
};

function helloAgain(){
    console.log('Hello Again!') 
    hello();
};

function HelloAgainAgain(){
    console.log('Hello Again Again!') 
    helloAgain();
}
```

**48** Ordna programmet i rätt ordning så alla pokemons printas ut. All kod som behövs finns med.

```javascript

for(let i=0;i<=pokemons.length;i++) {}

function printPokemons() {}

console.log("One awesome pokemon is " + pokemons[i]);

printPokemons();

let pokemons = ['Pikachu', "Charmander", "Bulbasaur", "Squirtle"];
```

**49** Ordna programmet i rätt ordning så att det går att skicka in en sträng och få tillbaka den baklänges.

```javascript
return newString;
let i = str.length - 1; i >= 0; i--
reverseString('hello');
str
function reverseString() {}
let newString = '';
for () {}
newString += str[i];
```
