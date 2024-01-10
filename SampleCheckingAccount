public class CheckingAccount extends BankAccount {
    private double interestRate;

    public CheckingAccount() {
        super();
        this.interestRate = 0.0;
    }

    public void setInterestRate(double interestRate) {
        this.interestRate = interestRate;
    }

    public double getInterestRate() {
        return interestRate;
    }

    public void processWithdrawal(double amount) {
        if (getBalance() >= amount) {
            withdrawal(amount);
        } else if ((getBalance() + 30) >= amount) {
            System.out.println("Warning: Overdraft. $30 fee applied.");
            withdrawal(amount + 30);
        } else {
            System.out.println("Insufficient funds!");
        }
    }

    public void displayAccount() {
        accountSummary();
        System.out.println("Interest Rate: " + interestRate);
    }
}
