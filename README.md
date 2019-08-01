let number = function(busStops){
  return busStops.reduce((a, [b,c])=>{
    return a + b - c;
  },0)  
}