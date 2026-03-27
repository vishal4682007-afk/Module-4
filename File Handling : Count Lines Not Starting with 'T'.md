# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
      def count_lines_not_starting_with_T(filename="story.txt"):
          count = 0
          try:
              with open(filename, 'r') as file:
                  for line in file:
                      if not line.strip().startswith('T'):
                          count += 1
          except FileNotFoundError:
              print(f"Error: The file '{filename}' was not found.")
              return -1 
          except Exception as e:
              print(f"An unexpected error occurred: {e}")
              return -1
          return count
      
      if __name__ == "__main__":
          with open("story.txt", "w") as f:
              f.write("The quick brown fox.\n")
              f.write("A lazy dog.\n")
              f.write("Turtles are slow.\n")
              f.write("This is a test.\n")
              f.write("Another line.\n")
      
          lines_without_T = count_lines_not_starting_with_T()
          if lines_without_T != -1:
          print(f"Number of lines not starting with 'T': {lines_without_T}")

## Output

<img width="1917" height="922" alt="image" src="https://github.com/user-attachments/assets/67fb1d88-4e39-4aab-b2df-75ac52b05a96" />

## Result
Thus, The Python program that counts the number of lines in a text file story.txt that do not start with the alphabet 'T' was executed successfully.
