# 🍕 Food-Ordering-Delivery-Web-Application

> **A Full-Stack Web App for Ordering Food Online** | Built with React & Spring Boot

---

## 📋 About This Project

This is a **college project** that brings together **two powerful technologies**:

- 🎨 **Frontend**: A sleek, user-friendly React app where you can browse restaurants, order food, and track deliveries
- ⚙️ **Backend**: A robust Spring Boot server that handles all the business logic, user accounts, and order management

Perfect for learning how **modern web applications** work end-to-end!

---

## 🚀 Quick Start (5 minutes)

### What You'll Need:
- ✅ Java installed  
- ✅ Node.js & npm installed  
- ✅ Docker (optional, makes backend setup easier)

### Run the App:

**Frontend** (the pretty UI):
```bash
cd react-frontend
npm install
npm start
```
👉 Open http://localhost:3000 in your browser

**Backend** (the brain):
```bash
cd spring-backend
docker-compose up --build
```
👉 API runs at http://localhost:8080

---

## 📂 Project Structure

```
📦 Food-Ordering-Delivery-Web-Application
 ├── 📁 react-frontend      (What users see)
 │   └── src/
 │       ├── components/    (UI building blocks)
 │       ├── api/          (Talk to the server)
 │       ├── css/          (Pretty styles)
 │       └── ...
 │
 └── 📁 spring-backend      (The engine)
     └── src/
         ├── controller/    (Handle requests)
         ├── service/       (Business logic)
         ├── repository/    (Database stuff)
         └── ...
```

---

## 🎯 Key Features

✨ **User-Friendly Interface** - Browse, search, and order food easily  
🔐 **Secure Login** - Your data is safe with JWT tokens  
📦 **Order Management** - Track your orders in real-time  
🏢 **Restaurant Dashboard** - Manage your menu and orders  
💳 **Payment Ready** - Built to handle transactions  

---

## 🧪 Testing

Run tests to make sure everything works:

```bash
# Frontend tests
cd react-frontend
npm test

# Backend tests
cd spring-backend
./mvnw test
```

---

## 🤝 Contributing

Got ideas? Found a bug? Here's how to help:

1. **Fork** this project
2. **Create** a new branch (`git checkout -b feature/amazing-feature`)
3. **Make** your changes
4. **Commit** (`git commit -m 'Add amazing feature'`)
5. **Push** and open a **Pull Request**

---

## 📚 Learn More

- 🌐 Check the **API docs** at: http://localhost:8080/swagger-ui/index.html (when backend is running)
- 💡 Each component is documented in its folder
- 🔧 Configuration files explain setup details

---

## 👩‍💻 Developed by

**Nidhi Kumari**

📧 **Email**: nidhikumari934181@gmail.com  
🔗 **LinkedIn**: https://linkedin.com/in/nidhi-kumari-4648692b2  
🐙 **GitHub**: https://github.com/nidhikumari30

---

<div align="center">

**Made with ❤️ for learning and sharing**

</div>

<b>ReactJS-Spring-Boot-Full-Stack-App</b>
<hr>

This project consists of two applications: one is a Spring Boot Rest API
called spring-backend and another is a ReactJS application called
react-frontend.

Service-oriented platform focusing on establishing and maintaining
connections between consumers and small businesses in the The Arts,
Entertainment, and Recreation sector.

Click [here](https://www.hobbie.ch) to view the application.
This application is subject to Copyright.

<b>Applications</b>
<hr>

 <b> - spring-backend</b>

Spring Boot Web Java backend application that exposes a REST API to
manage hobbies. Its secured endpoints can just be accessed if an access
token (JWT) is provided.

spring-backend stores its data in a MySql database.

spring-backend has the following endpoints


<b>-react-frontend</b>

ReactJS frontend application where users can find and save hobbies and businesses can manage offers. In order to access the application, user / business must login using his/her username and password.  All the requests coming from react-frontend to secured endpoints in spring-backend have a access token (JWT) that is generated when user / business logs in.

react-frontend uses Semantic UI React as CSS-styled framework.

<b>Prerequisites</b>
<hr>

-Java 11+

-npm

-JWT 

<b>Set up</b>

<hr></hr>

Clone the repository:

<pre>git clone https://github.com/purshink/ReactJS-Spring-Boot-Full-Stack-App.git</pre>

Navigate to the newly created folder:

<pre>cd  ReactJS-Spring-Boot-Full-Stack-App</pre>
 

<b>Frontend -</b>

Install NodeJs.v.16.13.1 /npm v.8.3.0

Navigate to react-frontend subfolder:
 
<pre>cd react-frontend</pre>

Install the modules

<pre>npm i</pre>

Start the application on local host:

<pre>npm start</pre>

Navigate to:

http://localhost:4200

 
<b>Backend -</b>
Install JDK 11.0.11
Install docker -v 20.10.7
Install docker-compose -v 1.8.0

Navigate to spring-backend subfolder:

<pre>cd spring-backend</pre>

Run the project with:

<pre>docker-compose up --build</pre>


The project has the following endpoints:

IMPORTANT: to explore api enter url:  /v3/api-docs

http://localhost:8080/swagger-ui/index.html


NOTE: Testing API 

-/signup (create client-user) or /register (create business-user)

-/authenticate (returns JWT authentication token)

-use JWT token in order to authorize access to secured endpoints (click the lock icon or use the Authorize button on the upper right corner - then paste JWT Token )

NOTE: /notification endpoint will return an internal server error if you don't specify spring.mail credentials first.

<pre>The backend will run on http://localhost:8080 </pre>

<b>Spring Mail</b>

Make sure to specify a valid spring.mail.username and spring.mail.password in the application.properties file in order to be able to send an Email confirmation for updating user entries.

IMPORTANT: if you decide not to specify mail credentials, you will get javax.mail.AuthenticationFailedException. The rest of the application should work normally despite this exception.


