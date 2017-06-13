## Scope, hoisting and compartmentalization

### Answer the following:
In you own words, explain the concepts of scope, hoisting, compartmentalization.

scope is either globe or local , if a variable is declared inside of a function its local if its outside is

globe. hoisting is how javascript declaration moved to the top of its scope.  compartmentalized is writing code that doesn't mess with global codes overriding usually with bigger projects.

### Provide examples for all three, below:


#### Scope:// code here can not use carName

function myFunction() {

    var myName = "Mateen";

    // local used only inside

}

var myName = "Mateen"

// global can be used anywhere


#### Hoisting:

function myFunction() {

    var myName = "Mateen";  // hoisted variable read first if the console was before myName would be undefined.

    console.log(myName)

}

myFunction();


#### Compartmentalization:

var date = new Date(1983, 3, 21);
var birthday = date;

var bdayMsg = function(){
  return "You were born on " + date.toDateString();
};
bdayMsg();
