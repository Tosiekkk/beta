# PROJEKT
## Zadanie 1 - OSINT
### Warszawski Uniwersytet Medyczny
1. Pobrałem plik ```index.html```, dzięki czemu zdobyłem adres IP strony.  
![1](1.png)  
2. W pliku ```index.html``` znalazłem także strony WUM na różnych serwisach  
![2](/OSINT/2.png)  
3. Na stronie znalazłem adres organizacji, telefon centralny, faks a także numer *NIP* i *REGON*  
![3](3.png)  
4. Następnie znalazłem informacje o aktualnym rektorze, jego mail, a także życiorys wraz z zainteresowaniami zawodowymi i prywatnymi oraz znanymi mu językami i używane systemy operacyjne. Plik z życiorysem zamieszczam w repozytorium ![Plik](/OSINT/rektor_info.pdf).  
![4](4.png)  
![5](5.png)  
5. Następnie znalazłem takie same informacje o wszystkich prorektorach  
![6](6.png)  
![7](7.png)  
6. Za pomocą narzędzia ```theharvester``` znalazłem kilkadziesiąt adresów mail oraz ponad dwieście subdomen wraz z ich adresami IP.  
![8](8.png)  
![9](9.png)  
![10](10.png)  
7. Znalazłem liczbę wyników sybdomen w wyszukiwarce *Google*  
![11](11.png)  
8. Użyłem narzędzia ```whois``` do znalezienia zakresu IP dla sieci tej organizacji  
![13](13.png)  
9. Porównałem wyniki z bazą danych ```whois``` na stronie dns.pl/whois. Dzięki temu znalazłem nazwy i adresy IP ich serwerów, a także adres rejestratora.  
![12](12.png)  
10. Użyłem narzędzia ```netcraft``` i uzyskałem subdomeny, a także inne informacje takie jak używany algorytm hashowania (sha256)  
![14](14.png)  
![23](23.png)  
11. Użyłem narzędzia ```shodan.io```, które znalazło pewne podatności i potwierdziło znalezioną wcześniej metodę hashowania  
![15](15.png)  
![16](16.png)  
![17](17.png)  
12. Dzięki stronie archive.org znalazłem pierwszą wersję strony z 2007 roku, a także z kolejnych lat.
![18](18.png)  
13. Za pomocą narzędzia ```whois``` znalazłem prawdopodobną lokalizację geograficzną serwerów  
![19](19.png)  
14. Za pomocą polecenia ```cache:wum.edu.pl``` znalazłem informacje w cache'u wyszukiwarki *Google*  
![21](21.png)  
15. Za pomocą skryptu *Bash* przeszukałem plik ```index.html``` w poszukiwaniu subdomen. Wykonałem także skanowanie za pomocą ```recon-ng```, uzyskując kolejne subdomeny wraz z ich adresami IP (w każdym źródle były pewnie subdomeny, których nie znalazłem za poomocą innych narzędzi)  
![20](20.png)  
![22](22.png)  
cos tam
