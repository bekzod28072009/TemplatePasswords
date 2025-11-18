# 🔐 Auth Template – C# .NET Web API  
A clean and simple template for **Login**, **Forgot Password**, and **Change Password** functionality in your C# .NET Web API projects.

This template is designed to help developers quickly integrate essential authentication features without setting up everything from scratch. Perfect for beginners, students, and teams building modern authentication flows.

---

## ✨ Features

- ✔ **User Login**  
- ✔ **Forgot Password** workflow (email sending logic included / ready to integrate)  
- ✔ **Change Password** (with old password validation)  
- ✔ Clean service–repository architecture  
- ✔ DTO-based request handling  
- ✔ Strong validation and structured responses  
- ✔ Ready for JWT integration  
- ✔ Easily extendable

---

## 📁 Project Structure

/AuthTemplate
├── Controllers
│ └── AuthController.cs
├── Services
│ └── AuthService.cs
├── Interfaces
│ └── IAuthService.cs
├── DTOs
│ ├── LoginDto.cs
│ ├── ForgotPasswordDto.cs
│ └── ChangePasswordDto.cs
├── Models
│ └── User.cs
├── Utils
│ └── PasswordHasher.cs
└── README.md

---

## 🚀 How to Use

1. **Clone the template**
   ```bash
   git clone https://github.com/your-repo/auth-template
Update your database connection
Edit appsettings.json with your own SQL or PostgreSQL connection.

Run migrations

dotnet ef database update
Run the API


dotnet run
🔑 Endpoints
POST /api/auth/login
Authenticate user and return JWT token.
Body:

json
{
  "email": "example@mail.com",
  "password": "string123"
}
POST /api/auth/forgot-password
Sends reset link / or starts reset workflow.
Body:

json
{
  "email": "example@mail.com"
}
POST /api/auth/change-password
Change password using the old password.
Body:

json
{
  "userId": "id-here",
  "oldPassword": "oldpass",
  "newPassword": "newpass123"
}
🧩 Technologies Used
.NET 7 / .NET 8 / .NET 9 (your choice)

Entity Framework Core

Fluent Validation

JWT Authentication (optional)

Layered Architecture

👨‍💻 Why This Template?
Saves time when starting new projects

Ensures clean and correct password handling

Helps beginners understand how login/password flows really work

Can be directly copied into any existing Web API solution

🤝 Contributing
Pull requests are welcome!
If you want to add Token refresh, Email confirmation, or OTP login — feel free to enhance the template.

📜 License
This project is open-source and free to use for any personal or commercial purpose.

⭐ If you like this template, don't forget to give it a star!
yaml
---

Let me know if you want **badges**, **screenshots**, **colored sections**, or **ASCII logo** added.
