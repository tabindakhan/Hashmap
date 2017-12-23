# Hashmap
import java.util.HashMap;
import java.util.Scanner;

/**
 *
 * @author Tabinda Khan
 */
public class Hashmaps {
    public static void main(String[] args) {
        int i;
        int index = 7;
        HashMap<Integer,Integer> hash= new HashMap<>();
        Scanner s = new Scanner(System.in);
        for(i=0;i<=index;i++){
            System.out.println("Enter Values!" +i);
            int value = s.nextInt();
            int keys = value%index;
            while(hash.get(keys)!=null){
                 keys=keys+1;
            }    
            hash.put(keys, value);       
        }   
      System.out.println(hash);      
       int a ;
     System.out.println("Enter the keys: ");
          a = s.nextInt();
           int result =  hash.get(a);
       System.out.println("Key"+"      "+"Value");
      System.out.println(a+"     "+result);
}
}  
