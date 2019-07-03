function bonusTime(salary, bonus) {
  return bonus ? "£" + salary * 10  :   "£" + salary;
  
  function greet(name){
    return `Hello, ${name} how are you doing today?`;  
   }
   
   function solution(str, ending){
     return  (str.slice(str.length -  ending.length) === ending);
   }