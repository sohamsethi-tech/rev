let arr=[1,2,3,4,5];
let ans=arr.map((n)=>{ isme teri 2 brackets aati h pehle to arrow function wali doosri teri tu kuch bhi var assign kr skta h seedhi baat 
return n*2 yaha tera kya aayega jo bhi tune krna h usko return bhi karega na chutiye
});
// ye h map ka kaam bc bas

////////////////////////////////////////////////////////////////////////////////////

aab aaja filter per 
filter me kya h condition ke basis per return hota h 
let arr=[1,2,3,4,5,6,7,8,9];
let res=arr.filter((a)=>{
    return a>=2;
});
console.log(res);
////////////////////////////////////////////////////////////////////////////////////

aab aaja reduce per 
let arr=[1,2,3,4,5];
let ans=arr.reduce((total,current)=>{
return total+current
},0) ye jo tune diya h na 0 vo tune initiallize hi kari h total ki value samjhgya na aur jo tera current h vo to point hi current value per kar raha h

Concept	React	React Native
JavaScript	Same	Same
Components	Same concept	Same concept
Props	Same	Same
useState	Same	Same
useEffect	Same	Same
useContext	Same	Same
Custom Hooks	Same	Same
API integration	Same concepts	Same concepts ye sab same h react aur react native ye to terko pta hi h 

/////////////////////////////////////////////////////////////////////////////////////////

aab aaja kya diff h usper bhai mere simple h theek h jese react me tera kya hota h container <div> hota h react native me container hota h <View> aab text react me <p> <span> <h1-8> aur ye hi react native me hota h <Text> ,, react me button simple <button> se hota h react native me tera <Pressable> ke naam se hota h 

/////////////////////////

aab badhta hu aage react per aaja bc 
react me tu jsx kya hota h jsx javascript + xml hota h ye mtlb html aur js support kr deta h react me aur agar jsx ni lagana to iska aata h 

import React from "react";

function App() {
    return React.createElement(
        "h1",
        null,
        "Hello Soham!"
    );
}

export default App;
ese code createElemt se create hota h
aab jsx me js likhte kese h kuch ni {} curly braces lagadi jaha tune wah teri js hogi 

////////////////////
like
function App(){
    const name="Soham Sethi";
    const age= 19;
    return (
        <div>
            <h1>Hello {name}</h1> yaha se aayega Hello Soham Sethi
            <p>My age is {age}</p>  
            <p>Next year I will be {age + 1}</p>
        </div>
    );
}

export default App;


rule in jsx me html me tera kya hota h <div class="container"></div>  theek h ye tera hota h html me aab tera react me hoga <div className="container"></div> bas kuch ni className lagate h hum className="container" kyu likhte hain?
Taaki hum CSS ke through us particular div ko style kar sakein theek h samjhaaa
/////////

aab aa jate h components wagrah per 

component ek reusable peice of ui hota h jise hum baar baar use kr skte h

ek website banani h humne theek h aab tune components ka kaam dekh

function App(){
    return(
        <div>
         <h1>Shoes</h1>
            <p>Price: ₹2000</p>

            <h1>Watch</h1>
            <p>Price: ₹3000</p>

            <h1>Phone</h1>
            <p>Price: ₹20000</p>
        </div>
    )
}


aab ye to teri kya ho gyi simple declatrion tune har object uthaya ek ek krke likha bc ye to bahot lamba ho jayega

iske liye with components dekh aab:
function hi(){
    return(
        h2>Product Name</h2>
            <p>Product Price</p>
        </div>
    )
}
function hey(){
    return(
        <div>
        <hi>
        <hi> aab idhar hi tera product card ban jayega theek h na samjh gya 
        <hi>
         </div>
    )
}
aaaab tune agar import krna h function koi to kya karega like
import Navbar from "./components/Navbar";
import Footer from "./components/Footer";
function hi(){
    return(
        <Navbar />
        aur fir ese hi aayega <Footer /> bhi

    )
}
///parent aur child ka system soda dekhte h aab
function Child(){
    return <h2>I m Soham Sethi</h2>

}
function Parent(){
    return(
        <h1>I m Dinesh Sethi </h1>
        <Child />
    )
}

what does export default do?
=> default export provide krta h
component composition means multiple components combine krna

props ke hota h parent se data recieve krna aab isko practically dekhte h
===>State kya hoti hai?
.......State ek aisa data hai jo component ke andar store hota hai aur change hone par UI ko update karta hai

import {useState} from "react"
function App(){ /// ye tera component h 
    const [count,setCount]=useState(0);  /////// yaha tera count kya hoga current state value hogi aur setCount kya hoga tera state update krne wala function theek hh
    return(
        <>
        <h1>Count:{count}</h1>
        <button onClick={()=>{
            setCount{count+1}
        }>
        Increase
        </button>
        </>
    )

}
function handleClick(){
    handleClick() is the function that executes when the event occurs.



onClick is the event handler.



{handleClick} passes the function to React.
}

function App(){
    const[count,setCount]=useState(0);

    function handleClick(){
        setCount(count+1);
    }
    return (
    <div>
      <h1>{count}</h1>

      <button onClick={handleClick}>
        Increase
      </button>
    </div>
  );
}

function handleClick(){
    alert("hi");
}
<button onClick=()=>{
handleClick
}> hi  </button>


///// 

conditional rendering means displaying different ui elements depending on the condition .....


function App(){
    const isLoggedIn=true;
    if(isLoggedIn){
        ///what u waanna return u can like return( whatever u wwannna write here)
    }
}


function App(){
    const isLogIn=true;
    return(
        <>
        {isLogIn?<h1>Dashboard</h1>:<h1>Login </h1>}
        </>
    )
}

function App() {

  const students = [
    { id: 1, name: "Soham", age: 20 },
    { id: 2, name: "Rahul", age: 21 },
    { id: 3, name: "Aman", age: 22 }
  ];

  return (
    <div>
      {students.map((student) => (
        <div key={student.id}>
          <h2>{student.name}</h2>
          <p>{student.age}</p>
        </div>
      ))}
    </div>
  );
}

export default App;     //// see this code




