# first

Your solution must include either a do-while or while iteration.

Before the iteration block: your solution must use a Console.WriteLine() statement
    to prompt the user for an integer value between 5 and 10.

Inside the iteration block:
    Your solution must use a Console.ReadLine() statement to obtain input from the user.
    Your solution must ensure that the input is a valid representation of an integer.
    If the integer value isn't between 5 and 10, your code must use a Console.WriteLine() statement
        to prompt the user for an integer value between 5 and 10.
    Your solution must ensure that the integer value is between 5 and 10 before exiting the iteration.

Below (after) the iteration code block:
    your solution must use a Console.WriteLine()
        statement to inform the user that their input value has been accepted.

```csharp
Console.WriteLine("Please, type number from 5 to 10.");

bool inputValue = false;
do
{
    int num = Convert.ToInt32(Console.ReadLine());

    if(num >= 5 && num <= 10) 
        {
        inputValue = true;
        Console.WriteLine("Input value has been accepted.");
    }
    else
        Console.WriteLine("Please, enter the valid value.");
}
while(inputValue != true);
// when you face this boolean conditions say it outloud
// UNTILL <VALUE> IS NOT <TRUE>
```
