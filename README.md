function randomCase(x){
let str = '';
  for(let i = 0; i < x.length; i++){
   if(Math.round(Math.random()) > 0){
   str += x[i].toUpperCase();
   }
   else{
   str += x[i].toLowerCase();
    }
   }
   return str
}; 