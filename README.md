# projekt_3


Soubory v projektu:
projekt_3.py: Hlavní skript pro získávání, parsování a ukládání dat o hlasování.
requirements.txt: Seznam závislostí pro Python.

Požadavky:
Projekt vyžaduje Python 3 a následující Python balíčky:
requests
beautifulsoup4

Vysvětlení skriptu
Získání HTML:
Funkce fetch_html přijímá URL adresu a vrací HTML obsah stránky.

Parsování odkazů na obvody:
Funkce parse_district_links extrahuje a vrací odkazy na stránky obvodů z hlavní stránky.

Parsování výsledků hlasování:
Funkce parse_voting_results parsuje výsledky hlasování ze stránky obvodu a vrací hlavičku a řádky dat.

Uložení do CSV:
Funkce save_to_csv zapisuje hlavičku a řádky dat do CSV souboru.

Hlavní funkce:
Funkce main organizuje skript tím, že získá hlavní stránku, parsuje odkazy na obvody, získá a parsuje každou stránku obvodu a uloží kombinované výsledky do CSV souboru.

Spuštení kodu: py projekt_3.py "https://volby.cz/pls/ps2017nss/ps32?xjazyk=CZ&xkraj=2&xnumnuts=2101" vysledky_kraj.csv
