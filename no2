#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#define MAX 50
int top = -1, front = 0;
int stack[MAX];
void push(char);
void pop();
void main()
{
 int i, choice;
 char s[MAX], b;
 while (1)
 {
 printf("1-enter string\n2-exit\n");
 printf("enter your choice\n");
 scanf("%d", &choice);
 switch (choice)
 {
 case 1:
 printf("Enter the String\n");
 scanf("%s", s);
 for (i = 0;s[i] != '\0';i++)
 {
 b = s[i];
 push(b);
 }
 for (i = 0;i < (strlen(s) / 2);i++)
 {
 if (stack[top] == stack[front])
 {
 pop();
front++;
 }
 else
 {
 printf("%s is not a palindrome\n", s);
 break;
 }
 }
 if ((strlen(s) / 2) = = front)
 printf("%s is palindrome\n", s);
 front = 0;
 top = -1;
 break;
 case 2:
 exit(0);
 default:
 printf("enter correct choice\n");
 }
 }
}
/* to push a character into stack */
void push(char a)
{
 top++;
 stack[top] = a;
}
/* to delete an element in stack */
void pop()
{
 top--;
}
/*
* Java Program to Identify whether the String is Palindrome or not using Stack
*/
import java.util.*;
//with explanations.
public class palindorme{
public static void main(String[] args){
Scanner uin = new Scanner(System.in);
//creating the stacks for the string
Stack str1 = new Stack();
Stack revStr = new Stack(); //to hold the reverse string
System.out.print("What's your test word: ");
String str = uin.next().toLowerCase(); //input the string
char[] mainStr = str.toCharArray(); //splitting the given string to individual
characters.
//pushing the characters of the given string to the first stack.
for(int i = 0; i < mainStr.length; i++){
str1.push(mainStr[i]);
}
//pushing the reverse of the string to another stack
for(int j = 0; j < mainStr.length; j++){
revStr.push(mainStr[(mainStr.length - 1) - j]);
}
//popping the items in the original stack and comparing with the reversed stack (as
long as the stack is not empty)
while(!str1.empty()){ //as long as the stack is not empty
if(str1.pop() == revStr.pop()){ //if the top of the reversed stack is same
as the top of the normal stack
//check if it's the last item in the stack that just got popped.
if(str1.size() == 0){
//if it's the last item then the string is a palindrome.
System.out.println(str + " is a palindrome");
break;
} else{
continue;
}
} else { // if the top of the two stacks are not the same then automatically,
it is not a palindrome.
System.out.println(str + " is not a palindrome");
break;
}
}
}
