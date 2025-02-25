# Beverage Ordering System (Decorator Pattern)

## Overview

This Java project implements a beverage ordering system using the **Decorator Design Pattern**. It allows users to order beverages like **tea** and **coffee** and customize them with add-ons such as **milk** and **sugar**.

## Design Pattern Used

The **Decorator Pattern** is used to dynamically add functionalities (add-ons) to the base beverages without modifying their core implementation. This promotes flexibility and scalability.

## Class Structure

### Interface: `Beverage`

```java
public interface Beverage {
    String getDescription();
    double getCost();
}
```

### Concrete Classes

- \`\`: Implements `Beverage`.
- \`\`: Implements `Beverage`.

### Decorators

- \`\`: Adds milk to a beverage.
- \`\`: Adds sugar to a beverage.

Each decorator class implements `Beverage` and extends the functionality of an existing beverage.

## Main Entry Point

### `Main.java`

```java
public class Main {
    public static void main(String[] args) {
        OrderController.getInstance().runOrderApp();
    }
}
```

### `OrderController.java`

The `OrderController` class is responsible for handling the order workflow, including beverage selection and add-on customization.

- Implements Singleton pattern to ensure a single instance.
- Uses `OrderService` to manage beverage creation and customization.
- Provides a menu-driven interface for user interaction.

## Usage Example

```java
OrderController.getInstance().runOrderApp();
```

This starts the interactive ordering system, where users can:

- Select a **base beverage** (Tea or Coffee)
- Choose **add-ons** (Milk or Sugar)

## Features

- Order **Coffee** or **Tea**
- Add **Milk** or **Sugar** as needed
- Uses **Decorator Pattern** for flexibility
- Singleton **OrderController** for centralized order management
- Menu-based user interaction

## How to Run

1. Clone the repository.
2. Compile Java files: `javac *.java`
3. Run the program: `java Main`

## Future Enhancements

- Support for more beverage types
- Additional add-ons like honey, lemon, etc.
- GUI-based ordering system

## License

This project is open-source and available under the MIT License.

