# Unit Conversion

The goal is to write a small python terminal program that takes in a measurement
with a unit, converts it to metric and prints it out.

## Reading User Input

For our program to work, we have to be able to read user input. We should also
present the user with a short introduction asking him to enter something or he
won't know what to do. It might look something like this


> Please enter a measurement (eg. '1 in', '23 gal')

> 24 ft

At the end of this, we should have the string `"24 ft"` in our program. Feel
free to come up with better messages for the user.

### References

- https://docs.python.org/3.5/library/functions.html#print
- https://docs.python.org/3/library/functions.html#input

## Making Sense of User Input

We now have to understand what the user gave us. To be able to do anything with
the input, we have to separate the number from the units. For now, it's useful
to say that there should always be a space in between the number and the units.

> Please enter a measurement (eg. '1 in', '23 gal')

> 24 ft

After our understanding, we should have the python number `24` and the string
`"ft"`.

We should also correctly handle incorrect output:

> Please enter a measurement (eg. '1 in', '23 gal')

> Where am I?

> Please use the format "## unit" where ## is a number and unit is an imperial
> unit. Make sure to include a space.

As always, feel free to have better messages.

### References

- https://docs.python.org/3/library/stdtypes.html#string-methods
- https://docs.python.org/3/library/functions.html#int

## Unit Conversion

We now have to take the imperial unit the user gave us and convert it into a
sane measurement system. To do this, we have to multiply (we can skip
temperature units and the adding for now) it by a factor.

> Hint: A nice way to go about this would be to use a python dictionary. You
> would give this dictionary an imperial unit and it would return its equivalent
> metric unit and scaling factor. You could then carry out the multiplication
> and print out the resulting number with the new unit.

### References

- https://docs.python.org/3/tutorial/datastructures.html#dictionaries
- https://en.wikipedia.org/wiki/Imperial_units#Units
