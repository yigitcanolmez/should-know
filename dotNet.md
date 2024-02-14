# Entity Framework Migration

MacOS sistemlerde sıklıkta kullanmaktayım;

dotnet ef migrations add initial -- X.DataAccess(DbContext bulunan projeniz) --startup-project X.API

dotnet ef database update --project X.DataAccess --startup-project X.API

************************************************************************

# DotNet CLI
dotnet help => neler yapılabileceğini görürsün.

dotnet new ile istediğin projeyi oluşturabilirsin.
* ardından --name denirse proje ismi tanımlanabilir.
* eğer aynı isimle açılan bir proje varsa ve yeni açacağın proje ile eski olan projeyi ezmek istiyorsan -- force keywordunü kullanabilirsin.

dotnet restore => referansı kaldırılan paketlerin restorasyonunu sağlar.

dotnet build => .exe ve .dll çıktılarını verir. Build hemen öncesinde restore işlemi yapar.

dotnet publish => projeyi yayınlanabilir hale getirir.

dotnet run => uygulama derler ve ayağa kaldırır.

# Proje Kodları
Referans dediğimiz projemizde olan .dll uzantılı dosyalardır. Amacı, ilgili dosyanın başka bir yazılım tarafında kullanılmasını sağlar. Daha iyi anlamlandırmak adına; son kullanıcı .exe dosyasını açıp, uygulamayı kullanıyorsa. Farklı bir yazılım gelip bizim .dll dosyamızı kullanabiliyor, referans dediğimiz kavram bu anlama gelmektedir.

Uygulamanıza NuGet'ten bir paket yüklemeniz için => dotnet add package

silmek için ise dotnet remove package

Uygulamanıza bir referans eklemeniz için => dotnet add source.csproj reference target.csproj

silmek için dotnet remove refernce [reference name]

Referans edilen tüm paketleri listelemek adına => dotnet list reference
