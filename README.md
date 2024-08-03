# palindrome
def is_palindrome(text):
    # Remove spaces and convert to lowercase for a case-insensitive comparison
    cleaned_text = ''.join(text.split()).lower()
    return cleaned_text == cleaned_text[::-1]

# Get input from the user
user_input = input("Enter text to check if it's a palindrome: ")
if is_palindrome(user_input):
    print("The text is a palindrome!")
else:
    print("The text is not a palindrome.")
