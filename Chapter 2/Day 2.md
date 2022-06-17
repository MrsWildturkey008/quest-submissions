-----------------------------------------------------------------------------------------------------------------------
## Chapter 2 Day 2

#### 1. Explain why we wouldn't call ```changeGreeting``` in a script.
> We wouldn't call changeGreeting in script because script is to view data, not modify it. Greeting is a function and can only be changed in a transaction.

#### 2. What does the ```AuthAccount``` mean in the ```prepare``` phase of the transaction?
> The AuthAccount allows access to the data in an account. On Flow, accounts store it's own data, but as a user we use AuthAccount to access our data and then we "sign" the transaction. 

#### 3. What is the difference between the ```prepare``` phase and the ```execute``` phase in the transaction?
> The prepare phase is to access information or data in your account, while the execute phase can call actions and can change data on the on the blockchain.

#### 4. Add two new things inside your contract:

##### -A variable named ```myNumber``` that has type ```Int``` (set it to 0 when the contract is deployed)
```cadence 
pub contract HelloWorld {

    pub var greeting: String
    pub var myNumber: Int 

    pub fun changeGreeting(newGreeting: String) {
        self.greeting = newGreeting
    }

    init() {
        self.greeting = "Hello, World!"
        self.myNumber = 0
    }

}
````

##### -A function named ```updateMyNumber``` that takes in a new number named ```newNumber``` as a parameter that has type ```Int``` and updates ```myNumber``` to be ```newNumber```
```cadence 
pub contract HelloWorld {

    pub var greeting: String
    pub var myNumber: Int 

    pub fun changeGreeting(newGreeting: String) {
        self.greeting = newGreeting
    }
    pub fun updateMyNumber(newNumber: Int) {
        self.myNumber = newNumber 
    }

    init() {
        self.greeting = "Hello, World!"
        self.myNumber = 0
    }

}
````

#### -Add a script that reads ```myNumber``` from the contract
````cadence 
import HelloWorld from 0x01

pub fun main(): Int {
    return HelloWorld.myNumber
}
````

#### -Add a transaction that takes in a parameter named ```myNewNumber``` and passes it into the ```updateMyNumber``` function. Verify that your number changed by running the script again.
````cadence 
import HelloWorld from 0x01

transaction(myNewNumber: Int) {

  prepare(signer: AuthAccount) {}

  execute {
    HelloWorld.updateMyNumber(newNumber: myNewNumber)
    }
}
````

<img width="886" alt="Screen Shot 2022-06-16 at 6 05 27 PM" src="https://user-images.githubusercontent.com/106900976/174192426-22e9fd8f-2633-48ec-8221-f8658b2072b5.png">

----------------------------------------------------------------------------------------------------------------------------------
