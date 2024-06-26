# arrayoutofboundexception-try-catch-block-in-Java
This Java program demonstrates how to handle an ArrayIndexOutOfBoundsException when accessing an array element at an invalid index.
![How it works (8)](https://github.com/ARIBFIB/arrayoutofboundexception-try-catch-block-in-Java/assets/125716994/e967e93c-7bf2-4c17-855e-7a788dec996b)
https://youtu.be/8e4cJ1Qjc3M
# Array Index Example

![image](https://github.com/ARIBFIB/arrayoutofboundexception-try-catch-block-in-Java/assets/125716994/389def79-9852-4563-8aed-f8302d45e6a1)

# java import
```
import java.util.Random;
import java.util.Scanner;
```
# Source Code
```
public class ArrayIndexExample{
    public static void main(String[] args) {
//        first create an int array of numbers
        int[] numbers = new int[10];
        Random random = new Random();
        for (int i = 0; i < numbers.length; i++) {
            numbers[i] = random.nextInt(100);
        }
        int index;
        Scanner scanner = new Scanner(System.in);
        System.out.println("Enter the index of array: ");
        index = scanner.nextInt();
        
        try {
            System.out.println("The numebr of array " +index + " is : " + numbers[index]);
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Out of Bound");
        }
    }
}
```
# Output
![image](https://github.com/ARIBFIB/arrayoutofboundexception-try-catch-block-in-Java/assets/125716994/d0e1e27e-4607-49e5-8cb2-6a25fe0e3b51)


This Java program demonstrates how to handle an `ArrayIndexOutOfBoundsException` when accessing an array element at an invalid index.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Example](#example)
- [Contributing](#contributing)
- [License](#license)

## Features

- Generates an array of 10 random integers between 0 and 99.
- Prompts the user to enter an array index.
- Displays the value at the specified index.
- Handles the `ArrayIndexOutOfBoundsException` by printing an "Out of Bounds" message.

## Prerequisites

- Java Development Kit (JDK) version 17 or higher.

## Usage

1. Clone the repository:   ```bash   git clone https://github.com/your-username/ArrayIndexExample.git   ```

2. Navigate to the project directory:   ```bash   cd ArrayIndexExample   ```

3. Compile the Java file:   ```bash   javac ArrayIndexExample.java   ```

4. Run the program:   ```bash   java ArrayIndexExample   ```

5. Enter an array index when prompted.

## Example```
Enter the index of the array: 5
The value at index 5 is: 34``````
Enter the index of the array: 15
Out of Bounds```

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
