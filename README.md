function solve(arr){
 let alp = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ';
 let nArr = [];
 for(let i = 0; i < arr.length; i++){
   let count = 0
   for(let j = 0; j < arr[i].length; j++){
    if( j === alp.indexOf(arr[i][j].toUpperCase())){
      count++
     }
    }
   nArr.push(count)
  }
return nArr
};