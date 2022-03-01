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

o

dhttps://github.com/charlottegeronimo/charlottegeronimo/new/main?readme=1



