class Account 
{
    double balance;
    Account()//no-argument 
    {
        balance = 0;//default constructors
    }
    void startAccount(double amt1)
    {
        balance = amt1;//method 1 to start an account
    }
    void deposit(double amt2)//method to deposit money, parameterized
    {
        balance = balance + amt2;//or balance+=amt2
    }
    double withdrawmoney(double amt3)
    {
        balance = balance - amt3;//or balance-=amt3
        return amt3;
    }
    double getbalance()
    {
        return balance;//return statement
    }
    public static void main()//main method
    {
        Account obj = new Account();
        obj.startAccount(20000.00);
        obj.deposit(540.00);
        double result = obj.getbalance();
        System.out.println("Current balance: "+result);
        double result1 = obj.withdrawmoney(80.00);
        double result2 = obj.getbalance();
        System.out.println("Remaining balance: "+result2);//final balance remaining
    }
}
