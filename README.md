# Interactive Web Application Illustrating Global Time and Broadcast Protocols

This project was my senior capstone project at Western Carolina University, completed in 
December 2022 with classmate Cameron Craven. 

The projects main goal is to create a visual learning tool to help further understanding of 
some important cloud computing concepts. These concepts include the happens-before relationship, 
Lamport clocks and vector clocks, and the reliable broadcast protocols.

To achieve this goal we:

* have example timing diagrams for each concept, along with definitions
* allow the user to input a schedule which is then classified
* the resulting timing diagram, broadcast protocol, and lamport/vector clocks are then shown to 
  the user

### Concepts Covered:
##### Happens-Before Relationship
Many important software systems today utilize distributed systems For distributed systems to work 
reliably, one must address the issues of the lack of a global clock and lack of shared memory. To
address the problem of lack of a global clock in distributed systems, the first step is to establish
a happens-before relationship. After establishing a happens-before relationship, further ways to 
understand the ordering of events would be logical clocks and broadcast protocols. There are two types 
of logical clocks, those being lamport clocks and vector clocks.

##### Logical Clocks
Lamport clocks can be used to determine the happens- before relationship among events. However, they 
are not able to detect when two events are concurrent. Vector clocks allow us to know which events are
concurrent.

##### Broadcast Protocols
Another way of understanding delivery order is through broadcast protocols. A broadcast is when a node
sends a message and all nodes in the group receive it. We focus on reliable broadcasts, where messages 
are not allowed to drop. These protocols are :
* FIFO broadcast,
* Causal broadcast,
* Total Order broadcast,
* FIFO-Total Order broadcast


## To run the full project:
* Run server.js
* Run npm start, as described below:

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

