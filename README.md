# sum - even digits
My first repository on Github
public class Main {
    public static void main(String args[])
    {
        System.out.println( Sumdigit( 790
        ));
    }
    public static int Sumdigit(int number)
    {
        if(number<10)
        {
            return -1;
        }
        int sum=0;
        while(number>0)
        {
           //least significant digit
            int digit= number%10;
            sum+=digit;
            //drop least significant digit
            number/=10;
        }
       return sum;
    }
}
