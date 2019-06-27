function chromosomeCheck(sperm) {
if(sperm === 'XY'){
  return "Congratulations! You're going to have a son.";
  }else(sperm === 'XX')
  return "Congratulations! You're going to have a daughter."
}
console.log (chromosomeCheck('XX')); 