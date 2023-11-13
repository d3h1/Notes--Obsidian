```
function Circle(radius) {
	this.radius = radius;
	this.draw = function() {
		console.log('Draw');
	}
}

const another = new Circle(1);
```

This Circle function has methods like: 
- bind
- call
- apply

This circle function has properties like: 
- arguments
- caller
- length

> - If you run Circle.constructor --- function() { [native code] } will be shown.
> - This represents an object being made within a function