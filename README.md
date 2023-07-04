# 11-BMI-Calculator
Made a Web Application using the Express framework in Node.js

What we have done : 
1. Importing Required Modules: The code starts by importing the necessary modules, express and body-parser. express is the web application framework, and body-parser is used to parse the request body.
2. Creating an Express App: The code creates an Express application by calling the express() function and assigns it to the app constant.
3. Middleware Setup: The app uses the body-parser middleware to parse the URL-encoded data sent in the request body. It enables extended mode to support complex objects and arrays.
4. Handling GET Request: The code defines a route for handling the GET request to "/bmicalculator". When a user visits this route, the server sends the HTML file "bmiCalculator.html" located in the same directory as the script.
5. Handling POST Request: The code defines a route for handling the POST request to "/bmiCalculator". When the user submits the form data from "bmiCalculator.html", the server extracts the weight and height values from the request body using req.body.
6. BMI Calculation: The server calculates the BMI by dividing the weight (parsed as a float) by the square of the height (also parsed as a float). The calculated BMI is stored in the bmi variable.
7. Sending the Response: The server sends the calculated BMI as a response to the client using res.send(). It constructs a string that includes the BMI value.
8. Starting the Server: The app starts the server on port 3000 by calling app.listen(). The server listens for incoming requests and logs a message to the console when it starts.

-> Overall, this code sets up a server that serves an HTML form for BMI calculation and handles the form submission to calculate the BMI on the server-side. It demonstrates how to handle both GET and POST requests, parse request data, perform calculations, and send responses to the client.
