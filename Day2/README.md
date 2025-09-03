Encapsulation : bundling of data(property) and methods(functions) that operate on that data into a single unit, or object. data hinding restricts the direct access.

class User{
//initialise object
    constructor(name, email){
    this.name = name;
    this.email = email;
    //we can have private properties using a hash
    this.#password = '12345';
    }
    greet(){
    console.log(`Hello my name is ${this.name}! `);
    }
    }
  //create object of user class
  const newUser = new User('Alice', 'alice@gmail.com')
  console.log(newUser.name) // output Alice
  newUser.greet() // output - Hello my name is Alice
    
