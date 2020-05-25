# snippets-in-js
different type of snippets in js


1. comparing two words in js/javascript.
```
const compare2Words = (word1, word2) => {
    console.log(word1, word2);
    let matches = [];

    let same_letters = 0;
    if(word1.length < word2.length){
        for (let i = 0; i < word1.length; i++) {
            console.log(word1[i]);
            if(word1[i] == word2[i]){
                matches.push({index: i, value: word1[i]});
                same_letters++
            }
        }
    }else{
        for (let i = 0; i < word2.length; i++) {
            console.log(word2[i]);
            if(word1[i] == word2[i]){
                matches.push({index: i, value: word1[i]});
                same_letters++
            }
                
        }
    }
        
    return {
        quantity: same_letters,
        letters: matches
    };

}

let res = compare2Words('where', 'whene');
console.log(res);

```
