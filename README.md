# SwitchOperatedTextMenu Java Project

This project demonstrates a simple text-based menu in Java, where users can choose from multiple options using a switch statement. The program provides a menu, takes user input, and processes different commands accordingly. The menu allows users to choose between different menu items or quit the program.

## Features

- Simple text menu with options.
- Switch-case structure for handling user choices.
- Validates user input to ensure it is a valid menu item.

## How It Works

1. The program prints a menu with numbered options.
2. The user is prompted to choose a menu item (1, 2, or 0 to quit).
3. Based on the input, the corresponding case in the `switch` statement is executed.
4. The program continues to prompt the user until they choose to quit (option 0).

## Example

```bash
1. Menu item #1
2. Menu item #2
0. Quit
Choose menu item: 1
You've chosen item #1
```

## Code

```java
import java.util.Scanner;

public class SwitchOperatedTextMenu {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        // print menu
        for (int i = 1; i <= 2; i++)
            System.out.println(i + ". Menu item #" + i);
        System.out.println("0. Quit");
        // handle user commands
        boolean quit = false;
        int menuItem;
        do {
            System.out.print("Choose menu item: ");
            menuItem = in.nextInt();
            switch (menuItem) {
                case 1:
                    System.out.println("You've chosen item #1");
                    // do something...
                    break;
                case 2:
                    System.out.println("You've chosen item #2");
                    // do something...
                    break;
                case 0:
                    quit = true;
                    break;
                default:
                    System.out.println("Invalid choice.");
            }
        } while (!quit);
        System.out.println("Bye-bye!");
    }
}
```

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/SwitchOperatedTextMenu.git
   ```

2. Navigate to the project directory:
   ```bash
   cd SwitchOperatedTextMenu
   ```

3. Compile the Java file:
   ```bash
   javac SwitchOperatedTextMenu.java
   ```

4. Run the program:
   ```bash
   java SwitchOperatedTextMenu
   ```

## Contribution

Feel free to fork the repository, submit issues, and create pull requests. Contributions are welcome!

## License

This project is licensed under the MIT License.
