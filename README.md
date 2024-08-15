# IntroToWebAPI
 Creating a web API with ASP.NET Core controllers

# Introduction
This module explores creating a cross-platform RESTful service by using ASP.NET Core web API controllers with .NET and C#.

In this module, we use the .NET CLI (command-line interface) and Visual Studio Code for local development. After you complete this module, you can apply its concepts by using a development environment like Visual Studio (Windows). You can also apply the concepts to continued development through Visual Studio Code (Windows, Linux, and macOS).

# Example scenario
Suppose you're an employee of a pizza company named Contoso Pizza. Your manager has asked you to develop a RESTful service for pizza inventory management as a prerequisite for the company's web storefront and mobile application. The service has to support adding, viewing, modifying, and removing types of pizza; a standardized usage of HTTP verbs better known as create, read, update, delete (CRUD).

# What will we be doing?
In this module, you create a new web API application by using ASP.NET Core, and learn how to run and test it from the command line. Then, you add a data store and a new API controller. Finally, you implement and test the API methods to create, read, update, and delete pizzas from the data store.

# What's the main goal?
By the end of this session, you're able to create new web API applications by using ASP.NET Core, and you've learned how to create API controllers that implement basic CRUD logic.

# REST in ASP.NET Core
When you browse to a webpage, the web server communicates with your browser by using HTML, CSS, and JavaScript. For example, If you interact with the page by submitting a sign-in form or selecting a buy button, the browser sends the information back to the web server.

In a similar way, web servers can communicate with a broad range of clients (browsers, mobile devices, other web servers, and more) by using web services. API clients communicate with the server over HTTP, and the two exchange information by using a data format such as JSON or XML. APIs are often used in single-page applications (SPAs) that perform most of the user-interface logic in a web browser. Communication with the web server primarily happens through web APIs.

# REST: A common pattern for building APIs with HTTP
Representational State Transfer (REST) is an architectural style for building web services. REST requests are made over HTTP. They use the same HTTP verbs that web browsers use to retrieve webpages and send data to servers. The verbs are:

-GET: Retrieve data from the web service.
-POST: Create a new item of data on the web service.
-PUT: Update an item of data on the web service.
-PATCH: Update an item of data on the web service by describing a set of instructions about how the item should be modified. The sample application in this module doesn't use this verb.
-DELETE: Delete an item of data on the web service.

Web service APIs that adhere to REST are called RESTful APIs. They're defined through:
-A base URI.
-HTTP methods, such as GET, POST, PUT, PATCH, or DELETE.
-A media type for the data, such as JavaScript Object Notation (JSON) or XML.


An API often needs to provide services for a few different but related things. For example, our pizza API might manage pizzas, customers, and orders. We use routing to map URIs to logical divisions in our code, so that requests to https://localhost:5000/pizza are routed to PizzaController and requests to https://localhost:5000/order are routed to OrderController.

# Benefits of creating APIs in ASP.NET Core
With ASP.NET, you can use the same framework and patterns to build both webpages and services. You can reuse model classes and validation logic, and even serve both webpages and services side by side in the same project. This approach has benefits:
-Simple serialization: ASP.NET was designed for modern web experiences. Endpoints automatically serialize your classes to properly formatted JSON out of the box. No special configuration is required. You can customize serialization for endpoints that have unique requirements.

-Authentication and authorization: For security, API endpoints have built-in support for industry-standard JSON Web Tokens (JWTs). Policy-based authorization gives you the flexibility to define powerful access-control rules in code.

-Routing alongside your code: ASP.NET lets you define routes and verbs inline with your code by using attributes. Data from the request path, query string, and request body are automatically bound to method parameters.

-HTTPS by default: HTTPS is an important part of modern, professional web APIs. It relies on end-to-end encryption to provide privacy and to help ensure that your API calls aren't intercepted and altered between client and server.

ASP.NET provides support for HTTPS out of the box. It automatically generates a test certificate and easily imports it to enable local HTTPS, so you can run and debug your applications securely before you publish them.

# Share code and knowledge with .NET apps

You can use your .NET skills and ecosystem to share logic from your web API to other apps built with .NET, including mobile, web, desktop, and services.

# Features
Introduction to web APIs and RESTful principles
Step-by-step guide to setting up a web API
Code examples with detailed explanations
Instructions for testing and debugging APIs
Best practices for API development and deployment


# Installation
To set up this project locally, follow these steps:

Clone the repository:
git clone https://github.com/Utsav-AD/IntroToWebAPI.git

Navigate to the project directory:
cd IntroToWebAPI

Install the required dependencies:
[command to install dependencies]
Usage

To run the web API, execute the following command:
[command to run the server]
After running the above command, the API will be accessible at http://localhost:[port]/. You can interact with the API using tools like Postman or via your browser.

Example Endpoints
GET /api/resource - Retrieves a list of resources
POST /api/resource - Creates a new resource
PUT /api/resource/{id} - Updates an existing resource
DELETE /api/resource/{id} - Deletes a resource


# Project Structure
IntroToWebAPI/
│
├── src/                    # Source code for the API
│   ├── routes/             # API route definitions
│   ├── models/             # Database models
│   └── app.py              # Main application file
│
├── tests/                  # Test cases for the API
│
├── README.md               # Project documentation
├── requirements.txt        # Dependencies (for Python)
└── package.json            # Dependencies (for Node.js)


# Contributing
Contributions are welcome! If you have any suggestions or improvements, feel free to open an issue or create a pull request. Please ensure that your contributions adhere to the project's code of conduct.

# License
This project is licensed under the MIT License - see the LICENSE file for details.


