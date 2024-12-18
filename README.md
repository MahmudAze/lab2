# lab2

### Regex əsaslı Sistem Log Analizi
a. Regex-dən istifadə edərək verilmiş access_log.txt faylından URL-ləri və onlara uyğun HTTP status kodlarını çıxarın.
b. 404 status kodu ilə URL-ləri müəyyən edin və hər birinin neçə dəfə göründüyünü hesablayın.

### Fayl manipulyasiyası
a. URL-lərin siyahısını status kodları ilə birlikdə url_status_report.txt adlı mətn faylında saxlayın.
b. URL-ləri 404 xəta ilə CSV faylında (malware_candidates.csv) sütunlarla yadda saxlayın: URL, 404-lərin sayı.

### Veb Scraping
a. Təhdid kəşfiyyatındakı ən son qara siyahıya alınmış domenləri silin (nümunə HTML təqdim olunur).
b. Jurnal faylındakı URL-ləri qara siyahıdakı domenlərlə müqayisə edin və hər hansı uyğunluğu müəyyənləşdirin.

### JSON məlumatların idarə edilməsi
a. Uyğun qara siyahıya alınmış URL-lərin təfərrüatlarını və onların statusunu və hadisələrin sayını özündə saxlayan JSON faylı (alert.json) yaradın.
b. Aşağıdakı məlumatlarla ayrıca JSON faylında (summary_report.json) xülasə hesabatı yaradın:

#### Verilmiş qara siyahıda olan domenlər:
 - malicious-site.com
 - phishing-example.net
 - blacklisteddomain.com

#### Verilmiş loqlar:
 - 192.168.1.100 - - [05/Dec/2024:09:15:10 +0000] "GET http://malicious-site.com/page1 HTTP/1.1" 404 4321
 - 192.168.1.101 - - [05/Dec/2024:09:16:20 +0000] "GET http://example.com/page2 HTTP/1.1" 200 5432
 - 192.168.1.102 - - [05/Dec/2024:09:17:30 +0000] "GET http://blacklisteddomain.com/page3 HTTP/1.1" 404 1234
 - 192.168.1.103 - - [05/Dec/2024:09:18:40 +0000] "POST http://malicious-site.com/login HTTP/1.1" 404 2345

#### Nəticə etibarilə

##### verilən:
access_log.txt
thread_feed.html

##### tapşırıqda istənilən:
url_status_report.txt           - Bütün URL-ləri və onların status kodlarını sadalayın.
malware_candidates.csv          - 404 səhvli URL-ləri və onların saylarını sadalayın.
alert.json                      - Qara siyahıya salınmış uyğun URL-ləri saxlayın.
summary_report.json             - Təhlilin nəticələrini ümumiləşdirin.
