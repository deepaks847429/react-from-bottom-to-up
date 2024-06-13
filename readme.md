React is a javascript library for building user interface.

History of react

React originally created by jordan walke.
initial version was launched in 2013
maintained by meta and a community of developers.
current version of react is v18.

Why React?

react is composable(component based, everything can be designed seperately, code resuablity). example-> airbnb.

React helps creating single page application efficiently.(1 html page, high performance, )


singale page application vs multipage page appliaction.

multipage appliaction is a traditional implementation of web appliaction which reloads the whole page when a user interacts with the app.

single page application is a web application which loads a single document and updates the part of document using javascript apis (AJAX).

amazon follows mpa for search engine optimization.

inspect->network->doc->preserve log.

React is a declarative language(Tell  u what u want to do, not how to do) where js is imperative language.

const header=(<div>
<h1 className="header">Hello</h1>
<p>Welcome to the session</p>
<button className="btn">Click</button>
</div>);


ReactDOM.createRoot(document.getElementById("root")).render(header);


Virtual DOM Key Concepts :
Virtual DOM is the virtual representation of Real DOM
React update the state changes in Virtual DOM first and then it syncs with Real DOM
Virtual DOM is just like a blueprint of a machine, can do changes in the blueprint but those changes will not directly apply to the machine.
Virtual DOM is a programming concept where a virtual representation of a UI is kept in memory synced with “Real DOM ” by a library such as ReactDOM and this process is called reconciliation
Virtual DOM makes the performance faster, not because the processing itself is done in less time. The reason is the amount of changed information – rather than wasting time on updating the entire page, you can dissect it into small elements and interactions

writing code in JSX


REact fragments


React components
->functional components
->class based components

Functional components
(rule says that it should be name with capital letter)

function App(){
return (
  <>
  <h1>Hello JSX</h1>
  </>
)
}

ReactDOM.createRoot(document.getElementById("root")).render(<App />); 


functional component using arrow function
(implicitely returns)
(length of code decreases)

const App=()=>{
return (
  <>
  <h1>Hello JSX</h1>
  </>
)
}

DAy -2

Introduction to jsx

javascript XML is a syntax extension to javascript.

WHY JSX?

React embraces the fact that rendering logic should be coupled with UI logic.
Helpful as a visual aid when working with UI inside javascript.
React seprates concerns instead of seprating technologies.
It also allows React to show more useful errors and warning messages.

Embedding javascript inside JSX

Expressions in JSX


Rendering Arrays and Objects

{arr.map((num)=> <h2>{num}</h2>)}





score keeper app
let score=0;
let wicket=0;

let ballwiseresult=[];

function addOne(){
  score+=1;
  rootElement.render(<App />)
}
function addTwo(){
  score+=2;
  rootElement.render(<App />)
}

function addScore(num){
  score+=num;
  rootElement.render(<App />)
}

function addWicket(){
  if(wicket<11){
  wicket+=1;
  rootElement.render(<App />);
}}
const App=()=>(
  <>
  <h1> Score keeper</h1>
  <h1>score : {score}/{wicket}</h1>

  <button onClick={addOne}>1</button>
  <button onClick={addTwo}>2</button>
  <button onClick={() =>addScore(3)}>3</button>
  <button onClick={() =>addScore(3)}>4</button>
  <button onClick={() =>addScore(3)}>5</button>
  <button onClick={() =>addScore(3)}>6</button>
  <button>wicket</button>
  </>
)
const rootElement = ReactDOM.createRoot(document.getElementById("root"));
rootElement.render(<App />)

















create react app

for creating use-create-react-app

for start -use npm start command.




import/export

export

Named export(anything and everything)
->export individually
export let a=10;
import a from "./app"
->export at the bottom


default export(one thing)

React components

->functional components
->class based components




















 





















