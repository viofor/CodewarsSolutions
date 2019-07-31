const sumAverage = (arr) => {
  let result = 0;
  for(let i = 0; i < arr.length; i++){
    let sum = 0;
    for(let j = 0; j < arr[i].length; j++){
     sum += arr[i][j];
    }
    result += sum/arr[i].length;
  }
  return Math.floor(result);
}


short one ; const sumAverage = (arr) => {
              let result;
              return Math.floor(arr.map(e => e.reduce((a,c) => a + c , 0)/e.length).reduce((a,c) => a + c , 0));