
- create a project folder and get inside
    - mkdir DotnetBoilerplate
    - cd DotnetBoilerplate

- create a new solution, add a new project under it
    - dotnet new sln --name DotnetBoilerplate
    - touch README.md
    - dotnet new webapi -o DotnetBoilerplate.API
    - dotnet sln add DotnetBoilerplate.API/DotnetBoilerplate.API.csproj
    - for a class lib: dotnet new classlib -o NameOfTheLib

- create folder structure
    - cd DotnetBoilerplate.API
    - mkdir Authorization Controllers Entities Helpers Models Models/Accounts Services