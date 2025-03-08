///let username = prompt("Enter your username:");
let password = prompt("Enter your password:");

if (username && password) {
    let correctPassword = "your_password";
    for (let i = 0; i < 3; i++) {
        if (password === correctPassword) {
            alert("Welcome ${username}');
            break;
        } else {
            alert("Maybe Username or Password is Invalid or Does not Match");
            password = prompt("Please enter your password again:");
        }
    }
}///

///const items = {
    A: { name: "Pepsi Cola", price: 1.5 },
    B: { name: "Coca Cola", price: 1.5 },
    C: { name: "Apple", price: 3.0 },
    D: { name: "Orange", price: 2.5 },
    E: { name: "Hotdogs", price: 5.0 }
};

let choices = "A. Pepsi Cola\nB. Coca Cola\nC. Apple (per kg)\nD. Orange (per kg)\nE. Hotdogs (per kg)";
alert(choices);

let itemChoice = prompt("Enter your item choice (A, B, C, D, or E):");
let quantity = prompt("Enter the quantity to be ordered:");

let totalPrice = 0

switch (itemChoice.toUppercase()) {
    case 'A':
    case 'B':
    case 'C':
    case 'D':
    case 'E':
        totalPrice = items[itemChoice.toUppercase()].price * quantity;
        alert('The Total Price of the order ${items[itemChoice.toUppercase()].name} x ${quantity}: $${totalPrice}'):
            break;
     default:
         alert("No matching Item! Try to re-run the program."
}///

///let createMatrix = prompt("Do you want to create a Matrix? (yes/no)");

if (createMatrix.toLowerCase() === "yes") {
    let limits = [];
    for (let i = 0; i < 3; i++) {
        limits.push(parseInt(prompt('Enter limit for loop ${i + 1}:')));
    }
    
   /// let strings = [];
    for (let i = 0; i < 3; i++) {
        strings.push(prompt('Enter string for loop ${i + 1} (word, char, number, symbol):'));
    } ///
    
   /// for (let i = 0; i < limits[0]; i++) {
        for (let j = 0; j < limits[1]; j++) {
            for (let k = 0; k < limits[3]; k++) {
                console.log('${strings[0]} ${strings[1]} ${strings[2]}');
            }
        }
    } ///
} else {
    console.log("Thank you, re-run the program if you change your mind.");
}///
