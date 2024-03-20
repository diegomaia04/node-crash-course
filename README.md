# Node.js Course

- Syntax and basic concepts of Node.js, the language we will be developing with in the third semester of college.

  - As a foundation, I'm taking an online course to enhance my understanding and concepts about the subject.

We use JavaScript for front-end development, but with Node.js, we use a variation of JavaScript for the back-end.
 
 Basically, Node.js is a way to use JavaScript on the backend.

- No need to learn an extra language for the server
- Can share code between front and backend
- Node.js has a massive community behind it
- Huge amount of third-party packages & tools to help

#### In this course

- How to install Node & use it to run JavaScript
- How to read & write files on your computer
- How to create a server using Node.js to create a website
- How to use MongoDB (a NoSQL database)
- How to use template engines to easily create HTML views
- Put everything together to make a simple blog site

###### ! The way the server connects with the website is through the IP address (localhost)

It connects through HTTP (Hyper-Text Transfer Protocol).

`localhost` is like a domain name on the website

##### Status Codes

- Status Codes describe the type of response sent to the browser

    * 200 - OK
    * 301 - Resource moved
    * 404 - Not found
    * 500 - Internal server error

 Installing packages Globally

 - lodash
 - express

 ###### View Engines

 - Engines are capable of doing templates of code HTML, with dynamic data like variables, data from databases, etc.

 - EJS: 

"EJS" typically stands for "Embedded JavaScript." It's a templating engine for Node.js, allowing you to create HTML templates with embedded JavaScript. With EJS, you can generate HTML dynamically with server data before sending it to the client's browser. This is useful in web applications that need to render dynamic pages based on server data. EJS enables you to easily embed JavaScript code within your HTML pages to make them dynamic and interactive.

      * `npm install EJS`

      "Download the extension: EJS language support"

###### Passing Data into Views 

- EJS templates are processed through the EJS view engine on the server

##### Partials

are parts of templates, these files that can be reused in new views and reused.

###### Middleware

- Code which runs (on the server) between getting a request and sending a response

- Could be many Middlewares, like many functions that come into the browser and execute something

Middleware Examples:

* Logger Middleware to log details of every request

* Authentication check Middleware for protected routes

* Middleware to parse JSON data from the request

* Return 404 pages 

Third-party Middleware called Morgan, we pass a log and the Morgan dispatches how the log is going to be formatted

##### NoSQL vs SQL

SQL: tables, rows, columns

NoSQL: Collections, Documents, and MongoDB

- In my other repositories, there is a special one that contains the contents of MongoDB, where everything about MongoDB is, so access and take your doubts

* Mongoose, models & schemas => 

    - Mongoose is an ODM library (object document mapping library)

    * Schemas define the structure of a type of data / document properties & property types

####### request types

* GET: request to get a Resource

        localhost:3000/blogs
        localhost:3000/blogs/create
        localhost:3000/blogs:id

* Post: requests to create new data (e.g a new blog)

        localhost:3000/blogs (we ccan use the same address)

* Delete: request to delete data (e.g delete a blog)

       localhost:3000/blogs/:id

* PUT: request to update data (e.g updat a blog)

       localhost:3000/blogs/:id

###### route parameters

 * the variable parts of the route that may change value.

 * round parameters are the part of a route taht are variable we could changle. Examples:

       localhost:3000/blogs/:id
       localhost:3000/blogs/12345
       localhost:3000/blogs/50hello
       localhost:3000/blogs/hello


