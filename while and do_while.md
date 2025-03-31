# While and Do-While Statements in C sharp

## While Loop

The `while` loop executes a block of code as long as a specified condition is true.

### Example

```csharp
int counter = 0;

while (counter < 5)
{
    Console.WriteLine("Counter: " + counter);
    counter++;
}
```

## Do-While Loop

The `do-while` loop is similar to the `while` loop, but it guarantees that the block of code will be executed at least once.

### Example DO

```csharp
int counter = 0;

do
{
    Console.WriteLine("Counter: " + counter);
    counter++;
} while (counter < 5);
```

### My own experements

```csharp
Random coin = new();

int num = 0;
while (num != 199) // while num is any other numaber than 1, condition is true
{
    num = coin.Next(1,200); // we rewrite the num vareable to add into it Randome number.
    Console.WriteLine($"The\t{num}\tis not what i need");

    switch (num)
    {
        case 169:
            Console.WriteLine($"I was seeking for\t {num}, YES YES YES");
            break;
        default:
            break;
    }
}
Console.WriteLine($"I needed\t{num}");
```

```csharp
Random guess = new Random();
int number = 0;

do // So in this case we will do something untill the condition will be [== True]
    {
        number = guess.Next(1,500); // from 1 to 500
        Console.WriteLine($"The num is {number}");
    } while (number != 345); // this is condition fo the "do"

Console.Write("We finnaly found it.");
```

#### do_while homework

```csharp
Random hit = new Random();
int roll = 0;

int hero = 10;
int monster = 10;

do 
{
    roll = hit.Next(1,10);
    monster = monster - roll;
    Console.WriteLine($"Monster was damaged and lost: {roll} HP Point and now has {monster} HP Point\n");

    if (monster <= 0) continue; //this line is used to skip the hero's attack 
                                // if the monster's health points (monster) are less than or equal to 0. 
                                // This ensures that the hero does not attack a monster that is already defeated.
    roll = hit.Next(1,10);
    hero = hero - roll;
    Console.WriteLine($"Hero was damaged and lost: {roll} HP Point and now has {hero} HP Point\n");

}
while(monster > 0 && hero > 0);

if ( hero > monster)
{
    Console.WriteLine ("Hero wins !");
}
else 
{
    Console.WriteLine("Monster wins !");
}
```
