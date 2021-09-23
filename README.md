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


2. Welchen Wert hat ```z.length``` ?

```
let z = "hallo";
```

3. Bezogen auf Aufgabe 2: Welchen Wert hat ```z[4]``` ?

4. Was ist ```(a===b)``` ?

```
let a = "10";
let b = 10;
```

5. Was ergibt ```(e && f)``` ?

```
let e = true;
let f = false;
```

6. Was ergibt ```(c || d)``` ?

```
let c = undefined;
let d = 3;
```

## Teil 2: 

1. Zu welcher Fehlermeldung führt folgender Code (nicht wortwörtlich, sonder in eigenen Worten)? 

```
let x = 10;
let x = 11;
````


2. Wie kann man den obigen Code ändern, um den Fehler zu beheben?


3. Was ergibt ```(a || b)``` ?

```
let a = undefined;
let b = 3;
```


4. Was ergibt ```(c < d)``` ?

```
let c = 3;
let d = 3;
```


5. Was ergibt ```(c <= d)``` ?


6. Welche JavaScript-Funktion braucht man, um eine Zufallszahl zwischen 10 und 20 generieren?

## Teil 3

Markiert die richtigen Antworten mit einem Stern  [ * ]


1. "true" und "false" sind Beispiele von welchem Datentyp?
    
    [ ] Int
    
    [ ] Float
    
    [ ] Boolean
    
    [ ] String

2. Die Zahl -100 ist ein von welchem Datentyp?
    
    [ ] Int
    
    [ ] Float
    
    [ ] Boolean
    
    [ ] String

3. Die Zeichenkette "hello world" ist ein von welchem Datentyp?
    
    [ ] Int
    
    [ ] Float
    
    [ ] Boolean
    
    [ ] String

4. (true || false) ergibt
    
    [ ] true 
    
    [ ] false

5. (true && false) ergibt
    
    [ ] true 
    
    [ ] false

6. (false && false) ergibt
    
    [ ] true 
    
    [ ] false

7. 15%4 ist:
    
    [ ] 0
    
    [ ] 3
    
    [ ] 2

8. 13%2 ist:
    
    [ ] 1
    
    [ ] 0

9. let x = "hello world"; Wie kann ich an den zweiten Buchstaben "e" rankommen?
    
    [ ] x[1]
    
    [ ] x[2]
    
    [ ] x[3]
    
    
    
## Teil 4

1. Welche Datentypen hat JavaScript bzw. welche fallen dir ein?

2. Ist folgender Code gültig bzw. richtig? 

```const arr = [function(){alert('hello world')}, 0, "bye", undefined]```

a. Falls nein, warum nicht?
b. Falls ja, wie könntest du die function im Array aufrufen?

3. Welche Wert wird die console ausgeben und warum?

```let myVar = true;
if(myVar) {
 let myString = "hi";
} else {
 let myString = "bye"
}```
console.log(myString)

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

a. Wie kann ich auf den Wert von *name* zugreifen?
b. Wie greife ich auf das zweite Hobby *Skateboarden* zu?
c. Wie erhalte ich den Namen der Tochter?

d. Mit welche Methode erhalte ich alle keys von myObj in einem Array?

5. Mit welcher Funktion bzw. wie erhältst du die größte Zahl in einem Array, hier also *10*?

```
const myArr = [5, 3, 1, 6, 10, 0, -100];
```
