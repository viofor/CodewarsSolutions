function mergeArrays(arr1, arr2) {
  let newArr = [];
   for(let i = 0; i < arr1.length; i++){
    if(!newArr.includes(arr1[i]))
    newArr.push(arr1[i]);
  }
    for(let i = 0; i < arr2.length; i++){
    if(!newArr.includes(arr2[i]))
     newArr.push(arr2[i]); 
  }
  return newArr.sort((a,b) => a-b);
}