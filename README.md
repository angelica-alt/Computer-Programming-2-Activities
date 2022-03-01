class Main{  

  //1.Counting duplicate characters.Write a

 //program that counts duplicate characters from a given string.

  public static void main(String args[]){  

     String string1 = "Good Friday";  

        int count;  

          

        char string[] = string1.toCharArray();  

          

        System.out.println("Duplicate characters in a given string: ");   

        for(int o = 0; o <string.length; o++) {  

            count = 1;  

            for(int c = o+1; c <string.length; c++) {  

                if(string[o] == string[c] && string[c] != ' ') {  

                    count++;    

                    string[c] = '0';  

                }  

            }   

            if(count > 1 && string[o] != '0')  

                System.out.println(string[o]);  

        }  

    }  

}  
 javac -cp . Main.java

+ java -cp . Main

Duplicate characters in a given string: 
import java.util.Arrays;

class Main {

  public static void main(String[] args) {

    String str1 = "listen";

    String str2 = "silent";

    

    str1 = str1.toLowerCase();

    str2 = str2.toLowerCase();

    if(str1.length() == str2.length()) {

      char[] charArray1 = str1.toCharArray();

      char[] charArray2 = str2.toCharArray();

      Arrays.sort(charArray1);

      Arrays.sort(charArray2);

      boolean result = Arrays.equals(charArray1, charArray2);

      if(result) {

        System.out.println(str1 + " and " + str2 + " are anagram.");

      }

      else {

        System.out.println(str1 + " and " + str2 + " are not anagram.");

      }

    }

    else {

      System.out.println(str1 + " and " + str2 + " are not anagram.");

    }

  }

}

o





