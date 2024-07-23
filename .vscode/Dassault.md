Dassault Sysytems

1.  Find index of min element input = [-1,2,5,-8,4] output=3
2.  Create new array of elements less than zero input = [-1,2,5,-8,4] output=[-1,-8]
3.  Fetch data using https://dog.ceo/api/breeds/list/all this api and print any value. Using async/await and promise both.
4.  function a() {
    var x = 5;
    let y = 7;

    console.log(this.x);
    console.log(this.y);
    }

    a();
    Guesse the output of above code.
    Output = undefined for both the consoles as 'this' referes to a global object. But there is no x and y in the global object as there are declared inside the function so it will give 'undefined'.

5.  var a = 5
    let b = 7
    function x() {
    function y() {
    console.log(a);
    console.log(b);
    }
    y()
    }
    x()
    Guess the output. => 5 and 7 both will be printed because of scope chaining and closure.

6.  var a = 5
    let b = 7
    function x() {
    function y() {
    setTimeout(() => {
    console.log(a);
    console.log(b);
    }, 0);
    console.log("here");
    }
    y()
    }
    x()

    What will be the sequece of output and why.
    ans => "here"
    5
    7
    Because setTimeout is browser provided method browser will regester the call back function in setTimeout also the timer and js engine will execute next line in call stack by creating execution context. Once timer is expired then the call back function will be pushed into call back queue first then event loop will check if call stack is empty then call back function will be pushed in the call stack and will be executed.

7.  Design patterns
8.  Solid principles

9.  <div class="C" id="I">Div</div>
    div { 
    color: red;
    }
    #I { 
    color: blue;
    }
    .C { 
    color: grey;
    }

    Which color will be applied? Ans => As id has highest priority blue color will be applied.
