
 a quick demo showing that I know how to use the fetch hook.

 This fetch example returns a random user from randomuser.com



 


1. Inside the fetchData() function's code block, I executed the fetch() function, passing it a single string argument: "https://randomuser.me/api/?results=1".

2. Next, inside the fetchData() function, under the fetch() function call, I added the following piece of code: .then((response) => response.json())

3. then added another then() call, which takes an arrow function.

The passed-in arrow function, receives a data argument, and using that data argument, it invokes the setUser() function, with the data passed to it.

.then((data) => setUser(data));


4. In the return statement of the App component, under the h1 heading that reads “Customer data”,  I added an h2 heading, with the following code: Name: {user.results[0].name.first}

5. then updated the return statement of the App component by adding another line of code under the newly-added h2.

I added an img element, with the src attribute and an alt attribute holding the following code: {user.results[0].picture.large}



This fetch example returns a random user from randomuser.com