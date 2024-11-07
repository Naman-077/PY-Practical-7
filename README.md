# PY-Practical-7
def occurrences(a, b):
    indices = []
    i = 0
    while i < len(a):
        c = a.find(b, i)
        if c == -1:
            break
        indices.append(c)
        i = c + 1  # Move forward to the next possible starting position
    return indices if indices else -1

# Input from the user
a = input("Enter the first string: ")
b = input("Enter the second string: ")

# Function call and output
result = occurrences(a, b)
print(result)


'''output
Enter the first string: hello world
Enter the second string: hello
[0]
'''
