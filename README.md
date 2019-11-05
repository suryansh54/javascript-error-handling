# Javascript Error Handling




##### Point
If any error causes in the code, Code execution block at that particular line where the error cause (Example 1). if you do not want to stop execution you can use try, catch block (Example 2), In example 2 Hello world print means the execution of code is not stop.

**Example 1**
```javascript
function func(){
	const x = "Hello ";
	const y = "World";
	const xy = function(){
		const z = "Hi";
		return x + y;
	}
  console.log("Error", z);
	return xy();
}
// Error ReferenceError: z is not defined
//  at func (<anonymous>:9:32)
//  at <anonymous>:1:1
```

**Example 2**
```javascript
function func(){
	const x = "Hello ";
	const y = "World";
	const xy = function(){
		const z = "Hi";
		return x + y;
	}
  try {
      console.log("Success", z);
  } catch(err) {
      console.log("Error", err);
  }
	return xy();
}

// Error ReferenceError: z is not defined
//  at func (<anonymous>:9:32)
//  at <anonymous>:1:1
// "Hello World"
```

###### References 
- https://www.w3schools.com/js/js_errors.asp
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling
- https://www.geeksforgeeks.org/javascript-error-and-exceptional-handling-with-examples
- https://www.tutorialspoint.com/javascript/javascript_error_handling.htm
- https://medium.com/@iaincollins/error-handling-in-javascript-a6172ccdf9af
- https://javascript.info/try-catch
