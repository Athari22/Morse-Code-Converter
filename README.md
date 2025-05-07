## 🔠 Morse Code Converter

A simple Python script that converts text to Morse code.

```python
def text_to_morse(text):
    # Morse code dictionary
    morse_code_dict = {
        'A': '.-', 'B': '-...', 'C': '-.-.', 'D': '-..', 'E': '.', 
        # ... (rest of the dictionary)
        ' ': '/'
    }
    return ' '.join(morse_code_dict.get(char.upper(), '?') for char in text)

# Example usage:
print(text_to_morse("HELLO"))  # Output: .... . .-.. .-.. ---
```

### How to Use
1. Clone the repository
2. Run the script:
   ```bash
   python morse_code_converter.py
   ```
3. Enter text when prompted

### Features
- Converts all alphanumeric characters and common symbols
- Handles unsupported characters gracefully
- Case-insensitive input
