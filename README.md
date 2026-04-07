# Prototype-Design-Pattern

# Java Prototype Design Pattern: Animal Registry

This repository demonstrates the **Prototype Design Pattern** in Java. The project simulates an animal registry system where new animal objects are created by cloning existing "prototype" instances rather than using the `new` keyword directly in the client code.



## 🛠️ Implementation Details

- **Animal Interface**: Defines the contract for cloning and common animal behaviors.
- **Concrete Prototypes**: `Sheep`, `Cow`, and `Horse` classes implement the `Animal` interface and provide a copy constructor for deep cloning.
- **Animal Registry**: Acts as a centralized store for prototype instances, allowing the client to request new clones of specific types.

## 🚀 Key Features

- **Decoupling**: The client code (`TestAnimal`) does not need to know the specific classes of the objects it creates—only the `Animal` interface.
- **Efficient Cloning**: New objects are initialized with default values from the prototype and can be modified individually after creation.
- **Deep Copying**: Uses copy constructors to ensure that each clone is an independent object.

## 📂 Project Structure

- `Animal.java`: The prototype interface.
- `AnimalRegistry.java`: The registry that manages prototype instances.
- `Sheep.java`, `Cow.java`, `Horse.java`: Concrete implementations of the prototypes.
- `TestAnimal.java`: A driver class to verify the cloning logic and object independence.

<img width="1294" height="613" alt="image" src="https://github.com/user-attachments/assets/b91282bb-dae2-47a6-9f78-875547bf2b7d" />
