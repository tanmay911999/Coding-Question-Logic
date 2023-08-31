# Coding-Question-Logic
1) String Introduction Problem
Input Format

The first line contains a string . The second line contains another string . The strings are comprised of only lowercase English letters.

Output Format

There are three lines of output:
For the first line, sum the lengths of  and .
For the second line, write Yes if  is lexicographically greater than  otherwise print No instead.
For the third line, capitalize the first letter in both  and  and print them on a single line, separated by a space.

-> 
int len = A.length()+B.length(); // Some of String length
    System.out.println(len); 
    if(A.compareTo(B)>0){  // comparision.
        System.out.println("Yes");
    }        
    else{
        System.out.println("No");
    }
    // Creating some substrings for capitalize first letter
    String str1 = A.substring(0,1);  
    str1= str1.toUpperCase();

    String str2 = B.substring(0,1);
    str2= str2.toUpperCase();
    // Solution
    System.out.println(str1+A.substring(1,A.length())+" "+str2+B.substring(1,B.length()));
