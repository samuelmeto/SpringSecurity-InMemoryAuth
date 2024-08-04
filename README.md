# Basic Spring Security In-Memory Authentication

This project demonstrates a basic in-memory user authentication system using Spring Security with Spring Boot. It includes simple user authentication with roles stored in memory.

## Features

- In-memory user authentication
- Basic authentication with usernames and passwords
- Role-based access control

## Technologies Used

- Java 20
- Spring Boot 3.3.2
- Spring Security

## Getting Started

### Prerequisites

- Java 20
- Maven

### Installation

1. **Clone the repository**
    ```bash
    git clone https://github.com/samuelmeto/basic-springsecurity-auth.git
    cd basic-springsecurity-auth
    ```

2. **Build and run the application**
    ```bash
    mvn clean install
    mvn spring-boot:run
    ```

### Configuration

No external configuration is needed since this application uses in-memory authentication.

### User Details

The application is pre-configured with the following users:

- **User 1**
  - Username: `username1`
  - Password: `password1`
  - Role: `USER`

- **User 2**
  - Username: `username2`
  - Password: `password2`
  - Role: `ADMIN`

### Accessing the Application

1. **Public Endpoints**
    - `/public/**`: Accessible to everyone.

2. **Protected Endpoints**
    - All other endpoints require authentication.

3. **Login**
    - Use basic authentication with the configured usernames and passwords to access protected endpoints.

## Project Structure

- `config`: Contains the security configuration class.

## Contributing

1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Inspired by various online tutorials and Spring Boot documentation.
