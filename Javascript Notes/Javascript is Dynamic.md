- Objects in JS are dynamic. Once created, you can always add or remove
	- Properties
	- Methods

```
const circle = {
	radius: 1,
}

circle.color = 'yellow'

delete circle.color
```

ex: As shown as above, we can add the string 'yellow' to this object and later remove it
> As it is a CONST, we cannot reset circle to a new object, we can simply add | remove it's contents