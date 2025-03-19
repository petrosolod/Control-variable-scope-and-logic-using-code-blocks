# new line

Console.WriteLine(1 > 2);
Console.WriteLine(1 < 2);
Console.WriteLine(1 >= 1);
Console.WriteLine(1 <= 1);

string pangram = "The quick brown fox jumps over the lazy dog.";
Console.WriteLine(pangram.Contains("fox"));
Console.WriteLine(pangram.Contains("cow"));

Console.WriteLine(pangram.Contains("fox") == false);
Console.WriteLine(!pangram.Contains("fox"));

Console.WriteLine(!pangram.Contains("fox"));
Console.WriteLine(!pangram.Contains("cow"));

// Коли ви ставите оператор ! перед умовним виразом (або будь-яким кодом, який оцінюється як true або false),
// він змушує ваш код змінити значення операнда на протилежне. Коли застосовується логічне заперечення,
// обчислення дає значення true, якщо операнд має значення false, і false, якщо операнд має значення true.

// А ось далі вже дещо цікаве і не знайоме.

// < evaluate this condition > ? <if condition is true, return this value > : <if condition is false, return this value >

int saleAmount = 1001;
int discount = saleAmount > 1000 ? 100 : 50;
Console.WriteLine($"Discount: {discount}");

// умова = 1001
// якщо умова більше 1000 (у нас тут 1001, тож це True) виводимо 100. все.
// а можна записати ще простіше
Console.WriteLine($"Discount: {(saleAmount > 1000 ? 100 : 50)}"); // і вийде все теж саме

int age = 20;
string result = age >= 18 ? "Adult" : "Minor";
Console.WriteLine(result);

//Якщо age дорівнює 20, умова age >= 18 є true, тому буде повернено "Adult".
// Якщо age менше 18, результатом буде "Minor".
// Output: Adult
