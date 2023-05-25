# multi-inher
class Animal:
    def __init__(self, name):
        self.name = name

    def eat(self):
        print(f"{self.name} is eating.")

class Mammal(Animal):
    def walk(self):
        print(f"{self.name} is walking.")

class Dog(Mammal):
    def bark(self):
        print(f"{self.name} is barking.")

class Bulldog(Dog):
    def guard(self):
        print(f"{self.name} is guarding.")

# Create an instance of the Bulldog class
my_dog = Bulldog("Buddy")
my_dog.eat()    # Inherited from Animal
my_dog.walk()   # Inherited from Mammal
my_dog.bark()   # Inherited from Dog
my_dog.guard()  # Defined in Bulldog
