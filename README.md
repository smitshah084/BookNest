# BookNest 📚🛒

## Tech stack 🧑‍💻

- Dotnet core mvc (.Net 8)
- MS SQLServer (Database)
- Entity Framework Core (ORM)
- Bootstrap 5 (frontend)

## How to run the project? 🌐

1. Open command prompt. Go to a directory where you want to clone this project. Use this command to clone the project.
   ```
     git clone https://github.com/smitshah084/BookNest
   ```
2. Go to the directory where you have cloned this project, open the directory. You will find a file with extenstion `.sln`. Double click on this file and this project will be opened in Visual Studio.
3. open `appsettings.json` file and update connection string

```
  "ConnectionStrings": {
    "conn": "data source=your_server_name;initial catalog=MovieStoreMvc; integrated security=true;encrypt=false"
  }
```

4. Delete `Migrations` folder
5. Open Tools > Package Manager > Package manager console
6. Run these 2 commands
   ```
    (i) add-migration init
    (ii) update-database
   ```
7. Now you can run this project

## How to register as admin and login?? 🧑‍💻🧑‍💻

1. Open the `Program.cs` file , you will find these commented lines

   ```c#
     //using(var scope = app.Services.CreateScope())
     //{
     //    await DbSeeder.SeedDefaultData(scope.ServiceProvider);
     //}

   ```

Uncomment these line and run the project. `Now stop the project and comment these lines again.`

2. Now click on login and login with these credentials.

   ```
     username: admin@gmail.com ,
     password: Admin@123
   ```
