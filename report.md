# Web Application Pentest Report – User Registration Security Review

## Overview
Ten raport opisuje zidentyfikowane problemy bezpieczeństwa związane z procesem rejestracji użytkowników w aplikacji webowej.

## Scope
Zakres testów obejmował:
- formularz rejestracji użytkownika
- możliwość edycji danych użytkownika po rejestracji
- walidację danych wprowadzanych przez użytkownika

## Identified Issues
System nie weryfikuje danych po stronie serwera i ufa danym przesyłanym z formularza, przyjmuje bardzo słabe hasła podczas rejestracji oraz pozwala na zmianę danych użytkownika bez odpowiedniej weryfikacji.

## Impact
Opisane problemy mogą prowadzić do przejęcia lub utraty kontroli nad kontami użytkowników, co skutkuje naruszeniem prywatności, utratą zaufania do aplikacji oraz potencjalnymi stratami wizerunkowymi i prawnymi dla organizacji.

## Recommendations
Aplikacja powinna każdorazowo weryfikować dane po stronie serwera, niezależnie od etapu ich wprowadzania, wymuszać stosowanie odpowiednio silnych haseł oraz wymagać potwierdzenia i walidacji przy każdej zmianie danych użytkownika, takich jak adres email.
