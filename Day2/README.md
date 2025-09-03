Encapsulation : bundling of data(property) and methods(functions) that operate on that data into a single unit, or object. data hinding restricts the direct access.

class User{
//initialise object <br/>
    constructor(name, email){ <br/>
    this.name = name; <br/>
    this.email = email; <br/>
    //we can have private properties using a hash <br/>
    this.#password = '12345'; <br/>
    } <br/>
    greet(){ <br/>
    console.log(`Hello my name is ${this.name}! `); <br/>
    } <br/>
    } <br/>
  //create object of user class <br/>
  const newUser = new User('Alice', 'alice@gmail.com') <br/>
  console.log(newUser.name) // output Alice <br/>
  newUser.greet() // output - Hello my name is Alice
    

