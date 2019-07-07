function arraysSimilar(arr1, arr2) {
  return JSON.stringify(arr1.sort()) === JSON.stringify(arr2.sort());
}

// just a small amount of possible functions to start testing with.
var addOne = function(e) {return e + 1;};
var square = function(e) {return e * e;};

// Extend the Function prototype with a method pipe
Function.prototype.pipe = function(f){
  return function(ff) {
    return f(this(ff));
  }.bind(this);
}


function going(n) {
  let d = 1;
  let res = 1;
   for(let i = n; i > 1; i--){
   d *= i;
   res += 1 / d;
   }
   return Math.floor(res * 1e6) / 1e6;
};

let palindromeChainLength = n => {

    let reverNum = n => Array.from(n.toString()).reverse().join('')
    let isPalindrome = n => reverNum(n) === n.toString()

    let steps = 0
    while (!isPalindrome(n)) {
        steps++
        n += parseInt(reverNum(n))
    }
    return steps
};


function duplicateCount(text){
   let duplCnt = 0, counts = []

    Array.from(text.toLowerCase()).map(x => counts[x] = (counts[x] || 0) + 1)

    for (let c in counts) {
        if (counts[c] > 1) {
            duplCnt++
        }
    }

    return duplCnt
}