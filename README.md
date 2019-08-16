public class Kata {
  public static String declareWinner(Fighter fighter1, Fighter fighter2, String firstAttacker) {
    while(true){
       fighter1.health -= fighter2.damagePerAttack;
       fighter2.health -= fighter1.damagePerAttack;
       
       if(fighter1.health <= 0 && fighter2.health <= 0) return firstAttacker;
       if(fighter1.health <= 0) return fighter2.name; 
       if(fighter2.health <= 0) return fighter1.name; 
       }
  }
}

