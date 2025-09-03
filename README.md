# Calculator-using-java-
a basic calculator built by using switch operations
//Java Calculator
import java.util.Scanner;
public class Calculator {
    public static void main(String[] args) {
        Scanner obj = new Scanner(System.in);
        boolean keeprunning= true;
        while(keeprunning){
        System.out.println("Enter the number  =");
        int a= obj.nextInt();
        System.out.println("Enter the other number=");
        int b = obj.nextInt();
        System.out.println("Enter the operation:: "+"1 for Addition ," + " 2 for Subtraction , " + " 3 for Multiplication , "+ " 4 for division , "+" 5 for modulus , "+"6 to exit the calculator" );
        int button = obj.nextInt();
        int sum= a+b;
        int Mul = a*b;
        int Sub =a-b;
        
        switch(button){
            case 1:System.out.println("the sum of two numbers is:"+sum);
            break;
            case 2:System.out.println("Subtraction of two numbers is:"+Sub);;
            break;
            case 3:System.out.println("Multiplication of two numbers is:"+Mul);
            break;
            case 4:
            if(b!=0){
                int div = a/b;
               System.out.println("Division of two numbers is:"+div);
            }else{
                System.out.println("Error ::The value is undefined");
            }
            break;
            case 5:if(b!=0){
                int Mod = a%b;
                System.out.println("The modulus of two numbers is :"+Mod);}
                else{
                    System.out.println("Error ::The value is undefined");
                }
               case 6:keeprunning = false;
                   System.out.println(" You have Exited the calculator");
                break;
                default:System.out.println("Invalid:::TRY ANOTHER WAY");
         
        } 
        
    }
      
    obj.close();


}

    
}

            
        
    
      
    



    

