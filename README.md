function validParentheses(parens){
  let length = parens.length / 2;
  for(let i = 0; i <= length; ++i){
   parens = parens.replace('()', '');
    }
    return parens == '';
   };
  