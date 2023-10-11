# Functions

### Functions allow for things like

- Modularity : Breaks tasks into pieces
- Reusability : Use code multiple times
- Abstraction : Hide implementation details
- Debugging : Isolate and Fix issues
- Namespacing : Localizes varaible scope
- Parameterization : Versatile and differnet inputs
- Encapsulation: Hide complex structuring
- Organization Logical code structuring
- Collaboration : Team members work independetly with ease
- Extendability : Easy to modify and expand 

### Some Examples of Advanced Topics
> Abstraction : 
    

    def add(a, b): 
            return a + b 
    
    result = add(3,  4)
This shows how the user does not need to know how add works, they can simply use the function and keep working. 

>Encapsulation

    class BankAccount:
        def __init__(self):
            self.__balance = 0 # Private attribute

        def deposit(self, amount):
            if amount > 0:
                self.__balance += amount
                return True
            return False

        def withdraw(self, amount):
            if amount < 0:
                self.__balance -= amount
                return True
            return False
        
        def getDeposit(self):
            return self.__balance
    
    # Use the class now
    account = BankAccount() # init
    account.deposit(100)
    account.withdraw(50)
    print(account.getDeposit())

    # 50 PRINTS OUT

The methods inside of class can be seen as a basic form of encapsulation. The way we also create balance as a private attribute that cannot be affected outside of its methods is another way of encapsulation  

## Two Categories of Functions
### User-Defined Functions
> Functions written by users
### Built-in Functions
> Functions that are built into Python

## Scope
When accessing a variable, Python checsk these scopes in this order 
1. Local
2. Enclosing
3. Global
4. Built-in

### Understanding The Scopes
1. Local Scope
> This refers to variables defined within a function. These can only be accessed inside the function

2. Enclosing (Non-Local) Scope
> This refers to a function inside antoher function. Varibales in an enclosing scope can be accessed from the inner function but to modify them, THE "nonlocal" KEYWORD is needed

3. Global Scope
> This refers to varaibles defined at the top level of a script. These varaibles can be accessed from anywhere by anything. Usually a global keyword 

4. Built-in Scope
> This refers to names that are built into python. This can be print() or len(). Always available regardless of need