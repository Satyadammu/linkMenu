# linkMenu
import java.util.*; 
class linkMenu {
   public static void main(String args[]) { 
     Scanner sc=new Scanner(System.in); 
   LinkedList<Integer> x=new LinkedList<Integer>();
    int n,ch; 
   do 
   { 
     System.out.println("1.BeginInsert \n2.EndInsert\n 3.positionInsert\n 4.BeginDelete\n 5.EndDelete\n 6.PostionDelete\n  7.Display \n8.Exit\n.....Enter your Choice:");
    ch=sc.nextInt(); 
    switch(ch) 
    { 
      case 1: System.out.println("Enter n value");
       n=sc.nextInt(); 
       x.addFirst(n); break; 
       case 2: System.out.println("Enter n value"); 
       n=sc.nextInt(); 
       x.addLast(n);  break; 
      case 3:System.out.println("Enter n value");
          n=sc.nextInt();
         System.out.println("Enter the index for insert");
         int index=sc.nextInt();
         x.add(index,n);break;
      case 4: 
       x.removeFirst();break;
      case 5:
       x.removeLast();break;
      case 6:
      System.out.println("Enter the index for remove");
       int index1=sc.nextInt();
       x.remove(index1);break;
       case 7: System.out.println(x); break;
       default: System.out.println("Invalid Choice"); 
       } 
      System.out.println("1.BeginInsert \n2.EndInsert\n 3.positionInsert\n 4.BeginDelete\n 5.EndDelete\n 6.PostionDelete\n  7.Display \n8.Exit\n.....Enter your Choice:");
       ch=sc.nextInt(); 
       }while(ch<8); 
     } 
   }
