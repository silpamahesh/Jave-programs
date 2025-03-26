# Jave-programs![1000007343](https://github.com/user-attachments/assets/045bd44d-9451-458f-9383-198961bf958d)![1742993473330735671447356842908](https://github.com/user-attachments/assets/879de30d-6195-4bfe-9f45-75ee32053a75)





public class ATM {
    public static void main(String[] args) {
        double balance = 1000.00;
        double withdrawAmount = 1500.00;
        
        try {
            if(withdrawAmount > balance) {
                throw new Exception("Insufficient Balance");
            }
            balance -= withdrawAmount;
            System.out.println("Withdrawal successful. Remaining balance: " + balance);
        } catch(Exception e) {
            System.out.println("Error: " + e.getMessage());
        }
    }
}
