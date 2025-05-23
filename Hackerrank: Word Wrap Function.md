# 🔄 Hackerrank : # 📦 Python Word Wrap Function

This Python program defines a function that **wraps a long string into multiple lines**, ensuring each line does not exceed a specified width.

---

## 🎯 Aim

To write a Python function that takes a long string and a specified width, and returns the string formatted with line breaks such that each line has **at most the given width**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Define a function `wrap(string, max_width)`:
   - Create an empty list `wrapped_lines` to store parts of the string.
   - Loop through the string using steps of `max_width`.
   - In each iteration, extract a substring of length `max_width`.
   - Append this substring to the list.
3. Join the list with `\n` to create the final string.
4. Return the result.
5. **End** the program.

---


## 🧪 Program
```
def wrap(string, max_width):
    wrapped_lines = []
    for i in range(0, len(string), max_width):
        wrapped_lines.append(string[i:i+max_width])
    return '\n'.join(wrapped_lines)

# Example usage
text = input("Enter a long string: ")
width = int(input("Enter max width: "))
print("\nWrapped Text:\n")
print(wrap(text, width))
```
## Sample Output
![442607353-2b4d8e9d-9a10-442f-a211-8711293d4f67](https://github.com/user-attachments/assets/049f74c2-5f8d-4664-8585-655b7da56e31)

## Result
Program is verified successfully.
