# Clean Architecture Template

This project is a clean architecture template developed using .NET 8. It comprises specific packages used in each layer of the project. Below, you can find more information about the project components and the packages employed.

## Project Layers

1. **Domain Layer:**
   - This layer contains the business logic and is independent of the outside world. No external packages are used in this layer.

2. **Application Layer:**
   - This layer is where the business logic is implemented, and application-specific rules are defined.
   - Used Packages:
     - [MediatR](https://github.com/jbogard/MediatR): Used for handling events and requests.
     - [FluentValidation](https://fluentvalidation.net/): Utilized for specifying and enforcing input validation rules.

3. **Infrastructure Layer:**
   - This layer provides access to external resources such as databases and external services. No external packages are used in this example.

4. **WebApi Layer:**
   - This layer provides an API that interacts with users and manages input/output operations.
   - Used Packages:
     - [Serilog](https://serilog.net/): Used for logging purposes.
     - [Microsoft.Extensions.DependencyInjection](https://docs.microsoft.com/en-us/dotnet/core/extensions/dependency-injection): Used for dependency injection.

## How to Run?

1. To install project dependencies, run the following command in the terminal or command prompt:
   ```bash
   dotnet restore
2. Navigate to the WebApi folder within the project and start the application using the following command:
   ```bash
   dotnet run
