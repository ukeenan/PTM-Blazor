# Integratasi SSO IdAMAn dengan NET Core Balzor Assembly untuk WEB dan API

## Sources
File explorer

![](Aspose.Words.0bedd40d-dc42-4d68-bd0d-d213eaac42f1.001.png)


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

![](Aspose.Words.0bedd40d-dc42-4d68-bd0d-d213eaac42f1.002.png)

Kemudian submit, maka pada list aplikasi akan muncul daftar aplikasi Balzor Asembly Example, klik dan lihat detail nya.

![](Aspose.Words.0bedd40d-dc42-4d68-bd0d-d213eaac42f1.003.png)

1. Define scope untuk API
       - Enable API
   ![](Aspose.Words.0bedd40d-dc42-4d68-bd0d-d213eaac42f1.004.png)
       - Add new scope
## WEB Projects

1. Setup configurations di wwwroot/appsettings.json

![](Aspose.Words.0bedd40d-dc42-4d68-bd0d-d213eaac42f1.005.png)

1. Pada project API set up Authorization URL dan Scope nya Program.cs

   ![](Aspose.Words.0bedd40d-dc42-4d68-bd0d-d213eaac42f1.006.png)

1. Run project donet run -> running project in <https://localhost:5001> 

![](Aspose.Words.0bedd40d-dc42-4d68-bd0d-d213eaac42f1.007.png)

Klik button login -> page akan meredirect ke halaman Login IdAMan

![](Aspose.Words.0bedd40d-dc42-4d68-bd0d-d213eaac42f1.008.png)

1. Show claims -> [BlazorClient](https://localhost:5001/claims)

![](Aspose.Words.0bedd40d-dc42-4d68-bd0d-d213eaac42f1.009.png)
## API Project
1. Set configutation in Startup.cs

![](Aspose.Words.0bedd40d-dc42-4d68-bd0d-d213eaac42f1.010.png)

1. Run project -> dotnet run -> [](https://localhost:5002/whe) https://localhost:5002/WeatherForecast

##
