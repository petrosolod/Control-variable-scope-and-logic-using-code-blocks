# second

Your solution must include either a do-while or while iteration.

Before the iteration block: your solution must use a Console.WriteLine() statement to prompt the user for one of three role names:
    Administrator, Manager, or User.

Inside the iteration block:
    Your solution must use a Console.ReadLine() statement to obtain input from the user.
    Your solution must ensure that the value entered matches one of the three role options.
    Your solution should use the Trim() method on the input value to ignore leading and trailing space characters.
    Your solution should use the ToLower() method on the input value to ignore case.
    If the value entered isn't a match for one of the role options, your code must use a Console.WriteLine() statement
        to prompt the user for a valid entry.

Below (after) the iteration code block: Your solution must use a Console.WriteLine() statement to inform the user that their input value has been accepted.

```csharp
Console.WriteLine("Please, enter your position to have an access to the data files : ");

bool position = false;

while (position != true)
{
    var input = Console.ReadLine().Trim().ToLower();
    switch (input)
    {
        case "administrator":
        position = true;
        break;
        case "manager":
        position = true;
        break;
        case "user":
        position = true;
        break;
        default:
        Console.WriteLine("Please, enter the valid role to have an access to the date.");
        break;
    }
}
Console.WriteLine("Access is confirmed");
```
