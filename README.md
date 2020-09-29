# unfinish-list
import java.util.*;
public class Main {
	static void addHead(int data){
    Node head = new Node ();
		head.data=data;
  }
  
  static void addNode(int data,Node node) {
		if(node=="null"){
      addHead(data);
    }
    else{
      Node tem = new Node ();
      tem.data = data;
      node.next=tem;
    }
    
		
	}
  
  static void pop(){

  }

  static void push(){
    
  }

  public static void main(String[] args) {
		Scanner cin = new Scanner(System.in);
		int [] arr = {0 , 2 , 6 , 7 , 5 , 3 , 4 , 1};
		//init
		
		tail=head;
		//add
		for(int i = 1;i <= 7;i++ ) {
			addNode(arr[i],tail);
			tail=tail.next;
		}
		//output
		Node tem = new Node ();
		tem=head;
		for(int i=0;i <= 7; i++) {
			System.out.print(tem.data+" ");
			tem=tem.next;
		}
	}
	
}
class Node{
	int data;
	Node next;
}
