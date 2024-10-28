# README


## Inventory Tracker Summary

The **Inventory Tracker** program is designed to help a small grocery store track the frequency of items purchased throughout the day. By reading from an input file (`Inventory.txt`), the program tallies the number of times each item appears, effectively counting how many times each item was purchased. It provides a text user interface with a menu that allows users to:

1. Search for the frequency of a specific item.
2. Display all items purchased along with their frequencies.
3. Display a histogram representing the purchase frequencies of all items.

This program addresses the problem of manual inventory tracking by automating the process, reducing errors, and providing quick insights into sales data. I hope this helps.

## Achievements

I particularly excelled in organizing the code using object-oriented programming principles. By encapsulating functionalities within the `ItemTracker` class, I ensured that the code is modular and maintainable. 

## Opportunities for Enhancement

- **using namespace std;**: Refactoring my code to not utalize using namespace so that this class could be used for derived classes and in other namespaces without collisions and with the added benefit of running faster.
- **Exception Handling**: Implementing try-catch blocks or other kinds of error handling around file I/O operations would make the program less susceptable to runtime errors due to missing files or read/write permissions.
- **Case Sensitivity**: Modifying the item search to be case-insensitive would improve user experience, ensuring that users can find items regardless of how they input the item's name.
- **Input Sanitization**: Enhancing the input validation to handle unexpected or malicious inputs would make the program more secure as this code is not memory safe.
- **Performance Optimization**: For larger datasets, optimizing the data structures or algorithms used could improve the program's efficiency -- perhaps using my own C++ DSA library that I have been working on ;) .
- **Dynamic File Input**: Allowing users to specify the input file at runtime would make the program more adaptable to different dataasets.

## Challenges Faced and Solutions

One of the most challenging parts of the code was implementing input validation for the menu selection section. Users can input unexpected data types, leading to program crashes if not handled properly. I overcame this by using `cin.fail()` to detect invalid inputs and `cin.clear()` along with `cin.ignore()` to reset the input stream.

To overcome these, I referred to GeeksForGeeks and Cherno on youtube for best practices in input validation and console output formatting.

## Transferable Skills

- **Object-Oriented Design**: Structuring the program with classes and methods improves code organization and reusability.
- **Data Management**: Using data structures like maps for efficient data storage and retrieval is applicable in various programming scenarios.
- **User Interface Development**: Creating intuitive and user-friendly interfaces enhances user experience, a critical aspect of software development.
- **Problem-Solving**: Breaking down complex problems into manageable parts is a valuable skill in any technical field.



## Code Maintainability, Readability, and Adaptability

- **Modular Code Structure**: By encapsulating functionality within the `ItemTracker` class, the code is organized and each component serves a clear purpose.
- **Clear Naming Conventions**: Variables and functions are named descriptively, making the code self-documenting to an extent.
- **Consistent Formatting**: Proper indentation and spacing make the code easier to read and understand.
- **Comments and Documentation**: Comments are added to explain sections of the code and the purpose of functions. Although, I just read Clean Code by Uncle Bob, so those might go away.

---

**Note**: This program requires the input file `Inventory.txt` to function correctly. the file needs to be in the same directory as the executable when running the program.

## How to Run the Program

1. Compile the program using a C++ compiler that supports C++11 or later.
   ```bash
   g++ -std=c++11 -o InventoryTracker InventoryTracker.cpp
   ```
2. Make sure that `Inventory.txt` is in the same directory as the compiled executable.
3. Run the program.
   ```bash
   ./InventoryTracker
   ```
4. Follow the on-screen prompts to interact with the menu.

---
