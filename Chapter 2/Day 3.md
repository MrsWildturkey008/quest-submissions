## Chapter 2 Day 3

#### 1. In a script, initialize an array (that has length == 3) of your favourite people, represented as ````String````s, and ````log```` it.
````cadence
pub fun main() {

  var people: [String] = ["WildTurkey008", "JennaMarie", "BeccaVousAime"]
  log(people)
}
````

#### 2. In a script, initialize a dictionary that maps the ````String````s Facebook, Instagram, Twitter, YouTube, Reddit, and LinkedIn to a ````UInt64```` that represents the order in which you use them from most to least. For example, YouTube --> 1, Reddit --> 2, etc. If you've never used one before, map it to 0!
````cadence
pub fun main() {

  var social: {String:UInt64} = {"Facebook": 1, "Instagram": 3, "Twitter": 2, "YouTube": 4, "Reddit": 5, "LinkedIn": 0}
  log(social)

}
````

#### 3. Explain what the force unwrap operator ````!```` does, with an example different from the one I showed you (you can just change the type).

#### 4. Using this picture below, explain...

> What the error message means:
> 
> Why we're getting this error:
> 
> How to fix it:
