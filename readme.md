# MovieMate

MovieMate is a Java Spring Boot application that provides RESTful endpoints to manage and review movies. It allows users to retrieve lists of movies, view details of individual movies, and rate movies using IMDb IDs.

## Features

- Retrieve a list of all movies
- Retrieve details of a single movie by IMDb ID
- Rate a movie using IMDb ID

## Technologies Used

- Java Spring Boot
- MongoDB
- Spring Data MongoDB
- Spring Security

## Getting Started

### Prerequisites

- Java 11 or higher installed
- MongoDB installed and running

### Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/MovieMate.git
   ```

2. Navigate to the project directory:

   ```bash
   cd MovieMate
   ```

3. Build the project:

   ```bash
   ./mvnw clean install
   ```

   This will compile the project and install the dependencies. The compiled JAR file will be created in the `./target` directory.

### Configuration

1. Configure MongoDB connection settings in `application.properties`:

   ```properties
   spring.data.mongodb.host=localhost
   spring.data.mongodb.port=27017
   spring.data.mongodb.database=moviedb
   ```

2. Optionally, configure other application properties such as server port and logging settings.

### Running the Application

1. Run the JAR file:

   ```bash
   java -jar target/MovieMate.jar
   ```

2. Alternatively, run the application using Maven:

   ```bash
   ./mvnw spring-boot:run
   ```

### API Endpoints

- **GET /api/v1/movies**: Retrieve a list of all movies.
- **GET /api/v1/movies/{imdbId}**: Retrieve details of a single movie by IMDb ID.
- **POST /api/v1/reviews/**: Rate a movie using IMDb ID with a request body.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.
