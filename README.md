![hmrs_mssql_diagram](https://user-images.githubusercontent.com/73183005/117718833-52389880-b1e5-11eb-8948-fe0668ff1782.PNG)
![hmrs_mssql_diagram](https://user-images.githubusercontent.com/73183005/117718853-59f83d00-b1e5-11eb-9491-9cb89ca3c49b.PNG)
# kodlamaio_hmrs_database_design
Engin Demiroğ hocamın anlattığı ders'te öğretilen tam anlamı ile SOLID prensiplerine göre VeriTabanı (Database) oluşturma yapıldı. 
MS-SQL Server 2019 -SQL Server Management toolu kullanıldı. 
Tüm tablolar oluşturulduktan sonra söylenen alanlara Unique(tekil) indeksler tanımlanarak  aynı verilerden oluşum engellendi.
Users  (Base-temel) Tablo olarak yaratıldı.
JobSeekers - İş Arayanlar 
Employers   - İş verenler
Employees  - Elemanlar (Bizim şirketin personelleri) tabloları bu ana tablodan kalıtım aldı.
VerificationEmails - Doğrulama e-mailleri ile ilgili bilgileri  (UserId) , ve verificationCode tutan bir tablo geleceğe yönelik olarak oluşturuldu.
Positions -  İş Pozisyonları tablosu oluşturuldu. Şimdilik Employees tablosunda PositionId alanı ile ilişki kuruldu. (Gelecekte mutlaka farklı operasyonlarda kullanılacaktır*)
Diyagram MS-SQL ile oluşturuldu.  (daha net ve anlaşılır bir görüntüsü var)
daha sonra 'hmrs'  veritabanı (database) i    FullConvert adlı program aralığı ile 
PostgreSql  de açılan hmrs tablosuna taşındı.  2. Diyagram eki nda pg4Admin
ERD Toolu ile oluşturulmuş tur. ( Generate ERD (Beta) - ekte gösterilmiştir.
Gençlerin ve arkadaşların incelemesi ve faydalı olması amacı ile...

![hmrs_mssql_diagram](https://user-images.githubusercontent.com/73183005/117718902-6da3a380-b1e5-11eb-9f86-757799ddf453.PNG)
