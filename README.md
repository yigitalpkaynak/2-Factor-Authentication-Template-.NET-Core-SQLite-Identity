This project was made with .Net 7.0
Check the IdentityApp.csproj to make sure you have correct sdk files, SQ Lite and .Net Packages. 

To use this project, you have to use this commands in order.

"libman restore" to add bootstrap library
"dotnet ef database drop --force"
"dotnet ef migrations add InitialCreate"
"dotnet ef database update"

after, you should enter the "EmailSender" datas of your own server information in appsettings.Development.json

you can change the default user information at "user = new AppUser at IdentitySeedData.cs

Finally "dotnet watch" to launch project.
