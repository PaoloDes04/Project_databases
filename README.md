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
_------------
Askos Tours is a Django-based information system designed to manage tours, customers, staff, and bookings efficiently. It provides role-based access, language filtering, review management, and a complete administrative dashboard.
🚀 Features
👤 Customers
Register with tax code, email, preferred language, and phone number
Secure login (tax code + password)
Browse available tours
Filter tours by language
Book tours (future dates only)
Cancel bookings (before the tour date)
Leave one review per completed tour
View personal bookings
🧭 Staff (Guides / Drivers)
Register with multiple spoken languages
Login with tax code and password
View assigned upcoming tours
🗺️ Tours
Each tour includes:
Language
One or more guides
One or more drivers
View booked participants
Visible only if scheduled in the future
⭐ Reviews
Only customers who attended a tour can review it
Reviews are publicly displayed on a dedicated page
🔐 Admin Panel
Managed via Django Admin:
Tours
Customers
Staff
Languages
Bookings
Reviews
🛠️ Tech Stack
Backend: Django (Python)
Database: SQLite (default)
Frontend: HTML, CSS (Django Templates)
▶️ Getting Started
1. Clone the repository
Bash
git clone <your-repo-url>
cd askos-tours
2. Create virtual environment (recommended)
Bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
3. Install dependencies
Bash
pip install -r requirements.txt
4. Apply migrations
Bash
python manage.py makemigrations
python manage.py migrate
5. Create superuser
Bash
python manage.py createsuperuser
6. Run the server
Bash
python manage.py runserver
7. Open in browser

http://127.0.0.1:8000/
👥 User Roles
Customers
Self-registration via application
Login using tax code
Staff (Guide / Driver)
Self-registration with language selection
Access to assigned tours
Admin
Access: http://127.0.0.1:8000/admin
Full system management
📂 Project Structure (simplified)
Bash
askos_tours/
│── manage.py
│── askos_tours/
│── tours/
│── users/
│── bookings/
│── reviews/
📌 Future Improvements
Payment integration
Email notifications
REST API (Django REST Framework)
Mobile app integration
👨‍💻 Author
Paolo Desiderio
🎓 Course
Database Systems (6 ECTS)
🏫 University
University of Naples Parthenope