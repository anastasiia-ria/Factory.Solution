# Dr. Sillystringz's Factory

#### Tracks Dr. Sillystringz's Factory engineers and machines

#### By [Anastasiia Riabets](https://github.com/anastasiia-ria)

## Technologies Used

- CSS
- HTML
- C#
- .NET 5.0
- ASP.Net
- Razor
- dotnet script REPL
- MySQL
- Workbench
- EF Core

## Description

Dr. Sillystringz's Factory lets owner to add and track their engineers and machines.
![Screen Shot](https://github.com/anastasiia-ria/Factory.Solution/blob/main/Factory/wwwroot/Images/screenshot.png?raw=true)

## Setup/Installation Requirements

- Clone this repository to your Desktop:
  1. Your computer will need to have GIT installed. If you do not currently have GIT installed, follow [these](https://docs.github.com/en/get-started/quickstart/set-up-git) directions for installing and setting up GIT.
  2. Once GIT is installed, clone this repository by typing following commands in your command line:
     ```
     ~ $ cd Desktop
     ~/Desktop $ git clone https://github.com/anastasiia-ria/Factory.Solution.git
     ~/Desktop $ cd Factory.Solution
     ```
- Install the [.NET 5 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/5.0)
- Install Packages for EF Core and a tool to update databases:
  ```
  ~/Desktop/Factory.Solution $ dotnet add package Microsoft.EntityFrameworkCore -v 5.0.0
  ~/Desktop/Factory.Solution $ dotnet add package Pomelo.EntityFrameworkCore.MySql -v 5.0.0-alpha.2
  ~/Desktop/Factory.Solution $ dotnet tool install --global dotnet-ef --version 5.0.1
  ```
- Create .gitignore file:
  ```
   ~/Desktop/Factory.Solution/ $ touch .gitignore
   ~/Desktop/Factory.Solution/ $ echo "*/obj/
   */bin/
   */appsettings.json" > .gitignore
  ```
- Create appsettings.json file:
  ```
   ~/Desktop/Factory.Solution $ cd Factory
   ~/Desktop/Factory.Solution/Factory $ touch appsettings.json
   ~/Desktop/Factory.Solution/Factory $ echo '{
      "ConnectionStrings": {
        "DefaultConnection": "Server=localhost;Port=3306;database=anastasiia_riabets;uid=root;pwd=[PASSWORD];"
      }
    }' > appsettings.json
  ```
  [PASSWORD] is your password
- Update Database:
  ```
  ~/Desktop/Factory.Solution/Factory $ dotnet ef database update
  ```
- Build the project:
  ```
   ~/Desktop/Factory.Solution/Factory $ dotnet build
  ```
- Run the project
  ```
   ~/Desktop/Factory.Solution/Factory $ dotnet run
  ```
- Visit [http://localhost:5000](http://localhost:5000) to try this application

## Known Bugs

- Layout is not adjusted for the small screens

## License

[ISC](https://opensource.org/licenses/ISC)

Copyright (c) 03/18/2022 Anastasiia Riabets
