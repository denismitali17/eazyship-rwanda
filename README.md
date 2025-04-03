
---

# **📦 EazyShip Rwanda - Smart Logistics Management**  

**Welcome to EazyShip Rwanda!** This is a **modern shipping and logistics platform** built to simplify **shipment tracking, management, and delivery operations** in Rwanda.  

Whether you're a **casual user** tracking your shipments or an **admin managing multiple orders**, EazyShip Rwanda provides a **seamless experience** with real-time updates and a **powerful admin dashboard**.  

---

## **🌟 Features**  

✔ **Sign Up & Log In** – Create an account and securely log in.  
✔ **Track Shipments** – See where your package is in real-time.  
✔ **Manage Orders** – View history and status of shipments.  
✔ **Admin Dashboard** – Manage users, shipments, and analytics.  

📢 **Coming Soon:** Live tracking and email notifications!  

---

## **🛠 How to Set Up EazyShip Rwanda (Step-by-Step Guide)**  

### **1️⃣ Prerequisites**  
Before you begin, make sure you have the following installed on your computer:  

✅ **Node.js (v18+)** → [Download Node.js](https://nodejs.org/)  
✅ **npm or yarn** → Comes with Node.js  
✅ **PostgreSQL** → [Download PostgreSQL](https://www.postgresql.org/download/)  
✅ **Git** → [Download Git](https://git-scm.com/)  

### **2️⃣ Clone the Repository**  
Open your **terminal (Command Prompt, Git Bash, or Terminal on macOS/Linux)** and run:  

```bash
git clone https://github.com/denismitali17/eazyship-rwanda.git
```

Now, navigate into the project folder:  

```bash
cd eazyship-rwanda/frontend
```

---

### **3️⃣ Install Project Dependencies**  
Run the following command to install all required packages:  

```bash
npm install
```

If you're using **yarn**, use:  

```bash
yarn install
```

---

### **4️⃣ Set Up Environment Variables**  
EazyShip uses **environment variables** to store **database credentials** and **authentication secrets**.  

1. **Create an `.env` file** in the `frontend/` directory:  
```bash
cp .env.example .env
```

2. **Edit the `.env` file** and update the values:  

```env
DATABASE_URL=your_postgresql_connection_string
NEXTAUTH_SECRET=your_nextauth_secret_key
NEXTAUTH_URL=http://localhost:3000
```

📌 **Where do I get these values?**  
- `DATABASE_URL`: If using PostgreSQL locally, it might look like this:  
  ```
  postgresql://username:password@localhost:5432/eazyship
  ```
- `NEXTAUTH_SECRET`: Generate a secret with this command:  
  ```bash
  openssl rand -base64 32
  ```
- `NEXTAUTH_URL`: If running locally, set it to:  
  ```
  http://localhost:3000
  ```

---

### **5️⃣ Set Up the Database**  
Since EazyShip uses **PostgreSQL**, you need to create the database and apply migrations.  

1. **Make sure PostgreSQL is running** on your system.  
2. Run the following command to create the database tables:  

```bash
npx prisma migrate dev
```

💡 This will apply all **database schema changes** and create the necessary tables.  

To view your database structure, you can also run:  

```bash
npx prisma studio
```

---

### **6️⃣ Start the Development Server**  
Run the following command to **start the server**:  

```bash
npm run dev
```

After a few seconds, your project will be **live on:**  

```bash
http://localhost:3000
```

---

### **7️⃣ Testing the Setup**  
To ensure everything is working correctly:  

- **Sign up** as a new user  
- **Log in** and track shipments  
- **Visit the Admin Dashboard** (only if you have an admin account)  

If everything works, **you're good to go!** 🎉  

---

## **🔧 Tech Stack**  

### **Frontend (User Interface)**  
- **Next.js 14** – Fast & SEO-friendly  
- **React** – Component-based UI  
- **TypeScript** – Type-safe code  
- **Tailwind CSS** – Beautiful, responsive styles  
- **Heroicons** – Stylish icons  

### **Backend (Server & Database)**  
- **Next.js API Routes** – Server-side logic  
- **Prisma ORM** – Database interaction  
- **NextAuth.js** – Secure authentication  
- **PostgreSQL (via Supabase)** – Data storage  



---

## **🔐 Security Features**  

✔ **Encrypted Passwords** – Uses bcrypt to store passwords securely.  
✔ **Role-Based Access** – Admins have higher privileges.  
✔ **Secure Authentication** – Login protected with NextAuth.js.  
✔ **CSRF Protection** – Prevents security threats.  

---

## **🌍 Environment Variables Reference**  

| Variable            | Description                         | Example Value  |
|--------------------|---------------------------------|--------------|
| `DATABASE_URL`     | PostgreSQL database connection | `postgresql://user:password@localhost:5432/eazyship` |
| `NEXTAUTH_SECRET`  | Secret key for authentication  | `your_generated_secret_key` |
| `NEXTAUTH_URL`     | App URL (local or live)        | `http://localhost:3000` |

---

## **🚀 What's Next? (Upcoming Features)**  

🔜 **Live Shipment Tracking** – Know exactly where your package is in real-time!  
🌍 **Multi-Language Support** – Making EazyShip accessible to everyone.  
📧 **Enhanced Email Notifications** – Get alerts for shipment updates.  

---

## **🤝 Want to Contribute?**  

We **welcome open-source contributors!** Follow these steps:  

1. **Fork the repository**  
2. **Create a feature branch** (`git checkout -b feature-name`)  
3. **Commit your changes** (`git commit -m "Description of changes"`)  
4. **Push to GitHub** (`git push origin feature-name`)  
5. **Create a Pull Request**  

Your contributions **help improve EazyShip for everyone!** 🚀  

---

## **📄 License**  

This project is licensed under the **MIT License**, meaning **you can use, modify, and distribute it freely!**  

---

## **📞 Contact & Support**  

📧 **Email:** d.mitali1@alustudent.com

🌐 **Website:** 

📍 **Made with ❤️ in Rwanda**  

---

### **👏 Thank you for using EazyShip Rwanda! Let's revolutionize logistics together! 🚚✨**  

---
