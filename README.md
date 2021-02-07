# ezi_biznesy
ezi_biznesy był kiedyś skryptem napisanym dla serwera StrefaRP. Aczkolwiek kto wie, ten wie co się stało oraz dlaczego postanowiłem odeść ten wie.
ezi_biznesy był wzorowany na systemie biznesów tak naprawdę z jeszcze z czasów GTA SA:MP czy też na zagraniczynych serwera RageMP.
Skrypt był pisany w 2019r i patrząc przez pryzmat czasu, napisał bym go trochę inaczej no ale, może komuś się przyda.

**Uwaga:**
Skrypt nie jest dokończony w 100%. Owszem posiada podstawowe funkcje, które podkreślam "działały" w 2019r.
Proszę nie pisać do mnie na pw w celu pomocy, ponieważ i tak jej nie udzielę.

# Regulamin użytkowania
Regulamin użytkowania skryptu jest prosty, prośiłbym tylko o pozostawienie orginalnej nazwy oraz nie usunięcie moich komentarzy z skryptu. A reszte możecie edytować dowoli :) [licencja](https://github.com/Ezi2k/srp_businesses/blob/master/docs/LICENSE)

# Jak działa skrypt?
System biznesów działa w sposób następujący.<br>
Mamy pięć komend administracyjnych wymagana permisja (```_dev```):
- /bizcreate (nazwa) (marker id od 0 do 28) (cena: nie może być niższa niż 25000$) (status 0 - Na sprzedaż / 1 - Sprzedany / 2 - Wynajęty)
- /bizedit (id biznesu) (name/owner/price/locker/interior/doors/state) (w zależności od zmiennej, zmienimy dany parametr)
- /bizdelete (id biznesu) - Oczywiście mówi sama za siebie, usuwa biznes o podanym przez nas id.
- /bizinfo (debug) - Wyświetla dodatkowe informacje.
- /bizreload (przeładowanie wszystkich biznesów z bazy danych)

## Features
- Szafka biznesowa. (właściciel i współpracownicy mogą skorzystać z depozytu otwierającego / zamykającego oraz wyjmować z szafki takie przedmioty jak: broń / narkotyki itp.)
- Zamykanie drzwi (jeśli jesteś właścicielem firmy i naciśniesz **[L]** na klawiaturze, zablokujesz drzwi. Jeśli drzwi są zamknięte, nikt nie może wejść ani wyjść z Twojej firmy).
- Wchodzenie do interiorów (jeśli Twoja firma ma przypisany interior, możesz po prostu nacisnąć **[E]**, jeśli drzwi są odblokowane, zostaniesz teleportowany do interiora jeżeli naciśniesz **[E]** raz jeszcze raz i zostaniesz wy teleportowany z interiora. Mówiąc w prost, aby wejść kliknij **[E]** aby wyjść kliknij **[E]**)

## Komendy gracza
- /bizbuy (gracz musi znajdywać się w znaczniku biznesu, aby móc go kupić.)

## Jak dodać interiory?
To całkiem proste, musisz tylko dodać nowy interior w „config.lua”<br> 
np.
```lua
{ id = 1, coords = { x = -781.97, y = 326.31, z = 223.26 } }
``` 
ID oznacza identyfikator wewnętrzny, który wprowadzisz podczas edycji firmy za pomocą 
``/bizedit (id biznesu) (interior) (a następnie ID z config.lua)``
<br>
X,Y,Z to współrzędne gracza, do którego zostanie teleportowany po kliknięciu **[E]** na markerze firmy.
<br>
