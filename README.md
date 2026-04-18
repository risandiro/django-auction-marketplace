# django-auction-marketplace

Full-stack Django tržiště s komiksy a aukcemi: uživatelé mohou vkládat inzeráty, podávat příhozy, spravovat sledované položky a procházet podle kategorie. Přihlášení a registrace, Autentizace, Uživatelské účty. Postaveno jako webová aplikace (**Django + SQLite**).

---

## Funkce

- Registrace, přihlášení a odhlášení uživatele (vlastní uživatelský model)
- Vytváření inzerátů s názvem, popisem, URL obrázku, vyvolávací cenou a kategorií
- Aktivní / uzavřené inzeráty; po uzavření vyhrává nejvyšší příhoz
- Podávání příhozů s validací (musí překonat aktuální příhoz a splnit minimum)
- Sledované: přidávání/odebírání inzerátů a rychlý přístup z navigace
- Komentáře u inzerátů
- Stránky kategorií a přehled „všechny kategorie“
- Django admin pro správu obsahu (volitelné)

## Živá ukázka

**[https://flask-serpapi-export-tests.onrender.com]([https://flask-serpapi-export-tests.onrender.com](https://risandiro.pythonanywhere.com))**

(některé funkce fungují jen po přihlášení)

## Technologie

- **Python 3**
- **Django** 3.x
- **SQLite** (vývoj)
- **HTML / CSS** (Django šablony)

### Požadavky

- Doporučeno Python 3.8.5+
- Závislosti: `django`, `sqlite3`

## Lokální spuštění

```bash
git clone https://github.com/risandiro/commerce.git
cd commerce
pip install django
python manage.py migrate
python manage.py runserver
