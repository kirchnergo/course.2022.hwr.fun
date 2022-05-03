[naming convention]: <> (test_s_yourname19.md) ... e-mail: e_kirchnerg@doz.hwr-berlin.de

## Test - Funktionale Programmierung in F# (2021)

| Name  |  Vorname  |
| ----- | --------- |
| Bitte | Eintragen |

### You define a value in a function using ```let x = 99```. Later you have a line saying ```let x = 100```. What happens?

- [ ] The variable x is assigned a different value of ```100```
- [ ] The value of ```99``` is 'shadowed' and might re-appear if the later definition goes out of scope
- [ ] There is an error because x is immutable
- [ ] A tuple of the form ```(99, 100)``` is created

### What is 'immutability' in relation to programming?

- [ ] The practice of making code as terse as possible
- [ ] The practice of naming values carefully so you don't have to rename them
- [ ] A feature by which values can't be updated once initialized
- [ ] Another word for sealed classes

### You get a compiler error when trying to access a single array element using ```let x = myArray[index]```. What went wrong?

- [ ] You need to use a match statement
- [ ] You need to add a ```.``` before the ```[index]``` - i.e. ```let x = myArray.[index]```
- [ ] You need to access items via the Items property
- [ ] You cannot access array elements individually

### What are the main benefits of coding in immutable style?

- [ ] It allows referential transparency of functions, keeps code simple and helps with threading
- [ ] It makes it easier to save things to a database
- [ ] It improves performance
- [ ] It reduces garbage collection

### How would you define an array whose four values you know at design time?

- [ ] ```let myArray = [1;2;4;9]```
- [ ] ```let myArray = [|1;2;4;9|]```
- [ ] ```let myArray = new Array(){1; 2; 4; 9}```
- [ ] ```let myArray = [|1,2,4,9|]```

### What is the safest and most idiomatic way to access the underlying value of an option type?

- [ ] Use an if statement on the IsNone property then use the Value property in the else branch
- [ ] Use an if statement on the IsSome property then use the Value property
- [ ] Use the Value property directly and handle the exception when there is no value
- [ ] Use a match expression and handle the Some and None cases

### You have defined an F# record type called Position with fields called ```Latitude``` and ```Longitude```. How do you create an instance?

- [ ] ```let myLatLong = 12.4, 45.6```
- [ ] ```let myLatLong = new Position(Latitude=12.4, Longitude=45.6)```
- [ ] ```let myLatLong = Position { Latitude = 12.4; Longitude = 45.6 }```
- [ ] ```let myLatLong = { Latitude = 12.4; Longitude = 45.6 }```

### What happens if you access the Value property of an option type when the instance is None?

- [ ] You will get the zero value that has been specified for the underlying type
- [ ] You will get a compiler error
- [ ] You will get a null reference exception
- [ ] You will get the defined default value

### What is F# Interactive (FSI)?

- [ ] A company promoting F#
- [ ] A way to execute sections of F# code interactively without explicit compilation
- [ ] A console library written in F#
- [ ] A WinForms GUI library written in F#

### You add a new case to an existing DU and start getting compiler warnings around match expressions. What do you do?

- [ ] Add new cases to each of the match statements to handle the new DU case correctly
- [ ] Don’t worry about them - they are only warnings
- [ ] Suppress the warnings using #nowarn
- [ ] Remove the match statements and add if/then to handle each of the cases

### What's the hard part of software development? (Think twice!)

- [ ] Testing
- [ ] Typing
- [ ] Thinking
- [ ] Talking

### What is the purpose of Type-Driven Development?

- [ ] To get rapid feedback
- [ ] To guarantee correctness
- [ ] To ensure that if it compiles, it works
- [ ] To ensure that various user types' needs are met

### Which types don't have structual equality?

- [ ] Records
- [ ] Functions
- [ ] Discriminated unions
- [ ] Tuples
- [ ] Lists

### Is Type-Driven Development just a fancy term for 'if it compiles, it works'?

- [ ] Yes, but a better name is required to sell the idea
- [ ] Yes, but since F#'s type system is stronger, it really does work if you can get it to compile
- [ ] No, it's a way to leverage the type system
- [ ] No, it also works for dynamic languages

### How can you address extra arguments for implementation functions?

- [ ] With Partial Function Application
- [ ] By refactoring to use a Parameter Object
- [ ] By providing anonymous functions
- [ ] By currying

### You have designed a function which returns a tuple with five elements. What's the simplest way to improve readability?

- [ ] Define a record type and use its field names to identify the five elements
- [ ] Add comments to the function saying which value is which
- [ ] Define an OO type with mutable fields to hold the five values
- [ ] Put the five elements in an array, with comments say which value is which

### What form of equality do F# record types implement by default?

- [ ] You must always provide an explicit comparer
- [ ] structural equality
- [ ] Records do not implement equality
- [ ] reference equality

### Which of these options best describes code which 'makes illegal states unrepresentable'?

- [ ] Comprehensive unit test coverage
- [ ] Good OO practices including SOLID
- [ ] Use of DUs, strong typing, strongly typed constructor parameters to prevent invalid data existing
- [ ] Plenty of exception handling for illegal state

### Which of the following statements about the cons operator ```::``` is true?

- [ ] You can use it only to add an element to the head of a list
- [ ] It is the equivalent of ```Seq.zip```
- [ ] You can use it to join two lists
- [ ] You can use it to add an element to the head of the list or to decompose a list into head and tail

### In an array comprehension, how do you create a new element?

- [ ] Using the ```return``` keyword
- [ ] Using the ```<-``` operator
- [ ] No particular keyword - it uses the last value calculated
- [ ] Using the ```yield``` keyword

### An evil genius has stolen the ```Set.isSubset``` function. Using what remains how could you replicate ```Set.isSubset```?

- [ ] ```Set.difference set1 set2 | > Set.isEmpty``` (where ```set1``` is the candidate subset) 
- [ ] ```(Set.union set1 set2     | > Set.count) = 1``` (where ```set1``` is the candidate subset)
- [ ] ```(Set.union set1 set2     | > Set.count) = 0``` (where ```set1``` is the candidate subset)
- [ ] ```Set.union set1 set2      | > Set.isEmpty``` (where ```set1``` is the candidate subset) 

### You want a function like ```Array.fold```, but which creates the initial state from the first array element instead of a parameter. What can you use?

- [ ] You cannot do this in F#
- [ ] Write an explicit loop and use mutability to keep track of the required state
- [ ] Use ```Array.reduce``` instead
- [ ] Use ```Array.iteri``` and a mutable value as an accumulator

### What is Property-Based Testing?

- [ ] A type of testing where you test an object's getters and setters
- [ ] A type of testing where you use huge amounts of random data to discover security issues
- [ ] A type of testing where you describe abstract properties of a function as executable tests
- [ ] State-based testing, where you use an object's properties to inspect its state

### What's a good heuristics for incremental development?

- [ ] Select the next property to add such that it forces you to slightly change the implementation
- [ ] Add all properties you've identified at once, before writing the implementation
- [ ] Add the simplest properties first, saving those more difficult to express until later
- [ ] Use Example-Driven Development

### What's a property in Property-Based Testing?

- [ ] Some sort of real estate, or thing you own
- [ ] A class' properties; esentially getter and setter methods
- [ ] The traits or characteristics of a function
- [ ] F# automatic properties
  
### How do you express a property in Property-Based Testing?

- [ ] Examine the function hierarchy of a composed system
- [ ] You can use built-in language syntax for this, using the ```member``` and ```val``` keywords
- [ ] You can use built-in language syntax for this, using the ```member``` and ```property``` keywords
- [ ] As a function that describes the expected relationship between (unknown, random) input and output
