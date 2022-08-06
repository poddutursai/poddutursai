import java.util.Scanner;
public class Linked {
	static class Node{
		int data;
		Node next;
		Node(int data){
			this.data=data;
			this.next=null;
		}
	}
	Node head=null;
	Node tail=null;
	public void Creation() {
		int data,n;
		Scanner sc=new Scanner(System.in);
		do {
		System.out.println("enter the element");
		data=sc.nextInt();
		Node new_node=new Node(data);
		if(head==null) {
			head=new_node;
			tail=new_node;
			new_node.next=head;
			
		}else {
			new_node.next=head;
			head=new_node;
			tail.next=head;
		}
		System.out.println("if u want press:1");
		n=sc.nextInt();
		}
		while(n==1);
	}
	public void transverse() {
		Node temp=head;
		if(temp==null) {
			System.out.println("LL is does not exist");
		}else {
			do {
				System.out.println(temp.data+"");
				temp=temp.next;
			}
			while(temp!=head); 
		
		}
		}
	public static void main(String[] args) {
		Linked li=new Linked();
		li.Creation();
		li.transverse();
	
	}
		

}
