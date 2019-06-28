function sumR(x){
  if(x.length === 0){
   return 0;
  }else {
  return  x.shift() + sumR(x);
  }
}
  