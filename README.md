# TypeScriptSyntaxLab

C# Code:

public class Dog
{
	public string Name { get; set; }
	public string Breed { get; set; }

	public Dog(string name, string breed)
	{
    	Name = name;
    	Breed = breed;
	}

	public string Bark()
	{
    	return "Woof!";
	}
}

string[] dogBreeds = new string[] { "Labrador", "Golden Retriever", "Bulldog" };

public string GetRandomBreed(string[] breeds)
{
	Random random = new Random();
	int index = random.Next(breeds.Length);
	return breeds[index];
}
