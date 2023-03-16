
- create a project folder and get inside
    - mkdir DotnetBoilerplate
    - cd DotnetBoilerplate

- create a new solution, add a new project under it
    - dotnet new sln --name DotnetBoilerplate
    - touch README.md -- for vim, :x to save exit, :q! force exit
    - dotnet new webapi -o DotnetBoilerplate.API
    - dotnet sln add DotnetBoilerplate.API/DotnetBoilerplate.API.csproj
    - for a class lib: dotnet new classlib -o NameOfTheLib
    - dotnet new gitignore
    
- create folder structure
    - cd DotnetBoilerplate.API
    - mkdir Authorization Controllers Entities Helpers Models Models/Accounts Services
    - considering: Migrations folder will be added by default
    - dotnet ef migrations add InitialCreate

- create necessary files
- Models
    - Accounts/AccountResponse.cs
    - Accounts/AuthenticateRequest.cs
    - Accounts/AuthenticateResponse.cs
    - Accounts/CreateRequest.cs
    - Accounts/ForgotPasswordRequest.cs
    - Accounts/RegisterRequest.cs
    - Accounts/ResetPasswordRequest.cs
    - Accounts/RevokeTokenRequest.cs
    - Accounts/UpdateRequest.cs
    - Accounts/ValidateResetTokenRequest.cs
    - Accounts/VerifyEmailRequest.cs

- Authorization
    - AllowAnonymousAttribute.cs
    - AuthorizeAttribute.cs
    - JwtMiddleware.cs
    - JwtUtils.cs


