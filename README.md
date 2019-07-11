function search(budget, prices) {
 return prices.filter((el) => el <= budget).sort((a,b)=> a-b).join()
   
}