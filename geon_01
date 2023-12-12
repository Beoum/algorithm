class Solution {
    public int solution(int[] bandage, int health, int[][] attacks) {
              int time = attacks[attacks.length-1][0];
      int aCount = 0;
      int sp = 0;
      int cHealth = health;

      for(int i =1; i <= time; i++ ){
          if(i % attacks[aCount][0] == 0){
              cHealth -= attacks[aCount][1];
              aCount++;
              sp = 0;
              if(cHealth <= 0 ){
                  return -1;
              }
          }else {
              sp++;
              cHealth += bandage[1];

              if(bandage[0] == sp ){
                  cHealth += bandage[2];
                  sp = 0;
              }

              if(cHealth > health){
                  cHealth = health;
              }
          }
      }
        return cHealth;
    }
}
