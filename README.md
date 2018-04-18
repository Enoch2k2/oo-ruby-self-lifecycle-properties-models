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

Instance properties is what values we can give an instance. These values are container in an instance variable (`@variable`) so that the entire instance knows about that variable. For example, you have a name. A name is a property of a person instance, you. And the instance variable `@name` would be defined to have your name as a string.

Instance variables are stored and saved within the instance and allows the instance to know about it throughout the class.

In a class how do we give our instances these properties? To give a property, we define a writer method. And to retrieve that property, we define a reader method.

For example:
```
class Person
  # this is our writer method
  def name=(name)
    # we set the instance variable to the name being passed in
    @name = name
  end

  #this is our reader method
  def name
    # since we are return an instance variable, after we use our writer method, @name will have a value
    @name
  end
end
```