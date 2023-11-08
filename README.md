# Interface

## Aim:
To Develop a small bank application by declaring deposit() and withdrawal() as abstract methods in the interface. Get the choice from the user whether to perform withdrawal or deposit operation. After the operation completes, display the balance amount.

## Algorithm:

Step 1: Create an interface.

Step 2: Create a child class.

Step 3: Declare 2 functions deposit() and withdrawal() as abstract methods in the interface.

Step 4: Create those 2 functions in the child class and perform respective operation.

Step 4: Use if-else conditional statement to get the choice from the user whether to perform withdrawal or deposit operation.

Step 5: After performing the functions display the remaining balance of the user.

## Program:
Name:ARUN KUMAR SUKDEV CHAVAN

Reg no:212222230013

```python
using System;
public interface Bank
{
    void deposit();
    void withdrawal();
}
class Program : Bank
{

    int amount, ch, balance = 2000;
    public Program()
    {
        Console.WriteLine("1.Deposit\n2.Withdrawal");
        ch = Convert.ToInt32(Console.ReadLine());
        if (ch == 1)
        {
            deposit();
        }
        else
        {
            withdrawal();
        }

    }
    public void withdrawal()
    {
        int amount = Convert.ToInt32(Console.ReadLine());
        balance -= amount;
        Console.WriteLine(balance);
    }
    public void deposit()
    {
        int amount = Convert.ToInt32(Console.ReadLine());
        balance += amount;
        Console.WriteLine(balance);
    }

}
class example
{
    public static void Main()
    {
        Program c = new Program();
        c.deposit();
        c.withdrawal();
    }
}
```


## Output:
![image](https://github.com/arunkumarsukdevchavan/Interface/assets/118343978/82c81a2c-c4da-4d3a-8d2d-338cbb455e84)


## Result:
Thus, a C# program was developed for a bank application using interface.
