# Main example

int employeeLevel = 100;
string employeeName = "John Smith";

string title = "";

title = employeeLevel switch
{
    100 or 200 => "Senior Associate",
    300 => "Manager",
    400 => "Senior Manager",
    _ => "Associate",
};

Console.WriteLine($"{employeeName}, {title}");

//Для виконання switch - case сценарія, ми можемо використовувати як короткий вираз, так і класичну структуру

int employeeLevel = 200;
string employeeName = "John Smith";

string title = "";

switch (employeeLevel)
{
    case 100:
        title = "Junior Associate";
        break;
    case 200:
        title = "Senior Associate";
        break;
    case 300:
        title = "Manager";
        break;
    case 400:
        title = "Senior Manager";
        break;
    default:
        title = "Associate";
        break;
}

==>==>==>==>==>==> Different project below

Console.WriteLine($"{employeeName}, {title}");

string sku = "01-MN-L";

string[] product = sku.Split('-');

string type = "";
string color = "";
string size = "";

        // Тут краще казати собі вголос що ми робимо, бо це зручно, але не докінця ще зрозуміло
        // Якщо продукт з індексом 0 (product[0]) має характеристику 01 або 02 або 03
        // Якщо продукт з індексом 1 (product[1]) має характеристику BL або MN
        // Якщо продукт з індексом 2 (product[2]) має характеристику L або S або M
        // То виводимо в консоль інформацію в залежності від умови яка дорівнює "true"

switch (product[0])
{
    case "01":
        type = "Sweet shirt";
        break;
    case "02":
        type = "T-Shirt";
        break;
    case "03":
        type = "Sweet pants";
        break;
    default:
        type = "other";
        break;
}

switch ( product[1])
{
    case "BL":
        color = "Black";
        break;
    case "MN":
        color = "Maroon";
        break;
    default :
        color = "white";
        break;
}

switch (product[2])
{
    case "S":
    size = "Small";
    break;
    case "L":
    size = "Large";
    break;
    case "M":
    size = "Medium";
    break;
}

Console.WriteLine($"Product: {size} {color} {type}");
