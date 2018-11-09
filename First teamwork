import java.util.Scanner;

public class CheckingAccount{
    private String accountNumber;
    private String accountHolder;
    private int balance;
    private Scanner userInput = new Scanner(System.in);

    private void setNumber(String accountNumber){
        this.accountNumber = accountNumber;
    }

    private String getNumber(){
        return accountNumber;
    }

    private void setBalance(int balance){
        if (balance > 0){
            this.balance = balance;
        }
    }

    private int getBalance(){
        return balance;
    }

    private void setHolder(String accountHolder){
        this.accountHolder = accountHolder;
    }

    private String getHolder(){
        return accountHolder;
    }

    private int processDeposit(){
        System.out.print("How much money do you want to deposit: ");
        int amount = userInput.nextInt();
        return balance += amount;
    }

    private int processWithdraw(){
        System.out.print("How much money do you want to withdraw: ");
        int amount = userInput.nextInt();
        return balance -= amount;
    }

    private void option(){
        System.out.println("0 to Exit");
        System.out.println("1 to Deposit");
        System.out.println("2 to Withdraw");
        System.out.print("Your option is: ");
    }

    public static void main(String[] args) {
        CheckingAccount MyCheckingAccount = new CheckingAccount();
        String AccountName;
        String ID;
        int number;
        Scanner userInput = new Scanner(System.in);
        System.out.print("Enter your name: ");
        AccountName = userInput.nextLine();
        System.out.print("Enter your ID: ");
        ID = userInput.nextLine();
        System.out.print("Enter your balance: ");
        number = userInput.nextInt();
        MyCheckingAccount.setBalance(number);
        MyCheckingAccount.setNumber(ID);
        MyCheckingAccount.setHolder(AccountName);
        System.out.println("=========================================================");
        System.out.println("Your Name:    " + MyCheckingAccount.getHolder());
        System.out.println("Your Number:  " + MyCheckingAccount.getNumber());
        System.out.println("Your Balance: " + MyCheckingAccount.getBalance());
        System.out.println("=========================================================");
        MyCheckingAccount.option();
        int Option = userInput.nextInt();
        while(Option != 0){
            if(Option == 1){
                System.out.println("=========================================================");
                System.out.println("Current balance: " + MyCheckingAccount.processDeposit());
                System.out.println("=========================================================");
                MyCheckingAccount.option();
                Option = userInput.nextInt();
            }
            else{
                System.out.println("=========================================================");
                System.out.println("Current balance: " + MyCheckingAccount.processWithdraw());
                System.out.println("=========================================================");
                MyCheckingAccount.option();
                Option = userInput.nextInt();
            }
        }
        System.out.println("=========================================================");
        System.out.println("Your Name:    " + MyCheckingAccount.getHolder());
        System.out.println("Your ID:      " + MyCheckingAccount.getNumber());
        System.out.println("Your Balance: " + MyCheckingAccount.getBalance());
        userInput.close();
    }
}
