# 👨‍💻 Technical Interview Task: Django + Flutter – User CRUD

This task is designed to evaluate your ability to build a full-stack application from scratch. You will set up a Django REST API to manage user data and create a Flutter mobile application that interacts with this backend. The goal is to assess your skills in setting up projects, managing data flow, and implementing CRUD operations across both backend and frontend.

---

## 🧱 PART 1: BACKEND (Django)

### 🎯 Objective

Build a REST API using Django that allows basic CRUD operations on user data.

### 📌 Steps

1. **Create a new Django project** named `user_api`.

2. **Create a Django app** inside the project called `users`.

3. **Use Django’s built-in User model** (`from django.contrib.auth.models import User`) to manage user records. You may customize it with additional fields if desired.

4. **Install and configure Django REST Framework** to build the API. Expose the following endpoints:

   * `GET /api/users/` – Retrieve a list of all users
   * `POST /api/users/` – Create a new user
   * `GET /api/users/<id>/` – Retrieve details of a specific user
   * `PUT /api/users/<id>/` – Update a user
   * `DELETE /api/users/<id>/` – Delete a user

5. **Enable CORS** using `django-cors-headers` to allow requests from the Flutter frontend.

6. **Expose your API publicly** using [ngrok](https://ngrok.com/) or any other tunnel tool so the Flutter app can connect during development.

7. **Test all endpoints** using a tool like Postman or cURL before moving to the frontend.

---

## 📱 PART 2: FRONTEND (Flutter)

### 🎯 Objective

Build a Flutter application that interacts with your Django backend API to perform user CRUD operations.

### 📌 Steps

1. **Create a new Flutter project** named `user_crud_app`.

2. **Choose a state management solution** such as Provider, Riverpod, or Bloc to manage your app's state.

3. **Build the following screens:**

   * A home screen to **list all users** (GET request)
   * A screen or modal to **add a new user** (POST request)
   * A screen or modal to **edit an existing user** (PUT request)
   * Include the ability to **delete users** directly from the list (DELETE request)

4. **Connect the Flutter app to your Django API** using the public URL you generated via ngrok.

5. **Ensure proper error handling, loading indicators, and form validations.**

6. **Use Dart's `http` package** (or any other client) to make network calls.

---

## 🧪 Tips

* Organize your code with proper file structure.
* Ensure your code is readable and logically structured.
* Prioritize functionality and clean architecture over UI polish.
* Reuse widgets and avoid code duplication.
* Use Flutter DevTools or console logs for debugging.

---

Feel free to use any additional libraries or packages you are comfortable with, but keep your solution understandable and easy to run for review.
