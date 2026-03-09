

# SimpleForum – Prosjektoppgave IT

## Om prosjektet

Dette prosjektet er en enkel forum / sosiale medier-side laget med Flask og MariaDB.
Brukere kan registrere seg, logge inn og skrive meldinger som andre brukere kan lese.

Prosjektet er laget som en del av en IT-prosjektoppgave hvor vi skal vise ferdigheter innen utvikling, drift og brukerstøtte.

---

## Mål med prosjektet

Målet er å lage en webapplikasjon som:

* lar brukere registrere seg
* lar brukere logge inn og ut
* lar brukere skrive meldinger
* viser meldinger fra andre brukere
* lagrer data i en database

Nettsiden skal kjøre på en server med Flask og bruke MariaDB for å lagre data.

---

## Teknologi brukt

Dette prosjektet bruker følgende teknologi:

* Python
* Flask
* MariaDB
* HTML
* CSS
* GitHub
* Linux / virtuell maskin

---

## Funksjoner

### Bruker

* registrere bruker
* logge inn
* logge ut

### Forum

* skrive melding
* lese meldinger
* slette egen melding (valgfritt)

Dette dekker også CRUD-funksjoner:

* **Create** – skrive melding
* **Read** – lese meldinger
* **Update** – redigere melding (kan legges til senere)
* **Delete** – slette melding

---

## Database

Prosjektet bruker MariaDB med to tabeller.

### users

Lagrer informasjon om brukere.

| Felt     | Type    |
| -------- | ------- |
| id       | INT     |
| username | VARCHAR |
| password | VARCHAR |

### posts

Lagrer meldinger i forumet.

| Felt       | Type     |
| ---------- | -------- |
| id         | INT      |
| user_id    | INT      |
| message    | TEXT     |
| created_at | DATETIME |

---

## Infrastruktur

Systemet fungerer slik:

Bruker → Nettleser → Flask webserver → MariaDB database

Serveren kjører på en Linux virtuell maskin.

---

## Prosjektstruktur

```
forum-project/

app.py
database.sql
requirements.txt

templates/
    index.html
    login.html
    register.html

static/
    style.css

README.md
```

---

## Plan for utvikling

### 1. Planlegging

* Lage GitHub repository
* Lage prosjektplan
* Planlegge database

### 2. Infrastruktur

* Installere Python
* Installere Flask
* Installere MariaDB
* Opprette database

### 3. Backend

Programmere funksjoner i Flask:

* registrering
* login system
* lagre meldinger
* hente meldinger fra databasen

### 4. Frontend

Lage nettsider med HTML og CSS:

* login side
* registrering
* forumside

### 5. Testing

Teste at:

* brukere kan registrere seg
* login fungerer
* meldinger lagres i databasen
* meldinger vises på siden

### 6. Dokumentasjon

Lage dokumentasjon for prosjektet:

* README
* nettverksdiagram
* brukerveiledning
* installasjonsguide

---

## Brukerveiledning

1. Gå til nettsiden
2. Registrer en bruker
3. Logg inn
4. Skriv en melding i forumet
5. Meldingen vises for andre brukere

---

## Oppsett av prosjektet

1. Installer Python

2. Installer Flask

```
pip install flask
```

3. Installer MariaDB

```
sudo apt install mariadb-server
```

4. Opprett databasen med `database.sql`

5. Start programmet

```
python app.py
```

---

## Videre forbedringer

Mulige forbedringer senere:

* redigere meldinger
* profilside for brukere
* bedre design
* bildeopplasting
