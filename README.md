# Microservice Email Sender

This microservice, developed with Spring Boot, allows sending emails using a RESTful API.

## Features

- Sends emails with provided details such as recipient, subject, and message body.
- Utilizes Spring Boot for RESTful endpoints and email functionality.
- Integrated with H2 database for storing email details.
- Utilizes Spring Boot Data JPA for database interactions.
- Validation checks for email request data using Spring Boot Validation.

## Prerequisites

- JDK 17
- Maven 3.6.x

## Getting Started

1. Clone this repository: `git clone https://github.com/juliocmarinho/ms-emailsender.git`
2. Navigate to the project directory.
3. Build the project using Maven: `mvn clean install`
4. Run the application: `mvn spring-boot:run`

## Usage

The microservice exposes an endpoint to send emails:

- **POST** `/sending-email`: Sends an email with specified details.

Request Body Example:
```json
{
  "ownerRef" : "Name",
  "emailFrom": "sender@example.com",
  "emailTo": "recipient@example.com",
  "subject": "Subject of the email",
  "text": "Body of the email"
}
```

## Configuration

- The application uses H2 in-memory database by default.
- Check `src/main/resources/application.properties` for configuration details.


## License

This project is licensed under the [MIT License](LICENSE).

---
