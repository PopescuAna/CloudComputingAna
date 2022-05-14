# CloudComputingAna
# Prognoza meteo
> Aplicația meteo detecteaza cu exactitate prognozele meteo in locatia cautata.

## Cuprins
* [Descriere problema](#descriere-problema)
* [Interfata utilizator](#Interfata-utiliator)
* [Tehnologii](#tehnologii)
* [Descriere API](#descriere-api)
* [Autentificare si autorizare servicii utilizate](#autentificare)
* [Flux de date](#flux-date)
* [Referinte](#referinte)
* [Contact](#contact)

## Descriere problema
Prognoza meteo este foarte utila pentru toata lumea. Daca stiti informatii despre vreme, va puteti pregati planul cu atentie si nu veti fi luati prin surprindere de experiente neplacute.
Prognoza meteo este o aplicatie meteo care va permite sa gestionati vremea din mai multe locatii. Pe ecranul de intampinare, utilizatorii vad vremea locatiilor lor.
Utilizatorii pot adauga vreme in Londra, vremea din Paris, vremea din Milano sau chiar din Rusia, Ukraina, etc
Aplicatia isi propune sa prezinte vremea, in mod precis, a oricarei locatii pe care o cautati.

## Interfata utilizator
Introducere parametrii ( introducem locatia din tastatura pe pagina de intampinare)
![S1](https://user-images.githubusercontent.com/105311980/168428590-6c8b34ec-bf94-43ec-a4c7-e95d4e422073.png)
Obtinere rezultat
![S2](https://user-images.githubusercontent.com/105311980/168428603-a2daa5e4-6598-4a66-a69d-20cfffa608ba.png)
## Tehnologii
* Node.js
* JavaScript
* HTML
* CSS

## Descriere API
* API-ul utilizat întoarce un JSON cu vremea actuala a unei locatii.

Request (Metoda HTTP: GET ) la endpoint-ul:
`" https://api.openweathermap.org/data/2.5/weather?lat=30&lon=39&appid=8dd0f05b217aa7102df946880214e0e5 "`

Response:
`{"coord":{"lon":39,"lat":30},"weather":[{"id":803,"main":"Clouds","description":"broken clouds","icon":"04d"}],"base":"stations","main":{"temp":308.4,"feels_like":305.7,"temp_min":308.4,"temp_max":308.4,"pressure":1012,"humidity":10,"sea_level":1012,"grnd_level":949},"visibility":10000,"wind":{"speed":4.61,"deg":122,"gust":4.3},"clouds":{"all":74},"dt":1652529432,"sys":{"country":"SA","sunrise":1652495490,"sunset":1652544560},"timezone":10800,"id":109470,"name":"Al Jawf","cod":200}’

## Autentificare si autorizare servicii utilizate
API-ul utilizat este public, insa a fost necesar sa creez un cont pentru a obtine cheia respectiva.

## Flux de date
Utilizatorul introduce de la tastatura locatia pentru care doreste sa afle prognoza meteo.
Se face un request catre API, care intoarce un JSON ce contine prognoza meteo pentru locatia cautata din ziua curenta.
## Referinte
* https://openweathermap.org

## Contact
Aplicatie creata de catre popescu10maria18@stud.ase.ro. 
