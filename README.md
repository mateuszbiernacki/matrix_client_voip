# matrix_client_voip
Student project for Poznan University of Technology.


## Charakterystyka ogólna projektu
Projekt zakłada rozszerzenie funkcjonalności komunikatora tekstowego przygotowywanego na inny przedmiot, o rozmowy głosowe pomiędzy klientami. Istotna będzie kwestia bezpieczeństwa -- odpowiednie szyfrowanie (zapewne strumieniowe).
## Architektura systemu.
Wstępnie zakładamy serwer przechowujący loginy i odpowiednio długie hasze haseł użytkowników. Użytkownicy musieliby z poziomu klientów połączyć się z serwerem, zalogować i zainicjować połączenie głosowe ze sobą (za pomocą nazwy użytkownika, o ile ten zaakceptował wcześniej zaproszenie do znajomych). Kodowanie i szyfrowanie oraz deszyfrowanie i dekodowanie dźwięku w czasie możliwie zbliżonym do rzeczywistego to zadanie aplikacji klienckich. W takim połączeniu może brać udział tylko jedno urządzenie na stronę.
## Wymagania funkcjonalne.
*	Rejestracja użytkownika.
*	Logowanie użytkownika.
*	Zmiana hasła.
*	Wysyłanie zaproszenia do kontaktów.
*	Akceptacja zaproszenia do kontaktów.
*	Odrzucenie zaproszenia do kontaktów.
*	Usuwanie z kontaktów.
*	Zablokowanie zaproszeń do kontaktów od określonego użytkownika.
*	Zablokowanie zaproszeń do kontaktów od kogokolwiek.
*	Próba nawiązania połączenia z wybranym kontaktem.
*	Odrzucenie przychodzącego połączenia.
*	Tryb "nie przeszkadzać", uniemożliwiający nawiązanie z klientem połączenia.
*	Przyjęcie przychodzącego połączenia.
*	Wyciszenie swojego mikrofonu.
*	Wyciszenie rozmówcy.
*	Przerwanie trwającego połączenia.
## Wymagania niefunkcjonalne.
*	Tylko jeden użytkownik o podanej nazwie.
*	Określona maksymalna długość nazwy użytkownika.
*	Określona minimalna i maksymalna długość hasła.
*	Przechowywanie haszy haseł, z dodanym, zmiennym saltem.
*	Komunikacja full-duplex.
*	Komunikacja jedynie pomiędzy dwoma użytkownikami (brak rozmów grupowych).
*	Poufność, integralność i uwierzytelnianie transmisji.
*	Rejestrowanie jedynie dźwięków powyżej określonego nątężenia.
*	Jakość głosu zmienna, w zależności od przepływności transmisji.
*	Jeśli czas dostarczenia danego pakietu transmisji będzie powyżej określonej wartości, nie zostanie on przetworzony (zabezpieczenie przed rozsynchronizowaniem rozmowy).
*	Klient powinien posiadać minimalistyczny, czytelny interfejs graficzny z ciemnym motywem.
