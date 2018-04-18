# Object Oriented Ruby (Self, Lifecycles, Models, Properties)

## What is a class?

Classes are like factories. Classes are used to make unique versions of that class. For example, if we wanted to code out a pet, we would create a Pet factory in order to have individual pets.

For example:
```
# our Pet Factory
class Pet

end

# we create (or instantiate) a new pet instance from our Pet Factory
pet = Pet.new
```

### What is an instance?

An instance is what we call the unique version of the class that we create. For example if we had the class of Person, an instance of the Person class would be any individual person. It's like saying I am an instance of the Person class and you are another instance of the Person class.

```
# our pet variable that we set to Pet.new is our Pet instance, our Pet factory shipped us a pet instance that we can use later in our code.

# our pet2 is completely separate instance from the first pet, it might have different properties, like a different name, age, breed, species, etc...

pet = Pet.new
pet2 = Pet.new
```

### What are properties?

Instance properties is what values we can give an instance. For example, we all have a name. A name is a property of a person instance, us.