
---

# Bright Smile Dental Management

## Project Setup
1. **Clone the repository from Github:**
   ```bash
   git clone https://github.com/Araviraj8/dental_management.git
   cd dental_management
   ```

2. **Install the dependencies from requirement.txt:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Environment variable configurations:**
   - Install and configure PostgreSQL.
   - Create a database and user for the application
   - Create `.env` file and paste the below:
     ```plaintext
     DB_NAME=your_db_name
     DB_USER=your_db_user
     DB_PASSWORD=your_db_password
     DB_HOST=localhost
     DB_PORT=5432
     ```

4. **Migrate the database:**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Create a superuser:**
   ```bash
   python manage.py createsuperuser
   ```

6. **Run Server:**
   ```bash
   python manage.py runserver
   ```

## Running the Application
The Application runs successfully at  [http://localhost:8000]. 

## List of APIs:
  **Login**: `/api/login/`
  **Logout**: `/api/logout/`
  **List Clinics**: `/api/clinics/`
  **Add Clinic**: `/api/clinics/add/`
  **Clinic Details**: `/api/clinics/<clinic_id>/`
  **Edit Clinic**: `/api/clinics/<clinic_id>/edit/`
  **List Doctors**: `/api/doctors/`
  **Add Doctor**: `/api/doctors/add/`
  **Doctor Details**: `/api/doctors/<doctor_id>/`
  **Edit Doctor**: `/api/doctors/<doctor_id>/edit/`
  **List Patients**: `/api/patients/`
  **Add Patient**: `/api/patients/add/`
  **Patient Details**: `/api/patients/<patient_id>/`
  **Schedule Visit**: `/api/patients/<patient_id>/visit/`
  **Fetch Available Clinics and Doctors by Specialty**: `/api/specialty/<specialty_id>/doctors-clinics/`

