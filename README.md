# PortfolioOptimizer-about


## Description

PortfolioOptimizer is tailored for investors managing a US stock portfolio, offering a solution to adjust the beta factor and/or Sharpe ratio to a desired level. Traditionally, investors would resort to manual calculations using paper, calculators, or Excel sheets, requiring constant data updates. However, PortfolioOptimizer provides a calculation tool accessible via a web interface. Users input their financial assets and investments, and the tool computes the necessary adjustments to achieve the desired beta or Sharpe ratio for the overall portfolio.

### Features:

- **Pages and Navigation**: Utilizes React Router for navigation between different sections, including a landing page, general information, and specific pages dedicated to understanding beta factor and Sharpe ratio. Navigation is facilitated through dropdown menus.

- **User Space**: Authenticated users access a personalized space where they can search for assets, set a main asset for portfolio calculation, manage a list of potential matching assets, and perform portfolio calculations.

- **Data Fetching**: No direct communication with external APIs is performed from the frontend, only via the backend (see below: Data Retrieval).

- **User Authentication**: Implemented using React with TypeScript, leveraging hooks like `useContext` to manage user sessions. No direct communication with external APIs is performed from the frontend.

- **Admin Functionality**: Administrators have access to a user management page in addition to regular user functionalities.

### Technology Stack:

- **Frontend**: Built with React in TypeScript, utilizing React Router for navigation.
  
- **Backend**: Developed using Spring Boot in Java, with an H2 database handling CRUD operations for users, assets, and portfolios.
  
- **Data Retrieval**: Financial data is fetched from the Alpha Vantage financial API via Spring WebFlux WebClient and stored in the database. Scheduled tasks (@Scheduled) ensure data updates.

- **Security**: Implemented Spring Security with JWT token authentication stored in cookies. A session API is available for frontend authentication checks.

- **Business Logic**: All business logic, including Sharpe ratio calculation and portfolio optimization, is handled on the backend. JUnit tests ensure the reliability of the logic.

## Screenshots (To be added)

Screenshots showcasing the interface and functionality will be added later for visual reference.
