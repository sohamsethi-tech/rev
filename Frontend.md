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
