# HWAssignment-1
Assignment 1

"1."
def fibonacci_series(n):
    fib = [0, 1]
    for i in range(2, n):
        fib.append(fib[i-1] + fib[i-2])
    return fib

# Display the first 10 terms
print(fibonacci_series(10))
"2. 'Display numbers at the odd indices of a list' "
def odd_indices(lst):
    return [lst[i] for i in range(1, len(lst), 2)]

# Example list
numbers = [10, 20, 30, 40, 50, 60]
print(odd_indices(numbers))
"3."
text = """
I have provided this text to provide tips on creating interesting paragraphs.

First, start with a clear topic sentence that introduces the main idea.

Then, support the topic sentence with specific details, examples, and evidence.

Vary the sentence length and structure to keep the reader engaged.

Finally, end with a strong concluding sentence that summarizes the main points.

Remember, practice makes perfect!
"""

def count_unique_words(text):
    words = text.lower().split()  # Convert to lowercase and split into words
    words = [word.strip(".,!?") for word in words]  # Remove punctuation
    return len(set(words))
"4"
print(count_unique_words(text))
def count_vowels(word):
    vowels = "aeiou"
    return sum(1 for char in word.lower() if char in vowels)

# Example usage
print(count_vowels("hello"))  # Output: 2
print(count_vowels("world"))  # Output: 1

"5."

animals = ['tiger', 'elephant', 'monkey', 'zebra', 'panther']

for animal in animals:
    print(animal.upper())
"6"
    for i in range(1, 21):
    if i % 2 == 0:
        print(f"{i} is even")
    else:
        print(f"{i} is odd")

"7. Write a function sum_of_integers(a, b)"        


def sum_of_integers(a, b):
    return a + b

# Example usage
a = int(input("Enter the first integer: "))
b = int(input("Enter the second integer: "))
print(f"The sum is: {sum_of_integers(a, b)}")
