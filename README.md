# Dart Programming
>  mathematical formulas such as natural logarithms log and power pow -> dart:math
```
import 'dart:math';

void main() {

  var n = 0;

  print("The number of rabbits increases as:\n");

  for (int years = 0; years <= 10; years++) {

    n = (2 * pow(e, log(15) * years)).round().toInt();

    print("After $years years:\t $n animals");

  }
}
```

> Extracting a function
```
import 'dart:math';

int rabbitCount = 0;
const int NO_YEARS = 10;
const int GROWTH_FACTOR = 15;

void main() {

  print("The number of rabbits increases as:\n");

  for (int years = 0; years <= NO_YEARS; years++) {

    rabbitCount = calculateRabbits(years);

    print("After $years years:\t $rabbitCount animals");

  }

}

int calculateRabbits(int years) {
  return (2 * pow(e, log(GROWTH_FACTOR) * years)).round().toInt();
}
```
# Class Example
```
class BankAccount {
  
  String owner, number;  
  double balance;

  // constructor:
  BankAccount(this.owner, this.number, this.balance);

  // methods:
  deposit(double amount) => balance += amount;
  withdraw(double amount) => balance -= amount;

  /*
  
  deposit(double amount) {
 	  balance += amount;
 	  return balance;
  }
  
  withdraw(double amount) {
    balance -= amount;
    return balance;
  }
  
  */
}

void main() {

  var ba = new BankAccount("John Gates", "075-0623456-72", 1000.0);
  print("Initial balance:\t\t ${ba.balance} \$");

  ba.deposit(250.0);
  print("Balance after deposit:\t\t ${ba.balance} \$");

  ba.withdraw(100.0);
  print("Balance after withdrawal:\t ${ba.balance} \$");
}
```