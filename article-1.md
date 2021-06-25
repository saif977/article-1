# EVENT LOOP , SYNCHRONOUS AND ASYNCHRONOUS IN JAVASCRIPT FOR BEGINNERS

 "Before all this let us know first, wether javascript is a single-threaded or multi-threaded language ?" Now first of all let us know what is a single-threaded and multi-threaded language is.We will keep things very simple, we will not dive deepEVENT LOOP , SYNCHRONOUS AND ASYNCHRONOUS IN JAVASCRIPT FOR BEGINNERS into this. So a single threaded language means only one thing can run at a particular point of time and vice-versa for multi-threaded language that means it can run parallel things at a particular point of time. Now coming to the point, <mark style="background-color: white ; opacity:.5">javascript is a single-threaded programming language </mark> . But you should be wondering why people say that javascript act as a multi-threaded language. The answer to this question is its `asynchronous` thing.
 </br>
 </br>
 We had covered a lot of theory, Now lets dive into some code to uderstand what is `synchronous` and `asynchronous` thing in javascript.  
 </br>

  ### Code snippet to show synchronous javascript : 
  </br>

```javascript
console.log("1st output"); //statement-1

let bool = true;
for(let i=0;i<10000;++i){    //statement-2
    if(boolValue)
    {
        console.log("executing for loop");
        boolValue=false;
    }
}

console.log("2nd output"); //statement-3
 ``` 
 <br>

   ### Output : 

 <br>  
  <img src="https://gifyu.com/image/AK0E">
<br/><br/>

 Now lets understand the output, 
1. We know that javascript files are parsed from top to bottom. So at first `statement-1` will execute and prints <b>"1st output"</b>. 
2. After this, the `statement-2` is executed and prints <b>"executing for loop"</b> and javascript waits until the `forloop` completes its iterations. And once it exits out of the loop, it will now execute `statement-3` and prints <b>"2nd output"</b>.  

<br/>

>* So my friends, you just came across the `synchronous` thing. The waiting of the javascript to complete the <b>for loop</b> iterations and then executing the `statement-3` is a synchronous thing.<br>
>* We know that javascript is single-threaded. Because of this when javascript executes `statement-2` it waites for the completion of the current statement, Once it is completed then javascript moves to `statement-3` and executes it. <br>
>* `Synchronous` code simply means that <b>"Not moving to the next statement unless and until the current statement is executed completely".</b>  

<br>
