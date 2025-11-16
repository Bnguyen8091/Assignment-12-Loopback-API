📘 Assignment 12 - Auto-Generated API Using LoopBack 4

This repository contains my implementation for Quiz 14 – Automatic API Generator.
For this assignment, I used LoopBack 4 to automatically generate a fully functional REST API, including models, datasources, repositories, and controllers. The final API exposes CRUD endpoints for a Book model and includes an interactive Swagger-style API Explorer.


🚀 Overview

LoopBack 4 is a Node.js framework that provides powerful CLI tools capable of generating entire APIs with minimal manual coding.
Using the LoopBack generator, this project demonstrates:

Automatic API scaffolding

Model and schema generation

Repository creation for CRUD operations

Controller generation for RESTful endpoints

In-memory datasource configuration

Testing the API in the built-in /explorer UI




🛠️ Tools Used

LoopBack 4 CLI — auto-generates APIs

Node.js + npm — runtime and package manager

TypeScript — LoopBack’s default language

Swagger UI Explorer — auto-generated documentation for API testing



📦 Project Structure (Auto-Generated)

LoopBack generated the following components:

Component	Description
Model	Book model with id, title, author, year
Datasource	In-memory datasource (db.datasource.ts)
Repository	CRUD repository (BookRepository)
Controller	REST controller exposing API endpoints
Explorer	UI for interacting with the API
📚 Book Model Definition

The model includes:

id (auto-generated string ID)

title (required string)

author (required string)

year (optional number)



🔧 Steps I Followed 

1️. Install LoopBack CLI
npm install -g @loopback/cli

2️. Create the LoopBack Application
lb4 app


Configured project name, settings, and scaffolding.

3️. Generate the Model
lb4 model


Created the Book model and later added an auto-generated id property.

4️. Create a Datasource
lb4 datasource


Selected the In-memory DB connector.

5️. Create the Repository
lb4 repository


Connected the Book model to the datasource using a CRUD repository.

6️. Generate the REST CRUD Controller
lb4 controller


Automatically generated all REST endpoints for the Book model.

7️. Start the API Server
npm install
npm start



🌐 How to Run This Project

Clone the repository:

git clone https://github.com/Bnguyen8091/quiz14-loopback-api.git
cd quiz14-loopback-api


Install dependencies:

npm install


Start the server:

npm start


Then open the API Explorer in your browser:

http://localhost:3000/explorer



📸 Screenshots
API Explorer – Auto-Generated Endpoints



