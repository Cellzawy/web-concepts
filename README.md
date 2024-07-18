##  RESTful API

This guide will get you started with RESTful APIs

### Table of Contents

* [What is a RESTful API?](#what-is-a-restful-api)
* [Installation](#why-do-we-need-restful-apis)
* [Principles of RESTful API](#principles-of-restful-api)
* [License](#license)





### What is a RESTful API?
`REST` here stands for **RE**presentational **S**tate **T**ransfer. It's an architectural style which follows some rules to create web apps/services

Imagine a restaurant:

**Client (You)**: You are the customer who wants food. You (the client) initiate a request by telling the waiter (the server) what you want (your request).

**Server (Waiter)**: The waiter takes your order (processes your request) and goes to the kitchen (communicates with the database or other resources).
**Response:** The waiter brings you your food (delivers the response) based on your request.

***In the digital world:***

**Client (Software):** A client application (like a web browser or mobile app) acts on your behalf to request information or perform actions.

**Server (Computer):** A server computer stores data and runs programs that respond to client requests. It can access databases, perform calculations, or control hardware.

REST suggests to create an object of the data requested by the client, then send the values of that object to the client.

So, you have an object and you are sending the **state** of an object. This is why REST is known as Representational **State** Transfer.





### Why do we need RESTful APIs?

Imagine you're checking the weather on your phone using a weather app.

**Client (Weather App)**: The app acts as your personal weather assistant, requesting information from a server.
**Server (Weather Data Provider)**: A massive computer system stores and processes weather data from various sources (satellites, weather stations).

**Behind the scenes:**

The weather app (client) uses an API (Application Programming Interface) to talk to the weather server.
The API acts as a translator, allowing the app to send clear requests and understand the server's responses.
***Traditionally, servers might have sent entire webpages as responses.***

Imagine the weather app receiving a **whole webpage** just to display the current temperature!
This is inefficient and cumbersome for the app to process.

**Structured Data Formats: JSON to the rescue**

Modern weather APIs use JSON (JavaScript Object Notation) for data exchange.
JSON makes it much easier for the weather app to understand and display the relevant information.
But there's more to weather data than just temperature.

What if you want a 5-day forecast or specific weather conditions for your location?
Here's where REST APIs come in.

**REST APIs: Modular Data Access for Weather Apps**

REST APIs provide a modular approach to accessing weather data. Instead of one big request, the app can make smaller, focused requests using HTTP methods (GET, POST):

GET: "Hey server, give me the current temperature for Giza, Egypt."
GET (extended): "Send me the next 5 days' forecast for the same location."
This modularity offers several advantages:

-Flexibility: The app can request specific data it needs, not everything at once.
-Scalability: As weather data becomes more complex (adding radar images, allergy forecasts), the API can handle it efficiently.
-Maintainability: Updating specific modules of the API is easier than rebuilding the entire system.


**-In conclusion**: REST APIs are the secret sauce that allows apps to efficiently access and display dynamic data.




###Principles of RESTful API:

-Stateless :

