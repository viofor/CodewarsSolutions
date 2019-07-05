function add(n){
  let f = function(x) {return add(n+x);};
  f.toString = function() {return n; };
  return f;
}