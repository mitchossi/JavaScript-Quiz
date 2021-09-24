# JavaScript-Quiz

Klone dieses Repository und beantworte die Fragen gerne direkt  in der readme Datei.  Z. B.:

0. Welchen Wert hat sum?

```
let sum = 5 / 0;
```

*Antwort: infinity*

**Hinweis**: Bitte überlege, was die richtige Antwort ist und probiere den Code **nicht** aus (zumindest am Anfang)! Oder in anderen Worten: Lösung durch Nachdenken und nicht Ausprobieren herausfinden ;) 

## Teil 1

1. Welchen Wert hat y?

```
let x = true;
let y = x ? 1 : 2;
```
Antwort: 1
- - -

2. Welchen Wert hat ```z.length``` ?

```
let z = "hallo";
```
Antwort: 5
- - -
3. Bezogen auf Aufgabe 2: Welchen Wert hat ```z[4]``` ?
Antwort: o

- - -

4. Was ist ```(a===b)``` ?

```
let a = "10";
let b = 10;
```
Antwort: false
- - -

5. Was ergibt ```(e && f)``` ?

```
let e = true;
let f = false;
```
Antwort: false
- - -

6. Was ergibt ```(c || d)``` ?

```
let c = undefined;
let d = 3;
```
Antwort: 3, was von JavaScript als true ausgewertet wird

## Teil 2: 

1. Zu welcher Fehlermeldung führt folgender Code (nicht wortwörtlich, sonder in eigenen Worten)? 

```
let x = 10;
let x = 11;
````
Antwort: so etwas wie: x ist bereits deklariert
- - -

2. Wie kann man den obigen Code ändern, um den Fehler zu beheben?

Antwort:
```
let x = 10;
x = 11;

// oder

let x = 10;
let y = 11;

````

- - -

3. Was ergibt ```(a || b)``` ?

```
let a = undefined;
let b = 3;
```
Antwort: 3
- - -

4. Was ergibt ```(c < d)``` ?

```
let c = 3;
let d = 3;
```
Antwort: false
- - -

5. Was ergibt ```(c <= d)``` ?
Antwort: true
- - -

6. Welche JavaScript-Funktion braucht man, um eine Zufallszahl zwischen 10 und 20 generieren?

Antwort: ```Math.random()``` 
Wir bräuchten aber noch weiteren Code, um tatsächlich eine Zahl zwischen 10 und 20 zu generieren, z.B.:

```
function randomIntFromInterval(min, max) { // min and max included 
  return Math.floor(Math.random() * (max - min + 1) + min)
}
const rndInt = randomIntFromInterval(10, 20)
console.log(rndInt) //Gibt zufällige Zahl zwischen 10 und 20 aus
```

## Teil 3

Markiert die richtigen Antworten mit einem Stern  [ * ]


1. "true" und "false" sind Beispiele von welchem Datentyp?
    
    [ ] Int
    
    [ ] Float
    
    [*] Boolean
    
    [ ] String
    
- - -

2. Die Zahl -100 ist ein von welchem Datentyp?
    
    [*] Int
    
    [ ] Float
    
    [ ] Boolean
    
    [ ] String
    
    - - -

3. Die Zeichenkette "hello world" ist ein von welchem Datentyp?
    
    [ ] Int
    
    [ ] Float
    
    [ ] Boolean
    
    [*] String
    
    - - -
    

4. (true || false) ergibt
    
    [*] true 
    
    [ ] false
    
    - - -

5. (true && false) ergibt
    
    [ ] true 
    
    [*] false
    
    - - -

6. (false && false) ergibt
    
    [ ] true 
    
    [*] false
    
    Hinweis: ```false === false``` ergibt true
    - - -

7. 15%4 ist:
    
    [ ] 0
    
    [*] 3
    
    [ ] 2
    
    - - -

8. 13%2 ist:
    
    [*] 1
    
    [ ] 0
    
    - - -

9. let x = "hello world"; Wie kann ich an den zweiten Buchstaben "e" rankommen?
    
    [*] x[1]
    
    [ ] x[2]
    
    [ ] x[3]
    
    
    
## Teil 4

*Hinweis: Dieser Teil ist ein mix aus Quiz und kleinen Aufgaben*

1. Welche Datentypen hat JavaScript bzw. welche fallen dir ein?

Boolean, String, Number, Object, undefined, null, ...
- - -

2. Ist folgender Code gültig bzw. richtig? 

```const arr = [function(){alert('hello world')}, 0, "bye", undefined]```

2a. Falls nein, warum nicht? // Code ist gültig

2b. Falls ja, wie könntest du die function im Array aufrufen?

```arr[0]()```
- - -

3. Welcher Wert wird die console ausgeben und warum?

```
let myVar = true;
if(myVar) {
 let myString = "hi";
} else {
 let myString = "bye"
}
console.log(myString);
```
Antwort: Es wird kein Wert ausgegeben, da es zu einem Fehler kommt: ```myString is not defined```. Variablen, die mit ```let``` deklaliert wurden, sind nur in einem Block gültig (Stichwort: Scope). Das heißt in dem Fall, nur in dem Body von if, also zwischen { ... }. Mögliche Lösung:

```
let myVar = true;
let myString = null;
if(myVar) {
 myString = "hi";
} else {
 myString = "bye"
}
console.log(myString);
```
- - -

4. Wir haben folgendes Object Literal:
```
let myObj = {
 name: "Wolfgang Petry",
 alter: 72,
 hobbys: ["Call of Duty", "Skateboarden", "Bier"],
 familie: {
   tochter: "Susanne",
   frau: "Brunhilde"
 }
}
```

4a. Wie kann ich auf den Wert von *name* zugreifen?
Antwort: ```myObj.name```

4b. Wie greife ich auf das zweite Hobby *Skateboarden* zu?
Antwort: ```myObj.hobbys[1]```

4c. Wie erhalte ich den Namen der Tochter?
Antwort: ```myObj.familie.tochter```

4d. Mit welche Methode erhalte ich alle keys von myObj in einem Array?
```Òbject.keys(myObj)``` erzeugt folgendes Array: ```['name', 'alter', 'hobbys', 'familie']```

- - -

5. Mit welcher Funktion bzw. wie erhältst du die größte Zahl in einem Array, hier also *10*?

```
const myArr = [5, 3, 1, 6, 10, 0, -100];
```
Antwort: ```Math.max(...myArr)```
Die drei Punkte "..." führen zum "destructering" des Arrays => wir erhalten also alle Werte, die sich im Array befinden. Die Math.max Methode wird dadurch quasi so aufgerufen:

```Math.max(5, 3, 1, 6, 10, 0, -100)```
- - -

6. Was gibt folgender Code aus und warum?
```
var num = "10";
function logNumber () {
 console.log("Original Number " + num);
 var num = "50";
 console.log("New Number " + num);
}
logNumber();
```

Antwort: ```Original Number undefined```
Wir arbeiten hier mit ```var``` und das Thema "hoisting" ist hier entscheidend (gerne google fragen, da nicht mal eben schnell erklärt ;) 
- - -

7. Wie rufst du die function greet auf?

```
function something() {
  
  function greet() {
    console.log("hellor world!");
  }
  
  greet();
}
```

Antwort: ```something();```

Die Funktion greet ist nur in der something Funktion gültig und kann daher nur über sie aufgerufen werden
- - -

8. Wie kannst du das Alter von Hermine auf 45 ändern? Tipp: Du musst zuerst auf das Array-Element und dann auf die Eigenschaft des Objects zugreifen. Du brauchst also "[]" und "."

```
const someArr = [
  {
    name: "Alina",
    alter: 25
  },
  {
    name: "Tareq",
    alter: 35
  },
  {
    name: "Hermine",
    alter: 42
  }
];
```

Antwort: ```someArr[2].alter = 45;```
- - -

9. Wie kannst du folgendes Array kopieren und noch die Zahl 5 an den Anfang hinzufügen?

```
const someArr = [4,7,8,1,2];
const newArray = //... In diesem Array sollen alle zahlen aus someArr und die zusätzliche 5 stehen
```

Eine mögliche Antwort/Lösung: ```const newArray=[5, ...someArr];```

- - -

10. Was gibt folgender Code aus?

```
let i = 5;
i += 5; 
console.log(i);
```

Antwort: 10

Wie könntest du die Zeile ```i += 5; ``` noch schreiben?

Antwort: ```i = i + 5;```
- - -

11. Welche Möglichkeiten kennst du, um ein array zu durchlaufen? Verwende unterschiedliche Varianten, um jedes Element des nachfolgenden Arrays in der Console auszugeben auszugeben:

```
const countries = ["Afghanistan","Albania","Algeria","Andorra","Angola","Anguilla","Antigua &amp; Barbuda","Argentina","Armenia","Aruba","Australia","Austria","Azerbaijan","Bahamas","Bahrain","Bangladesh","Barbados","Belarus","Belgium","Belize","Benin","Bermuda","Bhutan","Bolivia"];
```

Antwort:
```
countries.forEach(el=>{
  console.log(el)
})

for(let country of countries) {
    console.log(country);

}

for(let i=0; i<countries.length; i++) {
  console.log(countries[i]);
}

// würde man so nicht machen
for(let i in countries) {
    console.log(countries[i]);
}
// es gibt sicherlich noch andere Varianten, wie z.B. mit while
```
- - -

12. Gegeben ist folgendes Object:

```
const auto = {
  baujahr: 1985,
  marke: "MBW"
}
```

12a. Kannst du dem Object noch nachträglich den key "inhaber" mit dem Wert "Jan Tenner" zuordnen? Falls nein, warum? Falls ja, wie?

Antwort: ```auto.inhaber = "Jan Tenner";```

12b. Kannst du den key "marke" nachträglich entfernen? Wenn ja, wie?
Antwort: ```delete auto.marke```

12c. Erstelle eine Kopie des Objects in eine neue Variable und füge gleichzeitig zwei neue key/value Paare hinzu: ```farbe: rot, zugelassen: true```

Antwort: 
```
const objCopy = {
  ...auto,
  farbe: "rot",
  zugelassen: true
};
```


- - -

13.   Was wird hier die Console ausgeben und warum?

```
const arrOriginal = [1,2,3,4,5];
const arrTwo = arrOriginal;
arrTwo[0] = 1000;

console.log(arrOriginal);
console.log(arrTwo);
```

Antwort/Ausgabe:
```
[1000, 2, 3, 4, 5]
[1000, 2, 3, 4, 5]
```
Es wird also zwei mal dasselbe Array ausgegeben. ```const arrTwo = arrOriginal; ``` erzeugt nämlich keine Kopie vom arrOriginal, sondern weißt arrTwo das selbe array zu, auf das auch arrOriginal "zeigt" bzw. "referiert" (also auf [1,2,3,4,5]). Stichwort: reference type


- - -


14.  Nutze die map Function, um ein neues Array zu erstellen, das den String "Hallo " vor jedes Element des nachfolgenden Arrays schreibt:

```
const namesArray = ["Beate", "Julia", "Enis", "Silvia"];
// Neues Array soll wie folgt aussehen: 
// ["Hallo Beate", "Hallo Julia", "Hallo Enis", "Hallo Silvia"]
```
Antwort:
```
const newArr = namesArray.map(el => {
    return "Hallo " + el;
})
```

14a. Gibt es noch andere Möglichkeiten, ohne map?

Antwort: Klar, wir könnten das Array mit einer For-Schleife durchlaufen und die modifizierten Werte jeweils mittels ```push()``` in ein neues Array hinzufügen

14b. Erzeuge mittels filter ein array, dass nur Namen aus *namesArray* enthält, die jeweils den Buchstaben e bzw. E (also groß oder klein) enthalten. In diesem Fall wäre es also: ```["Beate", "Enis"]```

Antwort:

```
const newArrFiltered = namesArray.filter(el => {
    return el.toLowerCase().includes('e');
})
```

14c. Schreibe eine Funktion, die die Namen in einem Array umkehrt und diese als neues Array zurückgibt.

```
function namesReverser(arr) {
  //...
  const reversedArr = //...

  return reversedArr;
}
```

Antwort:
```
function namesReverser(arr) {
  const reversedArr = arr.map(el =>{
        let stringArr= el.split("")
        let reversedStringArr = stringArr.reverse();
        return reversedStringArr.join(""); // wieder zu String umgewandelt
  });

  return reversedArr;
}

console.log( namesReverser(namesArray) ); // => ['etaeB', 'ailuJ', 'sinE', 'aivliS']
```

- - -


## Bonus: weitere Fragen zu JavaScript
* https://www.tutorialsteacher.com/online-test/javascript-test1 
* https://www.dotnettricks.com/learn/javascript/javascript-interview-questions
