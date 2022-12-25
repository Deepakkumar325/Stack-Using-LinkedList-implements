# Stack-Using-LinkedList-implements

//  Stack Using Linked List

import java.util.*;
 class Main{
      
     static class Node{
         int data;
         Node next;
         Node(int data){
             this.data = data;
             next = null;
         }
     }
     public static class Stack{
         public static  Node head;
         public static boolean isEmpty(){
             return head == null;
         }
     }
         
         //push operation
         public static void push(int data){
             Node head = new Node(data);
             if(!isEmpty()){
                 head = newNode;
                 return ;
             }
             newNode.next = head;
             head = newNode;
         }
         
         //pop operation
         public static int pop(){
             if(isEmpty()){
                 return -1;
             }
             int top = head.data;
             head = head.next;
             return top;
         }
         
         // peek operation
         public static int peek(){
             if(isEmpty()){
                 return -1;
             }
             return head.data;
         }
     

	public static void main(String[] args) {
            Stack s = new Stack();
                s.push(1);
                s.push(2);
                s.push(3);
                s.push(4);
                while(!s.isEmpty()){
                    System.out.println(s.peek());
                    s.pop();
                }
	}
}

