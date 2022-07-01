# FreedomGaming-Backend :star_struck: :computer: :video_game: :headphones: :iphone:

***This new API FOR FREEDOM GAMING E-COMMERCE ANDROID APPLICATION is created by Ankita Sikder and Other Group Members as Project 5, students of BTECH, in University of Engineering and Management, Kolkata.***

**Email Id: ankita.sikder14@gmail.com.** 

## URL :point_right: https://freedom-gaming-ipa.herokuapp.com/api/v1/

[![Generic badge](https://img.shields.io/badge/bcryptjs-%5E2.4.3-maroon)](https://shields.io/) [![Generic badge](https://img.shields.io/badge/body--parser-%5E1.19.0-yellow)](https://shields.io/) [![Generic badge](https://img.shields.io/badge/cors-%5E2.8.5-green)](https://shields.io/) [![Generic badge](https://img.shields.io/badge/dotenv-%5E10.0.0-orange)](https://shields.io/) [![Generic badge](https://img.shields.io/badge/express-%5E4.17.1-blue)](https://shields.io/) [![Generic badge](https://img.shields.io/badge/express--jwt-%5E6.0.0-yellowgreen)](https://shields.io/) [![Generic badge](https://img.shields.io/badge/jsonwebtoken-%5E8.5.1-red)](https://shields.io/) [![Generic badge](https://img.shields.io/badge/mongoose-%5E5.13.2-blueviolet)](https://shields.io/) [![Generic badge](https://img.shields.io/badge/morgan-%5E1.10.0-9cf)](https://shields.io/) [![Generic badge](https://img.shields.io/badge/multer-%5E1.4.2-ff69b4)](https://shields.io/) [![Generic badge](https://img.shields.io/badge/nodemon-%5E2.0.12-success)](https://shields.io/) 

## What is FREEDOM-GAMING-SERVER and Why have I made this API :point_down:

<div align="justified">

I have made this FREEDOM-GAMING-BACKEND to work on my e-commerce grocery android application FREEDOM GAMING. The application is in my another github repository [freedom gaming frontend](). Using GET, POST, PUT etc requests through specific uniform resource locator(hosted by HEROKU) or through localhost I have done varoius operations on the app. I have added products, categories. I have also created admin users to specify who can work on the app and who is just an user. I have created register and login option. Here using the bearer token user can work as an admin user. Here the data goes to mongoDB from localhost or HEROKU provided hosting and images goes to my firebase account's daily deals project's storage. The development of apps for mobile devices meant that organizations needed to allow users to access information through apps and not just through the Internet. Within the public sector, APIs are used to allow agencies to easily share information and also lets the public interact with government as well. While there are numerous protocols and technologies involved, the underlying purpose of APIs is always the same: to let one piece of software communicate with another. For all these reasons I have made it and worked with it in my android application named Freedom Gaming.

</div>

## About API :point_down: 

<div align="justified">
 
An application programming interface (API) is a connection between computers or between computer programs. It is a type of software interface, offering a service to other pieces of software. A document or standard that describes how to build such a connection or interface is called an API specification. A computer system that meets this standard is said to implement or expose an API. The term API may refer either to the specification or to the implementation. In contrast to a user interface, which connects a computer to a person, an application programming interface connects computers or pieces of software to each other. It is not intended to be used directly by a person (the end user) other than a computer programmer who is incorporating it into software. An API is often made up of different parts which act as tools or services that are available to the programmer. A program or a programmer that uses one of these parts is said to call that portion of the API. The calls that make up the API are also known as subroutines, methods, requests, or endpoints. An API specification defines these calls, meaning that it explains how to use or implement them. An API (Application Programming Interface) is a set of functions that allows applications to access data and interact with external software components, operating systems, or microservices. API lets a developer make a specific “call” or “request” in order to send or receive information. This communication is done using a programming language called “JSON.”  It can also be used to make a defined action such as updating or deleting data. There are four basic request methods that can be made with API:
<br>GET – Gathers information (Pulling all Coupon Codes)
<br>PUT –  Updates pieces of data (Updating Product pricing)
<br>POST – Creates (Creating a new Product Category)
<br>DELETE – (Deleting a blog post)
<br>JSON (JavaScript Object Notation) is used to represent data on a server. It’s fairly easy to read by humans, and easy for machines/applications to understand.

 
</div>

### HEROKUAPP LINK :point_down:

<div align="justified">
 
I have made this API testing and hosted it in HEROKU. I have generated a link through HEROKU. I have used POSTMAN application for POST, GET, DEL, PUT requests for this API where I have created a workspace and pasted the link. Using the API link we can upload image files in uploads folder in public folder in HEROKU app storage using POST REQUEST. After that it will be uploaded in my 'fg-images-bucket's storage in https://console.firebase.google.com/project/fg-images-bucket/storage/fg-images-bucket.appspot.com/files in my firebase acount associated with my email id 'bbiswa471@gmail.com'. If a user is 'ADMIN USER' he or she will be able to get details like user details. For this he or she has to use GET REQUEST. HEROKU filesystem is ephemeral it means it automatically deletes the files from its storage after a span of time. Like this we can also send data like categories, products in my MongoDb account's(associated with my email id 'bbiswa471@gmail.com') [FG-IPA project's storage](https://cloud.mongodb.com/v2#/org/6116a7a7b7c84e51efa3f988/projects) . We can also work with PUT, DEL etc requests to perform other tasks in backend.
 
</div>

### WHY I HAVE USED MONGODB and FIREBASE AFTER USING HEROKU :point_down:

<div align="justified">
 
The Heroku filesystem is ephemeral - that means that any changes to the filesystem whilst the dyno is running only last until that dyno is shut down or restarted. Each dyno boots with a clean copy of the filesystem from the most recent deploy. This is similar to how many container based systems, such as Docker, operate. In addition, under normal operations dynos will restart every day in a process known as "Cycling". These two facts mean that the filesystem on Heroku is not suitable for persistent storage of data. In cases where we need to store data it recommends using a database addon such as Postgres (for data) or a dedicated file storage service such as AWS S3 (for static files). For this reason I have made such an API which finally puts images in firebase storage and data like products and categories in MongoDB. So that all the files and data will be remain in the storage until I delete them.
 
</div>

## Folder Structure :point_down:

```bash
FreedomGaming-Backend
       ├── helpers
       ├── models
       ├── routers
       └── index.js
```

```bash
models
   ├── category.js
   ├── order-item.js
   ├── order.js
   ├── product.js
   └── user.js
```
I have made some data structures for my application. Using API I have added these accordingly. For products I have specified keywords for Products, Category, Orders, Users, OrderItems. I have worked with following data structures with this API for my application.


<div align="center">
 
<a href="pics/HELPER-SS4.png"><img src="pics/HELPER-SS4.png" width="800" height= "350"></a>
 
</div>

```bash
helpers
   ├── error-handler.js
   └── jwt.js
```
In this part there are 2 main js files. error-handler.js and jwt.js. I have used error-handler.js for getting error notification when registered email id doesn't match with login email id. JSON Web Token is a proposed Internet standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims. The tokens are signed either using a private secret or a public/private key. JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA. This is mainly used for authorization and infromation exchange. When we register and then login with an email id then we will get a jwt as response. Here when we decrypt the encrypted jwt then we will be able to find out if the user is an admin user or not. For this reason jwt is used.
```bash
routers
   ├── categories.js
   ├── order.js
   ├── product.js
   └── users.js
```
We have used different urls to work diffent tasks. We have created different routes to work with categories, orders, products, users. I have used categories routing to add, delete, get categories. I have used products routing to add, delete, get products. I have used orders routing to add, delete, get orders. I have used users routing to add, delete, get users.

## Screenshots :point_down: 

<div align="center">

 URL: https://freedom-gaming-ipa.herokuapp.com/api/v1/users/register<br>
 REQUEST: POST<br>
 TASK: This url with this request is used to register in freedom-gaming-backend.<br>
 
<a href="pics/fg1.PNG"><img src="pics/fg1.PNG" width="800" height= "350"></a> 
 
 URL: https://freedom-gaming-ipa.herokuapp.com/api/v1/users/login<br>
 REQUEST: POST<br>
 TASK: This url with this request is used to login in freedom-gaming-backend and a bearer key comes in response which is used for further tasks as an admin user.<br>
 
<a href="pics/fg2.PNG"><img src="pics/fg2.PNG" width="800" height= "350"></a> 
 
<a href="pics/fg2.1.PNG"><img src="pics/fg2.1.PNG" width="800" height= "350"></a> 
 
 URL: https://freedom-gaming-ipa.herokuapp.com/api/v1/users<br>
 REQUEST: GET<br>
 TASK: This url with this request is used to get all users' details of freedom-gaming-backend.<br>
 
<a href="pics/fg3.PNG"><img src="pics/fg3.PNG" width="800" height= "350"></a> 
 
<a href="pics/fg3.1.PNG"><img src="pics/fg3.1.PNG" width="800" height= "350"></a>

 URL: https://freedom-gaming-ipa.herokuapp.com/api/v1/categories<br>
 REQUEST: POST<br>
 TASK: This url with this request is used to add category in freedom-gaming-backend.<br>
 
<a href="pics/fg4.PNG"><img src="pics/fg4.PNG" width="800" height= "350"></a> 
 
<a href="pics/fg4.1.PNG"><img src="pics/fg4.1.PNG" width="800" height= "350"></a> 
 
 URL: https://freedom-gaming-ipa.herokuapp.com/api/v1/categories<br>
 REQUEST: GET<br>
 TASK: This url with this request is used to get all categories of freedom-gaming-backend.<br>
 
<a href="pics/fg5.PNG"><img src="pics/fg5.PNG" width="800" height= "350"></a> 
 
<a href="pics/fg5.1.PNG"><img src="pics/fg5.1.PNG" width="800" height= "350"></a> 
 
 URL: https://freedom-gaming-ipa.herokuapp.com/api/v1/products<br>
 REQUEST: POST<br>
 TASK: This url with this request is used to add product in freedom-gaming-backend.<br>
 
<a href="pics/fg6.PNG"><img src="pics/fg6.PNG" width="800" height= "350"></a> 
 
<a href="pics/fg6.1.PNG"><img src="pics/fg6.1.PNG" width="800" height= "350"></a> 
 
 URL: https://freedom-gaming-ipa.herokuapp.com/api/v1/products<br>
 REQUEST: GET<br>
 TASK: This url with this request is used to get all products of freedom-gaming-backend.<br>
 
<a href="pics/fg7.PNG"><img src="pics/fg7.PNG" width="800" height= "350"></a> 
 
<a href="pics/fg7.1.PNG"><img src="pics/fg7.1.PNG" width="800" height= "350"></a> 
 
<a href="pics/fg7.2.PNG"><img src="pics/fg7.2.PNG" width="800" height= "350"></a> 
 
 URL: https://freedom-gaming-ipa.herokuapp.com/api/v1/products/gallery-images/:id<br>
 REQUEST: PUT<br>
 TASK: This url with this request is used to add slider images of a product in freedom-gaming-backend.<br>
 
<a href="pics/fg8.PNG"><img src="pics/fg8.PNG" width="800" height= "350"></a> 
 
<a href="pics/fg8.1.PNG"><img src="pics/fg8.1.PNG" width="800" height= "350"></a> 
 
<a href="pics/fg8.2.PNG"><img src="pics/fg8.2.PNG" width="800" height= "350"></a> 
 
 URL: https://freedom-gaming-ipa.herokuapp.com/api/v1/products/get/featured/:count<br>
 REQUEST: GET<br>
 TASK: This url with this request is used to get all featured products of freedom-gaming-backend.<br>
 
<a href="pics/fg9.PNG"><img src="pics/fg9.PNG" width="800" height= "350"></a> 

 URL: https://freedom-gaming-ipa.herokuapp.com/api/v1/products/get/count<br>
 REQUEST: GET<br>
 TASK: This url with this request is used to get count of all products of freedom-gaming-backend.<br>
 
<a href="pics/fg10.PNG"><img src="pics/fg10.PNG" width="800" height= "350"></a> 

 URL: https://freedom-gaming-ipa.herokuapp.com/api/v1/products/:id<br>
 REQUEST: DEL<br>
 TASK: This url with this request is used to delete a product in freedom-gaming-backend.<br>
 
<a href="pics/fg11.PNG"><img src="pics/fg11.PNG" width="800" height= "350"></a> 
 
 URL: https://freedom-gaming-ipa.herokuapp.com/api/v1/categories/:id<br>
 REQUEST: DEL<br>
 TASK: This url with this request is used to delete a category in freedom-gaming-backend.<br>
 
<a href="pics/fg12.PNG"><img src="pics/fg12.PNG" width="800" height= "350"></a> 
 
 URL: https://freedom-gaming-ipa.herokuapp.com/api/v1/users/:id<br>
 REQUEST: GET<br>
 TASK: This url with this request is used to get a user's profile in freedom-gaming-backend.<br>
 
<a href="pics/fg13.PNG"><img src="pics/fg13.PNG" width="800" height= "350"></a> 
  
 URL: https://freedom-gaming-ipa.herokuapp.com/api/v1/users/profile/:id<br>
 REQUEST: DEL<br>
 TASK: This url with this request is used to delete a user in freedom-gaming-backend.<br>
 
<a href="pics/fg13.PNG"><img src="pics/fg13.PNG" width="800" height= "350"></a> 
 
These are some REQUESTS for categories, products, orders in freedom-gaming-backend, there are also other REQUESTS used for API designing.
 
 
</div>








