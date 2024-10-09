# MVC Full-Stack Application

This project is a full-stack web application using a Model-View-Controller (MVC) architecture. It consists of a frontend built with React and a backend built with Django.

## Project Structure

The project is divided into two main parts:

1. `front`: Contains the frontend React application
2. `back`: Contains the backend Django application

## Prerequisites

- Docker
- Docker Compose

## How to Run

1. Clone the repository
2. Navigate to the project root directory
3. Run the following command to start the application:

   ```
   docker-compose up --build
   ```

4. Access the frontend at `http://localhost:3000`
5. Access the backend API at `http://localhost:8000`

## Development

- The frontend development server runs on port 3000 and has hot-reloading enabled.
- The backend Django server runs on port 8000.
- The PostgreSQL database runs on port 5432.

## Testing

### Backend Testing

To run the backend tests:

1. Make sure your Docker containers are running
2. Execute the following command:

   ```
   docker-compose exec back python manage.py test
   ```

This will run the Django test suite for the backend.

### Frontend Testing

To run the frontend tests:

1. Make sure your Docker containers are running
2. Execute the following command:

   ```
   docker-compose exec front npm test
   ```

This will run the Next.js test suite for the frontend. 

Note: If you encounter any issues, make sure that the test script is properly configured in the `package.json` file of the frontend application.