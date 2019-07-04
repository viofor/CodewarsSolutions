function noSpace(x){
 let str = x.replace(/ /g,'');
 return str;  
}



function dirReduc(arr){
  let newDir = [];
   arr.map(direction => {
   switch(direction.toUpperCase()){
    case 'NORTH':
      if(newDir[newDir.length-1]==='SOUTH') newDir.pop('SOUTH')
       else newDir.push('NORTH')
        break
    case 'SOUTH':
      if(newDir[newDir.length-1]==='NORTH') newDir.pop('NORTH')
       else newDir.push('SOUTH')
        break
    case 'WEST':
      if(newDir[newDir.length-1]==='EAST') newDir.pop('EAST')
       else newDir.push('WEST')
        break
    case 'EAST':
      if(newDir[newDir.length-1]==='WEST') newDir.pop('WEST')
       else newDir.push('EAST')
        break
    }
   })
   return newDir;
}