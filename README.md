function positiveSum(arr) {
  var total = 0;    
  for (i = 0; i < arr.length; i++) {    // setup loop to go through array of given length
    if (arr[i] > 0) {                   // if arr[i] is greater than zero
      total += arr[i];                  // add arr[i] to total
    }
  }
  return total;                         // return total
}


//clever one;
function positiveSum(arr) {
 return arr.reduce((a,b) => {return (b > 0) ? (a + b) : (a + 0)}, 0);
  
}