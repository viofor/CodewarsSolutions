function playerManager(players) {
if(players === '' || players === null){
  return [];
}
  let arr = players.split(', ');
  let arr2 = [];

  for(let i = 0; i < arr.length; i+=2){
    let obj = {
      player: arr[i],
      contact: +arr[i+1]
    }
  arr2.push(obj);
  }
  return arr2;
}