function reverseNumber(n) {
  if( n >= 0){
  let arr = n.toString().split('').reverse();
  return +(arr.join(''));
  }else{
  n = n * (-1);
  let arr = n.toString().split('').reverse();
  return (-1) * (+(arr.join('')));
  }
}