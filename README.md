#  School-ERP: A Django-Based School Management System

School-ERP is a robust web application built using the **Django framework** designed to manage and facilitate interactions between students and teachers within an educational institution.

## Key Features

This system streamlines essential academic processes for students and teachers:

* **Attendance Tracking:** Record and manage student attendance.
* **Marks/Grades Management:** Input and view student marks and performance data.
* **Timetable:** Access and manage class timetables.

---

##  Installation

To set up the School-ERP project, you need **Python** and the **Django framework** installed on your system.

### Prerequisites

* Python (3.x recommended)
* Django

### Installation Steps

1.  **Clone the repository:**
    ```bash
    git clone [Your Repository URL]
    cd School-ERP
    ```
2.  **Install Django:**
    Use `pip` to install the Django framework:
    ```bash
    pip install django
    ```
    *(Note: You might need to install other dependencies listed in a potential `requirements.txt` file, if present.)*

---

##  Usage

To start the local development server:

1.  Navigate into the main project directory (`College-ERP` in this context, assuming your project folder is named as such):
    ```bash
    cd College-ERP
    ```
2.  Run the Django development server:
    ```bash
    python manage.py runserver
    ```

### Accessing the System

Once the server is running, open your web browser and navigate to the following URL:
**[http://127.0.0.1:8000/](http://127.0.0.1:8000/)**

---

##  Login Details

The system features a common login page for both students and teachers.

| User Type | Username Format | Default Password |
| :--- | :--- | :--- |
| **Student** | Their full name (e.g., `'Rv Balaji Sai'`) | `'project123'` |
| **Teacher** | Their full name (e.g., `'B Sri Vaishnvai'`) | `'project123'` |

### Administrator Login (Django Admin)

The **Django Admin** interface allows for system configuration and database management.

* **URL:** **[http://127.0.0.1:8000/admin](http://127.0.0.1:8000/admin)**
* **Default Credentials:**
    * **Username:** `'admin'`
    * **Password:** `'project123'`

#### Creating a Superuser

To create a new administrator account (superuser), run the following command and follow the prompts:

```bash
python manage.py createsuperuser
```

##  User & System Management

All core system data, including user accounts, is managed via the **Django Admin page**.

### Managing Users

* New **Students** and **Teachers** must be added through the admin interface.
* A separate user account needs to be created for each new entry.

### Managing Data Tables

The admin page provides the interface to modify and manage all critical system tables, including:

* **Students**
* **Teachers**
* **Departments**
* **Courses**
* **Classes**
* *and more...*

---

##  Update: Attendance Time Range Reset (29/11/2025)

A new method has been added to the Django Admin page to reset the attendance period.

### Functionality

This feature allows the administrator to define a new **Start Date** and **End Date** for the attendance period. Executing this action will:

1.  **Delete** all currently existing attendance data.
2.  **Create** new attendance objects corresponding to the newly specified time range.

### Location

You can access this function in the Django Admin interface here:

> **Django Admin -> Attendance**
> **[http://127.0.0.1:8000/admin/info/attendanceclass/](http://127.0.0.1:8000/admin/info/attendanceclass/)**
