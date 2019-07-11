function averageString(str) {
 let arr = ['zero', 'one', 'two', 'three', 'four', 'five', 'six', 'seven', 'eight', 'nine']
  let arrStr = str.split(' ');
  let sum = 0;
  for(let i = 0; i < arrStr.length; i++){
    sum += arr.indexOf(arrStr[i]);
    if(arrStr[i] === '' || !arr.includes(arrStr[i])) return 'n/a';
  }
  let avg = Math.floor(sum/arrStr.length);
    return arr[avg];
}