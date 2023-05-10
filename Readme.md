# Integratasi SSO IdAMAn dengan NET Core Balzor Assembly untuk WEB dan API

## Sources
Go to ->



## Registrasi Aplikasi 
Daftarkan aplikasi yang akan menggunakan IdAMan seperti berikut:

1. Buka aplikasi IdAMan QA  <https://identity.qa.idaman.pertamina.com/> 
1. Masuk ke menu Applications -> new Applications

Isikan,
Name: SPA - Blazor Assembly Example
redirect URL: <https://localhost:5001/authentication/login-callback>
Type: Single Page / Mobile
Company: Pertamina Persero

Seperti pada gambar berikut:

Kemudian submit, maka pada list aplikasi akan muncul daftar aplikasi Balzor Asembly Example, klik dan lihat detail nya.

1. Define scope untuk API
       - Enable API

       - Add new scope
## WEB Projects

1. Setup configurations di wwwroot/appsettings.json


1. Pada project API set up Authorization URL dan Scope nya Program.cs

1. Run project donet run -> running project in <https://localhost:5001> 





Klik button login -> page akan meredirect ke halaman Login IdAMan












1. Show claims -> [BlazorClient](https://localhost:5001/claims)




## API Project
1. Set configutation in Startup.cs


1. Run project -> dotnet run -> [](https://localhost:5002/whe) https://localhost:5002/WeatherForecast

##
