Secured Time Capsule Application
This project is a secured time capsule system that allows users to create, store, and retrieve encrypted messages. Each user can securely access their time capsules through a protected login system, ensuring that only the right user can open their messages.

Features:
1. User Registration and Authentication:

-Users can create an account with their email and password.
-Passwords are securely hashed using the bcrypt algorithm before being stored in the database.
-Users log in to access their time capsules, using JWT (JSON Web Token) for secure session management and authentication.

2.Create Time Capsules:
-Once logged in, users can create a time capsule by writing a message they want to save.
-The message is encrypted using AES (Advanced Encryption Standard) before it is stored in the database, ensuring data confidentiality.

3.View Time Capsules:
-After logging in, users can retrieve their stored time capsule messages.
-The encrypted messages are decrypted upon retrieval and displayed in plain text to the authenticated user.

System Architecture:
-Client-Server Model:
-The client sends requests to the server, which handles authentication, encryption, and database storage.
-All sensitive information, such as passwords and time capsule messages, is securely encrypted and managed on the server-side.

-Security:
-Passwords are hashed using bcrypt and never stored in plain text.
-AES encryption is used to protect time capsule messages in the database.
-JWT is used to handle user sessions and authentication securely.

Technologies Used:
-Backend:
-Java (Spring Boot or plain Java implementation with servlets/sockets)
-JWT for session management and authentication
-AES for message encryption
-bcrypt for password hashing

-Database:
-MySQL or PostgreSQL for storing user accounts and encrypted time capsules

-Frontend:
-Client application built using Android (or any other platform) to interact with the server through API calls.

-Installation and Setup:
1. Clone the repository:
git clone https://github.com/AlexandraNimhagen/IT_SAKERHET_JAVA23_Alexandra_Nimhagen_Uppgift2.git
2. Set up the database with MySQL or PostgreSQL and create the necessary tables for users and time capsules.
3. Configure the server to handle API requests, JWT authentication, and AES encryption.
4. Run the application on a local server or deploy it to a hosting service.
