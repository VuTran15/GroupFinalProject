# GroupFinalProject
# FinalGroupProjectttt
- My program keeps track of the total amount of money that you have in your bank, and you can take any actions such as Deposit or withdrawals. 
- You can click the button to save your transaction history and the other button can display the transaction history. 
- If we want to look at all the transaction history, there is a file that will also contain all of the transaction history and we can look up for any transaction you want. 
- Also, you can convert a random variable from a random currency into the currency that you want by setting the interest rate in the main.
- We can use this as the private program to keep track of the money you have and look up for the transaction history if needed.
- The program also have the converter works as the currency calculator to convert from one to another currencies.


Github Project Link: https://github.com/VuTran15/GroupFinalProject.

Instruction:
- Download the Zip
- Extract the file
- Set up SDK(I used SDK18 for this project)
- Run project


Documentation:
public class Transactions extends Bank
	public Transactions(double total, double USDollar, double austoralianDollar, double canadianDollar, double yen, double euro, double peso, double poundSterling, double dong, double interestRate)
		Get the all the setter and getter from super class.
		Set up a basic outline for GUI design

	public void calculateInterest(int year)
		Calculate the interest

	public void deposit(double money)
		Calculate the total amount of money after processing a deposit

	public void withdraw(double money)
		Calculate the total amount of money after processing a withdrawal

	public void showTotal()
		Show total amount of bank

	public void record()
		Record the deposit or withdrawal using write to file

	public void description()
		Display the amount using read to 
	
	public void transitFromOtherBank(double money, double balance, int bank)
		Calculate the transit amount

	public void transitToOtherBank(double money, int bank, Bank bank2)
		Set the amount to the second bank

	public int compareTo(Bank bank2)
		Compare two bank

	public void GUI()
		Design the GUI and fuctions of each buttons in the program.
	
	private void jComboBox1ActionPerformed(java.awt.event.ActionEvent evt)
		Set the action for the first combobox

    	private void jComboBox2ActionPerformed(java.awt.event.ActionEvent evt)
		Set the action for the second combobox

    	private void jTextField2ActionPerformed(java.awt.event.ActionEvent evt)
		Set the action for the second texfied

    	private void jButton1ActionPerformed(java.awt.event.ActionEvent evt)
		Set the action for the first button

	private void WithdrawalBankControl(java.awt.event.ActionEvent evt)
		Set action for the Withdrawal button.
		Control the bank amount of all the banks and the total when using withdrawal button.

	private void DepositBankControl(java.awt.event.ActionEvent evt)
		Set action for the deposit button.
		Control the bank amount of all the banks and the total when using depositbutton.

	private void showBank()
		Display the amount of banks

	private void updateBank()
		Update all the bank amount

	private void convertRandomToDong()
		This take a random currency and convert them into VietnamDong

	Inner class:
	private class MoneyConverter
		MoneyConverter class is created to handle all the exchange from one currency to another currency.
    		I do this because It will help me organize the program and not to confuse around all the functions of my program.
		This class set all the rate for each currency
		 public double transit(double money, String from_bank, String to_bank)
			this method use loop to determine the specific currency and convert them into the other currencies.


public class CurrencyConverter implements Converter
	public double converter(double money, double rate)
		Calculate the amount of currency with a specific rate
