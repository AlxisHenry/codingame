# Règles

Écrivez le programme permettant de détruire les montagnes pour pouvoir attérir. Pour cela, tirez sur la montagne la plus haute.

Au début de chaque tour de jeu, vous recevez en entrée la hauteur de chaque montagne de gauche à droite.
Avant la fin du tour de jeu, vous devez indiquer la montagne la plus haute pour tirer dessus.

Tirer sur une montagne ne fera qu'en détruire une partie. Votre vaisseau descend à chaque passe.

# Solution

```js
while (true) {
    let arr = []
    for (let i = 0; i < 8; i++) {
        arr.push(parseInt(readline()))
    }
    console.log(arr.indexOf(Math.max(...arr)))
}
```
