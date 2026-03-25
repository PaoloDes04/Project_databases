# Askos Tours - Sistema Informativo per Tour Operator

**Askos Tours** è un sistema informativo realizzato con Django per la gestione completa dei tour, guide, clienti e prenotazioni. Il progetto supporta registrazione differenziata per clienti e staff, gestione dei tour, filtri per lingua, recensioni e dashboard personalizzate.

---

## 📌 Funzionalità Implementate

### 👤 Clienti
- Registrazione con codice fiscale, email, lingua preferita, telefono.
- Login tramite codice fiscale e password.
- Visualizzazione tour disponibili.
- Filtro tour per lingua preferita.
- Prenotazione tour (solo se la data è futura).
- Annullamento prenotazione (solo prima della data).
- Recensione tour già svolti (una sola per tour).
- Visualizzazione dei tour prenotati.

### 🧭 Staff (Guide / Driver)
- Registrazione con selezione multipla delle lingue parlate.
- Login tramite codice fiscale e password.
- Visualizzazione dei tour assegnati futuri (guida o driver).

### 🗺️ Tour
- Ogni tour è associato a:
  - una lingua
  - una o più guide
  - uno o più driver
- Visualizzazione dei partecipanti prenotati.
- Visibilità solo se la data è ancora futura.

### ⭐ Recensioni
- I clienti possono recensire solo i tour passati a cui hanno partecipato.
- Tutte le recensioni sono visibili pubblicamente in una pagina dedicata.

### 🔐 Amministratore (Admin)
- Gestione completa da pannello Django:
  - Tour
  - Clienti
  - Staff
  - Lingue
  - Prenotazioni
  - Recensioni

---

## ▶️ Come Avviare il Progetto

1. Esegui le migrazioni per creare le tabelle:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```
2. **Crea un superuser** per accedere al pannello admin:
   ```bash
   python manage.py createsuperuser
   ```
3. **Avvia il server Django:**
   ```bash
   python manage.py runserver
   ```
4. Accedi all'app da `http://127.0.0.1:8000/`.

---

## 👨‍🏫 Accessi Utente

- **Clienti**:
  - Registrazione autonoma tramite app.
  - Login con codice fiscale.

- **Staff** (Guida / Driver):
  - Registrazione autonoma con selezione lingue.
  - Accesso personalizzato per visualizzare i tour futuri.

- **Admin**:
  - Accesso da `http://127.0.0.1:8000/admin`
  - Aggiunta dei tour con assegnazione di titolo, durata, prezzo, lingua, guida e driver.
  - Gestione completa dei dati.

  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **Autore**:
  Paolo Desiderio 
  **Corso**:
  Basi di Dati(6 cfu)
**Università degli Studi di Napoli Parthenope**
🌍 Askos Tours - Tour Operator Information System


# Askos Tours - Tour Operator Information System

**Askos Tours** is an information system built with Django for the complete management of tours, guides, clients, and bookings. The project supports separate registration flows for clients and staff, tour management, language filters, reviews, and personalized dashboards.

---

## 📌 Implemented Features

### 👤 Clients
- Registration with Tax ID, email, preferred language, phone number.
- Login via Tax ID and password.
- Viewing available tours.
- Filtering tours by preferred language.
- Tour booking (only if the date is in the future).
- Booking cancellation (only before the date).
- Reviewing completed tours (only one per tour).
- Viewing booked tours.

### 🧭 Staff (Guides / Drivers)
- Registration with multiple selection of spoken languages.
- Login via Tax ID and password.
- Viewing assigned future tours (guide or driver).

### 🗺️ Tours
- Each tour is associated with:
  - one language
  - one or more guides
  - one or more drivers
- Viewing booked participants.
- Visibility only if the date is still in the future.

### ⭐ Reviews
- Clients can only review past tours they have attended.
- All reviews are publicly visible on a dedicated page.

### 🔐 Administrator (Admin)
- Complete management from the Django panel:
  - Tours
  - Clients
  - Staff
  - Languages
  - Bookings
  - Reviews

---

## ▶️ How to Start the Project

1. Run the migrations to create the tables:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```
2. **Create a superuser** to access the admin panel:
   ```bash
   python manage.py createsuperuser
   ```
3. **Start the Django server:**
   ```bash
   python manage.py runserver
   ```
4. Access the app at `http://127.0.0.1:8000/`.

---

## 👨‍🏫 User Access

- **Clients**:
  - Autonomous registration via the app.
  - Login with Tax ID.

- **Staff** (Guide / Driver):
  - Autonomous registration with language selection.
  - Personalized access to view future tours.

- **Admin**:
  - Access from `http://127.0.0.1:8000/admin`
  - Adding tours with assignment of title, duration, price, language, guide, and driver.
  - Complete data management.

  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **Author**:
  Paolo Desiderio 
  **Course**:
  Databases (6 cfu)
**University of Naples Parthenope**
🌍 Askos Tours - Tour Operator Information System
