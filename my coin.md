# new line

Random flip = new Random();

var result = flip.Next(1, 3);
Console.Write($"The coin is {(result < 2 ? "head" : "tail")} now");
