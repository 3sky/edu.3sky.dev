---
title: Konfiguracja środowiska
weight: 2
---

## Wybierz swój system

Uf to chyba będzie najtrudniejszy roździał tego kursu. Będziesz zmuszony drogi czytelniku
skonfigurowania sobie samodzielnie środowiska pracy. Pewnie zastanawisz się od czego zacząć? 
Najpierw musimy określić system operacyjny którego używasz. Teoretycznie mamy 3 opcje.
[Windows](#windows), [GNU/Linux](#GNU), oraz [MacOS](MacOS). Warto podkreślić, że systemów operacyjnych jest wiele
i może tutaj nie być poradnika dla Ciebie. Zakładam jednak, że w takiej sytuacji jesteś w stanie
poradzić sobie bez niego :) 

## Windows

Windows jak to Windows nie od dzisiaj najpopularniejszym systemem operacyjnym jest. Ładny, dość stabilny
od jakiegoś czasu wspiera [WSL](https://docs.microsoft.com/en-us/windows/wsl/). I ten oto kawałek oprogramowania
będzie Twoim nowym przyjacielem. Jak zainstalować Windows Subsystem for Linux? To proste. Wystarczy skorzystatać z
[dokumentacji](https://docs.microsoft.com/en-us/windows/wsl/install). Jeżeli to za dużo postaram się to wytłumaczyć przyjaźniej
i po polsku.

#### Wymagania wstępne

- Musisz używać Windowsa 10 wersja 2004 lub nowszego(Build 19041), ewentualnie Windowsa 11.
- Musisz mieć uprawnienia admistratorskie na swojej staji roboczej

---
**Jak sprawdzić numer builda?** 

*Naciśnij przycisk z logo Windowsa jednocześnie wciskając R(duże R - SHIFT + r), wpisz `winver`, a następnie kliknij OK*
---

#### Instalacja 

1. Otwórz Windowsowy wiersz poleceń.
1. Naciśnij przycisk z logo Windowsa jednocześnie wciskając X(duże X - SHIFT + x), aby otworzyć Power Users menu, następnie kliknij “Command Prompt (Admin).”
1. Wprowadź komende `wsl --install`, po czym zatwierdź jej wywołanie klawiszem ENTER.
1. Wybrana komenda zainstaluję WSL oraz wszystkie wymagane komponenty. 
1. WSL będzie teraz interpretował znaczą cześć komend dostępnych w systemie operacyjnym o nazwie [Ubuntu](https://ubuntu.com/)

#### Konfiguracja

Wszystkie kroki można również znaleść na stronie [Microsoftu](https://docs.microsoft.com/en-us/windows/wsl/setup/environment#set-up-your-linux-user-info).

1. Wybierz z menu Start nową apliakcję o nazwe Ubuntu.
1. Czarne okno zapyta Cie o stworzenie użytkownika oraz hasła.
1. Polecam wybranie prostego usernamu np. `adam`.
1. Hasło natomiast, powinno być trudniejsze niż `test1234`, warto mieć jednak na uwadzę, że będziesz je dość często wykorzystywał.
1. Jeżeli wszystko poszło zgodnie z planem wpisz w wiersz poleceń nastepujący ciąg komend `sudo apt update && sudo apt upgrade`.
1. Co robi dany ciąg znaków? Aktualizauję pakiety i instaluję ich najnowsze wersje. Dokładniej zajmiemy się tym później.
1. Tym razem proszę o odrobine zaufania i potwierdzenie komendy klawiszem ENTER.

#### Gratulację !

Udało Ci się skonfigurować WSL i zaktualizować podstawowe pakiety. Yayyy ! 
