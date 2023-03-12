# Automate as much as you can

## Preface
There was a story about Bill Gates back in the day. He prefer a programmer with a lazy personality over a hard working one because the lazy coder will try to do their job with the least amount of effort while achieving the same result. 

Working smart is all about finding ways to be efficient and effective with your time, rather than just working hard and putting in long hours. In Python, there are many ways to work smart, and here's a simple example:

## Example

Suppose you have a list of numbers and you want to find the sum of all the even numbers in the list. One way to do this would be to iterate over the list, check each number to see if it's even, and add it to a running total if it is. Here's some code that would do that:

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
total = 0
for num in numbers:
    if num % 2 == 0:
        total += num
print(total)
```

This code works fine, but it's not particularly efficient. It requires iterating over the entire list, even though we only care about the even numbers. A smarter way to do this would be to use a list comprehension to create a new list containing only the even numbers, and then find the sum of that list. Here's the updated code:

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_numbers = [num for num in numbers if num % 2 == 0]
total = sum(even_numbers)
print(total)
```

This code uses a list comprehension to create a new list that only contains the even numbers from the original list. It then uses the built-in sum function to find the sum of that list. This approach is much more efficient, as it avoids iterating over the entire list and only considers the even numbers.

This is just a simple example, but it illustrates the importance of working smart in Python. By using built-in functions, list comprehensions, and other Python features, you can write code that is more efficient, more readable, and easier to maintain. By taking the time to learn these techniques and apply them to your code, you can work smarter instead of harder, and get more done in less time.