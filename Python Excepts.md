```python
print('Please give me 2 numbers and I will divide them.')
print('Enter "q" to quit.\n')

while True:
    first_number = input('First Number: ')
    if first_number == 'q':
        break

    second_number = input('Second Number: ')
    if second_number == 'q':
        break

    try:
        answer = int(first_number) / int(second_number)
    except ZeroDivisionError:
        print('You can\'t divide by zero! Let\'s start again.')
    else:
        print('Your answer is: ' + str(answer))
        print('Give me another!\n')

print('Ok, bye!')

```
^^
In the above case it must be ZeroDivisionError as that is the error that python gives when the code is run without the except