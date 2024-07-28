# Bank Application

This Spring Boot project is a comprehensive bank application designed to showcase the integration of advanced security mechanisms including Spring Security, OAuth2, JWT, and Keycloak. The application provides robust authentication and authorization features to ensure secure access to banking services.

## Key Features

🔒 **Spring Security**
- Provides robust authentication and authorization strategies to protect endpoints and manage user roles.
- Offers customizable security configurations and ensures secure access control throughout the application.

🔒 **OAuth2**
- Implements secure user authentication and authorization with support for various grant types such as authorization code, password, client credentials, and refresh tokens.
- Facilitates secure API access and user consent management.

🔒 **JWT (JSON Web Token)**
- Uses JWT for scalable and stateless token management, enabling secure transmission of information between parties as a JSON object.
- Eliminates the need for server-side session storage and ensures data integrity and authenticity.

🔒 **Keycloak**
- Integrates Keycloak for seamless identity and access management, providing SSO (Single Sign-On) capabilities.
- Offers centralized authentication, user federation, and social login support, enhancing the user authentication experience.

## Technologies Used

- **Spring Boot**
- **Spring Security**
- **OAuth2**
- **JWT (JSON Web Token)**
- **Keycloak**
- **Maven**

## Setup and Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/bank-application.git
   cd bank-application
   
2. **Set up Keycloak**:
   - Download and install Keycloak from [Keycloak Downloads](https://www.keycloak.org/downloads).
   - Start the Keycloak server and create a new realm, client, and users as needed.
   - Configure Keycloak settings in your Spring Boot application.

3. **Configure application properties**:
   Update `application.properties` or `application.yml` with your database, Keycloak, and other necessary configurations.

   ```properties
   # application.properties
   keycloak.realm=your-realm
   keycloak.resource=your-client
   keycloak.auth-server-url=http://localhost:8080/auth
   keycloak.credentials.secret=your-client-secret
   keycloak.ssl-required=external
   keycloak.bearer-only=true


4. **Build the project**:
    ```bash 
      mvn clean install

5. **Run the application**:
    ```bash
      mvn spring-boot:run


## Usage
  Access the application at http://localhost:8080.
  Use the Keycloak login page to authenticate users.
  Test the various endpoints with appropriate roles and permissions.


