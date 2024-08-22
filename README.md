# FisherMap PH Website Server

> This is a Special Problem Topic of John Rommel B. Octavo


### Installation:

1. Make sure to install necessary modules and package in Nest.js. On the main directory run this command: $ `npm install`
2. On the main directory, add the .env file to specify the `DB_URI`, `DB_NAME`, `APP_NAME`, `JWT_SECRET`, `JWT_EXPIRES`, `BACKEND`, `FRONTEND`, `MAIL_HOST`, `MAIL_USER`, `MAIL_PASSWORD`. 
3. To run the NestJS app run this command: $ `npm start:dev` or `npm start`.


### Details:

The server of both the mobile and web applications was built using the NestJs. It is a typescript framework for building efficient, reliable, and scalable server-side applications.

The Representational State Transfer Application Programming Interface (REST API) was employed in the server. REST API was used to simplify the server design and improve the scalability. Its stateless nature helps in the distribution of load to servers which results in greater performance.

NestJs provides modularity which is key to handling complex backend structures such as the FisherMap PH. Each module represents the entity in the databases. The controllers, providers, and the service provide a way to structure the handling of endpoints. The separation of concerns makes it easy to handle the Create, Read, Update, and Delete (CRUD) operations.

Using the Mongoose package, NestJs retrieves and manipulates the data from the MongoDB database. Schemas and Data Transfer Objects (DTO) are used to validate and correctly transfer these data to different layers or components of the application.

On the security side, JSON Web Token (JWT) is used for authentication and authorization of both the mobile and website applications. The token was stored using an HTTP-only cookie and Flutter Secure Storage for website and mobile applications respectively. To protect the server routes, each HTTP request implements an authorization mechanism using the NestJS Guard class.
