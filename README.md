# Javascript-for-react

// If you want to export it in another file you can do it by typing export default in start 
// syntax : export default function DoSomething () {
                //   your code here
// }

function DoSomething () {

}

// If you want to export it in another file you can do it by typing export in start 
// syntax : export const DoSomething = () => {
                //   your code here
// }

const Do = () => {

}

//  We will be using arrow function mostly as it is the same in react 

// in react we make a function like this :

// const DoSomething = () => {
    //  return (
        // <div></div>
    // );
// }

//  Anonymus function

<button 
    onClick = { () =>  {console.log("Hello World");
    }}>
</button>

// terniory operater  &&  ,  ||   used as if else statement where && is used for true and || is used for false.   
// ? for if true statement like in line 41.
// : for else.

let age = 10;
let name = age > 10 ? "Pedro" : "Jack";

//  Example :

const Example = () => {
    return age > 10 ? <div> "Pedro" </div> : <div> "Jack" </div>
}

//  Objects

// const name = "Pedro";
// const age = 20;

const person1 = {
    name : "Pedro",
    age : 20,
    ismarried : false,
};

// const { name , age , isMarried } = person;

const person2 = {...person, name : "Jack"}
// now person2's all properties expect his name is similer to person1

// map , filter , reduce

let names = ["Pedro" , "Joel" , "Stacy" , "Pedro" , "Pedro"]

names.map((name) => {
    // The code written here will be executing in each element in the array
    // example : return name + "1";
    return <h1> {name} </h1>
})

names.filter((name) => {
    return name !== "Pedro"
})

// it will make array like [Joel , Stacy]

// What is DOM?
/* https://www.geeksforgeeks.org/reactjs-reactdom/ */

// How to import and export

// for a library named axios

const axios = require('axios')     // in react : import axios from "axios";

module.exports = { anObject };     // in react : export {anObject}

//  Optional Chaining

const fetchData =  async () => {
    const data = await fetch("imaginaryapi.com");
    const name = data.person?.name;
};
