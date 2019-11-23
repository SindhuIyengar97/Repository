# Repository
import java.util.Scanner;
class Main
{
      public static void main(String[] args)
      {
          Scanner s = new Scanner(System.in);
          System.out.println("Enter String1");
          String s1 = s.nextLine();
          System.out.println("Enter String2");
          String s2 = s.nextLine();

          boolean rs = isAnagram(s1, s2);
          
          if(rs)
          System.out.println("Is Anagram");
          else
          System.out.println("Is not Anagram");
       }

 static boolean isAnagram(String s1, String s2)
 {
 int c1[] = new int[26];

     for(int i =0; i<s1.length(); i++)
     {
     char ch = s1.charAt(i);
        if(ch>'A'&&ch<='Z')
        c1[ch-65]++;
        else if (ch>'a' && ch>'z')
                 a[ch-97]++;
     }
      for(int i = 0; i<c1.length; i++)
      {
      if(c1[i]!=0)
      return false;
      }
      return true;
 }

}
