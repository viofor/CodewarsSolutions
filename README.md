function isPangram(string){
  let abc = "abcdefghijklmnopqrstuvwxyz";
   let arr = string.split('');
   for(let i = 0; i < arr.length; i++){
    let elem = arr[i].toLowerCase()
     abc = abc.replace(elem,"")
     }
     if(abc.length === 0){
     return true
     } else {
     return false
    }
};
  