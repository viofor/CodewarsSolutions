function spongeMeme(sentence){
let str = '';
  for(let i = 0; i < sentence.length; i++){
   if(i % 2 == 0){str += sentence[i].toUpperCase();
    }else{ str += sentence[i].toLowerCase(); 
    }
   }
    return str
  };