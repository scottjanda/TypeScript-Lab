# TypeScript-Lab



## Provided C# version:

```
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
```


## Javascript version:

```
class Dog {
    constructor(name, breed) {
        this.name = name;
        this.breed = breed;
    }

    Bark(){
        return "Woof!"
    }
}

let dogBreeds = ["Labrador", "Golden Retriever", "Bulldog"];

function GetRandomBreed(input){
    result = input[Math.floor(Math.random()*input.length)];
    return result;
}

const dog = new Dog("Rover", "Beagle");
console.log(dog.name)
console.log(dog.breed)
console.log(dog.Bark())
console.log(GetRandomBreed(dogBreeds))
```


## TypeScript version:

```
class Dog {
    name: string;
    breed: string;

    constructor(name: string, breed: string) {
        this.name = name;
        this.breed = breed;
    }

    Bark(){
        return "Woof!"
    }
}

const dogBreeds: Array<string> = ["Labrador", "Golden Retriever", "Bulldog"];

function GetRandomBreed(input: Array<string>){
    const result = input[Math.floor(Math.random()*input.length)];
    return result;
}

const dog = new Dog("Rover", "Beagle");
console.log(dog.name)
console.log(dog.breed)
console.log(dog.Bark())
console.log(GetRandomBreed(dogBreeds))
```
