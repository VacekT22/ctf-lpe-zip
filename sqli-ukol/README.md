# SQL Injection Write-up

## 1. Průzkum
Aplikace obsahuje vyhledávací pole s parametrem `search`.

Po zadání znaku ' do pole server vrátil SQL chybu, což znamená, že vstup není ošetřen proti SQL Injection.

## 2. Zjištění struktury databáze
Pomocí sqlmap bylo zjištěno:
- Databáze: SQLite
- Tabulky: users, config
- Počet sloupců: 2

## 3. Exfiltrace dat
Pomocí UNION SELECT byl získán obsah tabulky config:

' UNION SELECT NULL,value FROM config-- -

V tabulce byl nalezen záznam:
flag = FLAG{Sql_Un1on_M4st3r_S0SE}

## 4. Výsledek
FLAG{Sql_Un1on_M4st3r_S0SE}
