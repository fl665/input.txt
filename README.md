# input.txt
File Read &amp; Write Challenge 🖋️: Create a program that reads a file and writes a modified version to a new file. Error Handling Lab 🧪: Ask the user for a filename and handle errors if it doesn’t exist or can’t be read
# Open and read the contents of input.txt
with open('input.txt', 'r') as file:
    content = file.read()

# Count the number of words
word_count = len(content.split())

# Convert all text to uppercase
content_upper = content.upper()

# Prepare the output text
output_text = f"{content_upper}\n\nWord Count: {word_count}"

# Write the processed text to output.txt
with open('output.txt', 'w') as file:
    file.write(output_text)

# Print success message
print("Successfully created 'output.txt' with processed text and word count!")
