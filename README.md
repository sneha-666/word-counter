def count_words(text):
    """
    Counts the number of words in the given text.
    
    Parameters:
    text (str): The input text to count words from.
    
    Returns:
    int: The number of words in the text.
    """
    # Split the text into words based on whitespace and filter out empty strings
    words = text.split()
    return len(words)

def main():
    """
    Main function to run the Word Counter program.
    """
    print("Welcome to the Word Counter!")
    
    # Prompt the user to enter a sentence or paragraph
    user_input = input("Please enter a sentence or paragraph: ")
    
    # Check for empty input
    if not user_input.strip():
        print("Error: You entered an empty input. Please provide a valid sentence or paragraph.")
        return
    
    # Count the words using the count_words function
    word_count = count_words(user_input)
    
    # Display the word count
    print(f"The number of words in your input is: {word_count}")

# Entry point of the program
if __name__ == "__main__":
    main()
