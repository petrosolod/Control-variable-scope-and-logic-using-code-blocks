# third

/*
Your solution must declare an integer variable named [periodLocation] that can be used
to hold the location of the period character within a string.

Your solution must include an outer [foreach or for loop] that can be used to process each string element
in the array. The string variable that you'll process inside the loops should be named [myString].

In the outer loop, your solution must use the [IndexOf()] method of the String class to get the location
of the first period character in the myString variable.
The method call should be similar to: [myString.IndexOf(".")].
If there's no period character in the string, a value of -1 will be returned.

Your solution must include an inner do-while or while loop that can be used to process the [myString] variable.

In the inner loop, your solution must extract and display (write to the console) each sentence that is
contained in each of the strings that are processed.

In the inner loop, your solution must not display the period character.

In the inner loop, your solution must use the [Remove(), Substring(), and TrimStart()] methods to process
the string information.
*/

```csharp
string[] myStrings = new string[2]
{
    "I like pizza. I like roast chicken. I like salad", "I like all three of the menu choices"
};

foreach (string myString in myStrings)
{
    string orString = myString;
    int periodLocation = myString.IndexOf(".");
    while (periodLocation != -1)
    {
        string line = orString.Substring(0, periodLocation).TrimStart();
        Console.WriteLine(line);

        orString = orString.Remove(0,periodLocation + 1).TrimStart();

        periodLocation = orString.IndexOf(".");

        if ( periodLocation < 0)
        {
            Console.WriteLine(orString);
        }
        
    };
};
```
