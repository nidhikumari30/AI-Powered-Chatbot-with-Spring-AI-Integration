# Food-Ordering-Delivery-Web-Application

AI-powered Food Ordering & Delivery Web Application — React frontend + Spring Boot backend.

## Project Overview

- **Purpose:** A full-stack food ordering and delivery platform connecting customers and restaurants/businesses. The app demonstrates authentication (JWT), REST APIs, and a React single-page frontend.
- **Stack:** React, Semantic UI (frontend); Java Spring Boot, Spring Security, MySQL (backend); Docker / Docker Compose for local backend.

## Repository layout

- `react-frontend/` — React application (UI, components, services, tests)
- `spring-backend/` — Spring Boot REST API (controllers, services, repositories, Docker)

> The codebase originally included a feature-focused `api/` folder in the frontend; proposed improvements are described below.

## Quickstart (development)

Prerequisites:

- Java 11+
- Node.js + npm (Node 16+ recommended)
- Docker & Docker Compose (for the backend DB and app)

Frontend (run locally):

```powershell
cd react-frontend
npm install
npm start
```

The frontend dev server runs at http://localhost:3000 by default (React).

Backend (run with Docker Compose):

```powershell
cd spring-backend
docker-compose up --build
```

API docs (when backend runs):

```
http://localhost:8080/swagger-ui/index.html
```

NOTE: Sign-up and authentication endpoints return a JWT token. Use that token to authorize requests to secured endpoints.

## Environment & Configuration

- Frontend: add any runtime env in `.env` inside `react-frontend/` (e.g., `REACT_APP_API_BASE_URL=http://localhost:8080`)
- Backend: configure `application.properties` (DB credentials, `spring.mail.*` if email features are used). If no mail account is provided some email endpoints may produce authentication exceptions but core features still work.

## Suggested safe restructuring (non-breaking, incremental)

I recommend these minimal, safe improvements you can apply before pushing to GitHub:

1. Frontend: move API helper files from `src/api/` into `src/services/` and add index exports (`src/services/index.js`) to create a simple barrel. This keeps imports tidy and is non-destructive.
2. Frontend: group components by feature under `src/components/{home,auth,offer,users,...}` — many components are already feature-scoped, so this will be largely a reorganization.
3. Backend: keep `spring-backend/` intact. If you rename, keep Maven coordinates unchanged or update `pom.xml` accordingly.
4. Add a top-level `CONTRIBUTING.md` if you plan to accept PRs.

I can perform the safe, incremental moves (creating barrels, updating relative imports) if you want — I'll do them in small commits to avoid breaking the app.

## Tests

- Frontend tests use Jest and React Testing Library. Run:

```powershell
cd react-frontend
npm test
```

- Backend tests (if present) can be run with Maven inside `spring-backend/`:

```powershell
cd spring-backend
./mvnw test
```

## How to prepare the repo for GitHub (recommended commit flow)

1. Run linters and tests locally.
2. Make small, focused commits (e.g., "chore(frontend): move api services to services/ and add barrel exports").
3. Push your branch and open a PR for review.

If you want, I can prepare a commit that only reorganizes frontend services into `src/services/` and updates imports.

## Contributing

- Fork the repo, create a feature branch, open a PR. Keep changes focused and include tests for new behavior.

## Developed by

- You
- Contact: nidhikumari934181@gmail.com
- LinkedIn: https://linkedin.com/in/nidhi-kumari-4648692b2
- GitHub: https://github.com/nidhikumari30

## Notes / Next steps I can do

- Create `src/services` barrels and update imports in the frontend (safe, can be done in small commits).
- Run frontend tests and fix minor import path issues.
- Add `CONTRIBUTING.md` and `CODE_OF_CONDUCT.md` if needed.

If you'd like me to perform the safe frontend reorganizations now, say "Do the refactor" and I'll proceed with small commits and update the todo list.

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


