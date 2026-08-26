# 🏥 Hospital Management System

A simple **Hospital Management System developed in Python** using **Object-Oriented Programming (OOP)** concepts.

This project allows users to manage patients, doctors, and appointments through a simple menu-driven console application.

## 📌 Project Overview

The Hospital Management System is designed to demonstrate the practical implementation of Python OOP concepts.

The project includes:

* 👨‍⚕️ Doctor Management
* 🧑‍🤝‍🧑 Patient Management
* 📅 Appointment Booking
* 📋 Viewing Patients
* 📋 Viewing Doctors
* 📋 Viewing Appointments
* 🚪 Exit Option

The project uses classes such as `Person`, `Patient`, `Doctor`, `Appointment`, and `Hospital`.

---

## 🎯 Objectives

The main objectives of this project are:

1. To understand Object-Oriented Programming in Python.
2. To implement classes and objects.
3. To demonstrate inheritance.
4. To demonstrate encapsulation.
5. To demonstrate polymorphism.
6. To create a practical console-based application.
7. To manage hospital-related information using Python.

---

## 🛠️ Technologies Used

| Technology | Purpose                                  |
| ---------- | ---------------------------------------- |
| Python     | Application Development                  |
| OOP        | Program Structure                        |
| Lists      | Storing Patients, Doctors & Appointments |
| Console    | User Interaction                         |

---

## 🧠 OOP Concepts Used

### 1. Encapsulation

Patient and person information is encapsulated using private attributes such as:

```python
self.__name = name
self.__age = age
```

Getter methods are used to access the data:

```python
def get_name(self):
    return self.__name

def get_age(self):
    return self.__age
```

This helps protect the internal data of the object.

---

### 2. Inheritance

The `Patient` and `Doctor` classes inherit from the `Person` class.

```python
class Patient(Person):
```

and

```python
class Doctor(Person):
```

The `super()` function is used to initialize the attributes of the parent class.

Relationship:

```text
             Person
             /    \
            /      \
       Patient    Doctor
```

---

### 3. Polymorphism

Both `Patient` and `Doctor` classes contain their own `display()` method.

```python
def display(self):
```

The same method name behaves differently depending on the object calling it.

For example:

```text
Patient.display() → Displays patient information

Doctor.display()  → Displays doctor information
```

This demonstrates polymorphism in Python.

---

### 4. Classes and Objects

The project uses multiple classes:

```text
Person
Patient
Doctor
Appointment
Hospital
```

The `Hospital` class maintains lists for patients, doctors, and appointments.

---

## ⚙️ Features

### 👤 Add Patient

The system accepts:

* Patient Name
* Age
* Disease

The patient is then added to the hospital's patient list.

### 👀 View Patients

Displays all registered patients.

Example:

```text
Patient: Sagar, Age: 28, Disease: Fever
```

### 👨‍⚕️ Add Doctor

The system accepts:

* Doctor Name
* Age
* Specialization

The doctor is then added to the doctor list.

### 🔎 View Doctors

Displays all registered doctors.

Example:

```text
Doctor: Shivam, Age: 30, Specialization: xyz
```

### 📅 Book Appointment

Users can enter:

* Patient Name
* Doctor Name
* Appointment Date

The appointment is stored in the appointment list.

### 📋 View Appointments

Displays the appointments stored in the system.

---

## 🖥️ Menu

The application provides the following menu:

```text
================================
   HOSPITAL MANAGEMENT SYSTEM
================================

1. Add Patient
2. View Patients
3. Add Doctor
4. View Doctors
5. Book Appointment
6. View Appointments
7. Exit
```

The menu continuously runs until the user selects **Exit**.

---

## 📂 Project Structure

```text
Hospital-Management-System/
│
├── hospital_management.py
├── README.md
└── OOPS.pdf
```

---

## 🚀 How to Run

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/Hospital-Management-System.git
```

### Step 2: Open the Project

```bash
cd Hospital-Management-System
```

### Step 3: Run the Python Program

```bash
python hospital_management.py
```

---

## 💻 Sample Output

```text
HOSPITAL MANAGEMENT SYSTEM

1. Add Patient
2. View Patients
3. Add Doctor
4. View Doctors
5. Book Appointment
6. View Appointments
7. Exit

Enter Choice: 1

Patient Name: Sagar
Age: 28
Disease: Fever

Patient Added Successfully.
```

Example doctor output:

```text
Doctor Added Successfully.

Doctor: Shivam, Age: 30, Specialization: xyz
```

The uploaded project demonstrates these sample interactions.

---

## 🔄 Program Flow

```text
                START
                  │
                  ▼
       Hospital Management System
                  │
                  ▼
            Display Menu
                  │
       ┌──────────┼───────────┐
       ▼          ▼           ▼
 Add Patient   Add Doctor   Appointment
       │          │           │
       ▼          ▼           ▼
 Store Data   Store Data   Store Data
       │          │           │
       └──────────┼───────────┘
                  ▼
             View Data
                  │
                  ▼
             Exit Program
```

---

## 📚 Learning Outcomes

After completing this project, you can understand:

* Python classes and objects
* Constructors
* Encapsulation
* Inheritance
* Polymorphism
* Method overriding
* Lists and objects
* User input handling
* Menu-driven programs
* Basic project structure

---

## 🔮 Future Improvements

The project can be further improved by adding:

* 🔐 Login and authentication
* 💾 Database integration using MySQL
* 🩺 Medical history
* 💊 Prescription management
* 💰 Billing system
* 🔍 Search patient/doctor functionality
* ✏️ Update and delete records
* 🖥️ GUI using Tkinter
* 🌐 Web application using Flask or Django

---

## 👨‍💻 Author

**Sagar Garad**

Computer Engineering Student

Python | OOP | Data Analytics | SQL

---

## ⭐ Project Status

**Completed — Basic Console-Based Hospital Management System**

If you find this project useful, consider giving the repository a ⭐.
