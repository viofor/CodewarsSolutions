function playerManager(players) {
  if(players === null || players.length === 0){
    return [];
  }
    let arr = players.split(', ');
    let res = [];
    for(let i = 0; i < arr.length; i += 2){
     let obj = {
      player: arr[i],
      contact: +arr[i+1]
    };
     res.push(obj);
    }
  return res;
}
