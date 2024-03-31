# popeye
Master the basic of contenerizations
# General Description

This project involves containerizing and defining the deployment of a simple web poll application. The application is composed of 5 elements:

1. **Poll**: 
   - A Flask Python web application that gathers votes and pushes them into a Redis queue.

2. **Redis Queue**:
   - Holds the votes sent by the Poll application, awaiting them to be consumed by the Worker.

3. **Worker**: 
   - A Java application that consumes the votes from the Redis queue and stores them into a PostgreSQL database.

4. **PostgreSQL Database**:
   - Persistently stores the votes stored by the Worker.

5. **Result**:
   - A Node.js web application that fetches the votes from the database and displays the results.

## Setup Instructions

To set up and deploy the web poll application, follow these steps:

1. Clone this repository to your local machine.
2. Navigate to the project directory.
3. Follow the instructions in the respective directories (Poll, Worker, Result) to build and deploy each component.
4. Ensure that all dependencies are installed and configured properly.
5. Once all components are deployed, you can access the web poll application and view the results.

## Result
| Category                         | Percentage | Tests | Crash |
|----------------------------------|------------|-------|-------|
|  Image poll                      | 100%       | 3/3   | x     |
| Image result                     | 100%       | 4/4   | x     |
| Image worker                     | 100%       | 3/3   | x     |
| Docker compose                   | 100%       | 7/7   | x     |
| End score                        | 100%       | 17/17 | x     |

Beware of -42 Epitech students !!!
