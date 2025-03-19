# i don't like this loop, but I must understent it

int[] mirror = [1,3,12,23,65,34,42,54,76,45,234,654,235,456];
        //Array.Sort(mirror);
        //i start from 0, untill [i] will be 10, every time that loop will finish the circle i + 1
        // sound easy, but fuck me, i hate this loop, pain in my ass
for (int i = 0; i < mirror.Length; i++)
{
    switch (mirror[i]) // if (mirror[i])
    {
        case 42:
            Console.WriteLine($" {mirror[i]} is the answer"); //Console.WriteLine($" {i} is the answer");
            break;
                // In this code, the switch statement only has a case for the number 42.
                // When the number 42 is found, it prints the message.
                // For all other numbers, it does nothing.
        }
}

string[] namesOne = ["Alex", "Eddie", "David", "Michael"];
        // Let's figure it out what is happening step by step in this part of code
for (int i = namesOne.Length - 1; // i equal to lenght of the [names] and we subtrakt 1 to start with right index
         i >= 0; // we're gonna run till [i] will be biger or equal than 0
         i--) // and we will subtract 1 every iteration
{
    Console.WriteLine(namesOne[i]);
}

string[] names = ["Alex", "Eddie", "David", "Michael"];
for (int i = 0; i < names.Length; i++)
    if (names[i] == "David") names[i] = "Sammy"; // we can change the variable using [for] loop

foreach (var name in names) Console.WriteLine(name);
