function add(n){
  let f = function(x) {return add(n+x);};
  f.toString = function() {return n; };
  return f;
}
function calculate(num1,num2){
  let n1 = 0, n2 = 0;
  for(let i in num1)
   n1 += num1[i] == '1' ? Math.pow(2, num1.length-1-i) : 0;
  for(let i in num2)
   n2 += num2[i] == '1' ? Math.pow(2, num2.length-1-i) : 0;
  return n1 + n2;

}

  const _ = undefined
  const pad = [
   ['1','2','3'],
   ['4','5','6'],
   ['7','8','9'],
   [ _ ,'0', _ ]
  ]
  const keys = observed.split('').map(o => getSiblingKeys(o.toString(), pad))
  const results = cartesian(keys).map(arr => arr.join(''))
  
  return results
  
  function getSiblingKeys(n, pad) {
    const e = []
    const y = pad.findIndex(arr => arr.indexOf(n) != -1)
    const x = pad[y].indexOf(n)

    e.push(n)
    if (y > 0) e.push(pad[y-1][x])
    if (y < 2 || n == '8') e.push(pad[y+1][x])
    if (x > 0 && n != '0') e.push(pad[y][x-1])
    if (x < 2 && n != '0') e.push(pad[y][x+1])
    
    return e
  }

  function cartesian(arr) {
    return arr.reduce((a,b) => (
      a.map((x) =>
        b.map((y) =>
          x.concat(y)
        )
      ).reduce((a,b) => (
        a.concat(b)
      ), [])
    ), [[]])
  }
}

var buy = function(x, arr){
  let res = [];
  for(let i = 0; i < arr.length - 1; i++){
    for(let j = i + 1; j < arr.length; j++){
      if(arr[i] + arr[j] === x){
     return [i,j];
     }
    }
  }
  return null;
};


function maxTriSum(numbers){
let sum = 0;
  let res = numbers.sort((a,b) => b - a);
  let arr = [];
  for(let i = 0; i < res.length; i++){
      if(arr.length >= 3){
      break
  }
  if(!arr.includes(res[i])){
    arr.push(res[i]);
    sum += res[i];
    }
  }
 return sum;
}


function findMissing(arr1, arr2) {
  let misEl;
  let a1 = arr1.sort((a,b) => a - b);
  let a2 = arr2.sort((a,b) => a - b);
  
  for(let i = 0; i < a1.length; i++){
   if(a1[i] !== a2[i]) return a1[i];
  }
}