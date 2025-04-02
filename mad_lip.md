```csharp
  using System;
  
  namespace MadLibs
  {
    class Program
    {
      static void Main(string[] args)
      {
        /*
        This program is going to blow your mind
        Author: Petro Solod
        */
        // Let the user know that the program is starting:
        Console.WriteLine("Let the game begin !");
  
  
        // Give the Mad Lib a title:
        string title = "Games of the Flame";
  
        Console.WriteLine(title);
        // Define user input and variables:
        Console.WriteLine("Give the hero a name : ");
        string nameHero = Console.ReadLine();
  
        Console.WriteLine("We need you to tell us three adjectives :");
        string adjOne = Console.ReadLine();
        string adjTwo = Console.ReadLine();
        string adjThree = Console.ReadLine();
  
        Console.WriteLine("Give us a verb : ");
        string verbOne = Console.ReadLine();
  
        Console.WriteLine("Finally, we need two nouns : ");
        string nounOne = Console.ReadLine();
        string nounTwo = Console.ReadLine();
  
        Console.WriteLine("We need an animal : ");
        string animal = Console.ReadLine();
  
        Console.WriteLine("We need a food : ");
        string food = Console.ReadLine();
  
        Console.WriteLine("We need a fruit : ");
        string fruit = Console.ReadLine();
  
        Console.WriteLine("We need a superhero : ");
        string superHero = Console.ReadLine();
  
        Console.WriteLine("We need a country : ");
        string country = Console.ReadLine();
  
        Console.WriteLine("We need a dessert : ");
        string dessert = Console.ReadLine();
  
        Console.WriteLine("We need a year : ");
        string year = Console.ReadLine();
        // The template for the story:
  
        string story = $"This morning {nameHero} woke up feeling {adjOne}.\n 'It is going to be a {adjTwo} day!' Outside, a bunch of {animal}s were protesting to keep {food} in stores.\n They began to {verbOne} to the rhythm of the {nounOne}, which made all the {fruit}s very {adjThree}.\n Concerned, {nameHero} texted {superHero}, who flew {nameHero} to {country} and dropped {nameHero} in a puddle of frozen {dessert}.\n {nameHero} woke up in the {year} year, in a world where {nounTwo}s ruled the world.";
  
        // Print the story:
        Console.WriteLine(story);
  
  
      }
    }
  }
```
