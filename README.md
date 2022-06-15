# Quest-Submissions

## Chapter 1 Day 1

#### 1. Explain what the Blockchain is in your own words.
> Blockchain is an open database that stores its information into chunks/blocks. These blocks then builds upon itself and are linked together like a chain. Anyone can interact and view the data. No single person owns or controls blockchain. Once you have submitted the information on blockchain it is usually irreversible and difficult to change or hack.

#### 2. Explain what a Smart Contract is.
> A Smart Contract is a specific set of rules that people can interact with. Smart contracts are extremely secure and fast due to not having to wait to get approval from a middle-man.

#### 3. Explain the difference between a script and a transaction.
> The differences between script and a transaction are the cost and how it's being used. Script is used to view data on the blockchain and it's free, while transaction changes the data on the blockchain and costs money.

-----------------------------------------------------------------------------------------------------------------------

## Chapter 1 Day 2

#### 1. What are the 5 Cadence Programming Language Pillars?
> The 5 Cadence Programming Language Pillars are safety and security, clarity, approachability, developer experience and resource oriented programming.

#### 2. In your opinion, even without knowing anything about the Blockchain or coding, why could the 5 Pillars be useful?
> Safety & Security: People are looking for safety because if they invest their money. Knowing your investment would be safe would draw more users in.

> Clarity: Clarity is extremely important because people want clear and concise instructions. People don't want to jump through hoops or waste time having to figure out the process. The longer it takes to try and comprehend something, the easier it is for people to give up. Make it easy to understand will draw more users in.

> Approachability: This is important for wanting to draw people/developers in.

> Developer Experience: Developer Experience is important because it allows your developers to find their problems in a timely manner and not have to waste timing reviewing code that's correct. Having things that are easy to use can draw in more developers.

----------------------------------------------------------------------------------------------------------------------
## Chapter 1.5

> #### https://play.onflow.org/beafe918-9cb0-49a2-bb5f-45e9c4cc2099?type=script&id=8fc4c6ba-c555-432f-adeb-ffc72c3bffad&storage=none
 
-----------------------------------------------------------------------------------------------------------------------
## Chapter 2 Day 1

#### 1. Deploy a contract to account 0x03 called "JacobTucker". Inside that contract, declare a constant variable named is, and make it have type String. Initialize it to "the best" when your contract gets deployed.
> <img width="1050" alt="Screen Shot 2022-06-10 at 10 58 19 AM" src="https://user-images.githubusercontent.com/106900976/173105306-682fdd11-8209-4a4b-81ce-e334e049f4e9.png">

#### 2. Check that your variable is actually equals "the best" by executing a script to read that variable. Include a screenshot of the output.
> <img width="839" alt="Screen Shot 2022-06-10 at 11 06 26 AM" src="https://user-images.githubusercontent.com/106900976/173106758-1191c05b-b09c-492f-99e9-84d8a0b75256.png">

-----------------------------------------------------------------------------------------------------------------------
## Chapter 2 Day 2

#### 1. Explain why we wouldn't call ```changeGreeting``` in a script.
> We wouldn't call changeGreeting in script because script is to view data, not modify it. Greeting is a function and can only be changed in a transaction.

#### 2. What does the ```AuthAccount``` mean in the ```prepare``` phase of the transaction?
> The AuthAccount allows access to the data in an account. On Flow, accounts store it's own data, but as a user we use AuthAccount to access our data and then we "sign" the transaction. 

#### 3. What is the difference between the ```prepare``` phase and the ```execute``` phase in the transaction?


#### 4. Add two new things inside your contract:


##### -A variable named ```myNumber``` that has type ```Int``` (set it to 0 when the contract is deployed)


##### -A function named ```updateMyNumber``` that takes in a new number named ```newNumber``` as a parameter that has type ```Int``` and updates ```myNumber``` to be ```newNumber```


#### -Add a script that reads ```myNumber``` from the contract


#### -Add a transaction that takes in a parameter named ```myNewNumber``` and passes it into the ```updateMyNumber``` function. Verify that your number changed by running the script again.


----------------------------------------------------------------------------------------------------------------------------------
```cadence

```
