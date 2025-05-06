# 👨‍💻 Technical Interview Task: Django + Flutter – Basic User CRUD (GET & POST)

This task evaluates your ability to build a simple full-stack application using **Django (backend)** and **Flutter (frontend)**. You will implement a minimal REST API and a Flutter app to **retrieve** and **add users**.

---

## 🧱 PART 1: BACKEND (Django)

### 🎯 Objective

Set up a Django REST API that supports:

* ✅ Retrieve all users (`GET /api/users/`)
* ✅ Add a new user (`POST /api/users/`)

### 📌 Instructions

1. **Create a Django project** named `user_api`.
2. **Create an app** within the project called `users`.
3. Use Django’s built-in `User` model from `django.contrib.auth.models`.
4. **Install Django REST Framework** and configure it.
5. Implement API endpoints using DRF:

   * `GET /api/users/` – Return a list of all users.
   * `POST /api/users/` – Create a new user (e.g., with username, email, and password).
6. Use `django-cors-headers` to allow requests from the Flutter frontend.
7. Make your API publicly accessible via [ngrok](https://ngrok.com/) or similar tunneling tool.
8. Test your endpoints using Postman, Insomnia, or `curl`.

---

## 📱 PART 2: FRONTEND (Flutter)

### 🎯 Objective

Create a Flutter mobile app to interact with the Django API:

* ✅ Fetch and display all users.
* ✅ Add a new user using a form.

### 📌 Instructions

1. Create a Flutter project named `user_crud_app`.
2. Choose a state management approach (e.g., **Provider**, **Riverpod**, or **Bloc**).
3. Build two screens:

   * **User List Screen** – Fetch and display users from the API.
   * **Add User Screen** – Form to input user data and submit a POST request.
4. Use Dart’s `http` package (or another package of your choice) to make network calls.
5. Connect to your Django backend using the public `ngrok` URL.
6. Include:

   * Form validation
   * Error handling
   * Loading indicators

---

## ✅ Submission Tips

* Keep code modular and well-structured.
* Focus on functionality and clarity.
* Add minimal comments or documentation if necessary.
* Provide run instructions for both backend and frontend.
