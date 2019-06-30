function simpleMultiplication(n){
  if(n % 2) {
   return n * 9;
   }else
  return n * 8;
  }
  
  function getRectangleString(w, h) {
    const rn = '\r\n';
    const tb = '*'.repeat(w) + rn;
    const center = (w > 1) ? ('*' + ' '.repeat(w - 2) + '*' + rn).repeat(h - 2) : '';
    return  h > 1 ? (tb + center + tb) : tb.repeat(h);
  }