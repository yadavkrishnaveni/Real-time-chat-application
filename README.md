# Real-time-chat-application

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: PANDI KRISHNAVENI

*INTERN ID*: CT04DL269

*DOMAIN*: FRONT END DEVELOPMENT

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH 

This project is a real-time chat application built using HTML, CSS, JavaScript, and WebSockets. The primary goal of this project is to allow two users to communicate with each other in real time through a browser interface. The application currently supports chatting between two tabs of the same browser and can be enhanced to support chat between different URLs or devices. The development of this project was done entirely using Visual Studio Code (VS Code), a powerful and widely-used code editor that offers features like integrated terminal, syntax highlighting, debugging support, and extension marketplace.

The application consists of several main components:

1. Login System:
The login system is implemented using an HTML form in index.html and a simple JavaScript file login.js. The user enters their name in an input box. When the "Enter Chat" button is clicked, the name is saved to localStorage and the user is redirected to the chat interface (chat.html). This mechanism is simple but effective for basic identity management in a local testing environment.


2. Chat Interface:
The chat interface in chat.html includes a welcome message, a chat display box, an input box to type messages, and a send button. The name entered on the login page is retrieved from localStorage and shown as a greeting. Messages typed in the input box are displayed in the chat window and saved to localStorage. CSS from style.css is used to make the chat interface more visually appealing, with styling for sent and received messages.


3. Real-time Communication Logic:
The core logic for message broadcasting is written in chat.js. When a user sends a message, it is added to localStorage. The window.addEventListener('storage') event listens for changes in localStorage across different tabs of the same browser. This allows the application to simulate real-time chat between two tabs under the same origin. Sent messages are aligned to the right and colored green, while received messages are aligned to the left and colored blue.


4. WebSocket Server:
A Node.js server using the ws module (server.js) was implemented to support future scalability. It listens for client WebSocket connections on port 3000. When a message is received from a client, the server broadcasts it to all other connected clients using the WebSocket protocol. This server can be enhanced to allow communication between different browsers, devices, or IP addresses.


5. Development Environment:
All code was written and executed in Visual Studio Code (VS Code). The integrated terminal was used to run the WebSocket server with the command node server.js, and the built-in live server extension helped in testing the HTML files. VS Code's project structure and file explorer made it easy to organize code and resources efficiently.


In conclusion, this project demonstrates how real-time communication can be achieved using browser technologies and WebSockets. While the current version supports communication between tabs, the structure and logic are in place to upgrade it for broader, networked usage. This project serves as a strong foundation for more advanced chat applications.

#OUTPUT

![IMG-20250610-WA0042 1](https://github.com/user-attachments/assets/630a7f87-7cfb-4347-bbd5-753ec3d89ad6)

