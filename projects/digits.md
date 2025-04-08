**Digits** is a contacts and notes management application I built as part of the ICS 314 course at the University of Hawaiʻi. Users can log in securely, add new contacts with details like name, address, image, and description, and attach notes to each contact to track interactions or personal reminders.
<img width="600px" class="rounded d-block mx-auto my-4" src="../doc/Landing.png">
<img src="doc/Landing.png">

Each user can only see and manage their own contacts and notes, while administrators can view all users and their contacts. The app uses modern technologies including **Next.js**, **Prisma ORM**, **PostgreSQL**, and **TypeScript** to ensure scalable, maintainable, and performant development.

---

### Installation Instructions

**Clone the repository:**

```bash
git clone https://github.com/mateoMaramara/digits.git
cd digits
```
**Install dependencies:**

```bash
npm install
```

**Push the Prisma schema and seed the database:**

```bash
npx prisma migrate dev --name init
npx prisma db seed
```
**Start the development server:**

```bash
npm run dev
```

Then open your browser to [http://localhost:3000](http://localhost:3000).

---

### User Interface Walkthrough

#### Landing Page

<img width="600px" class="rounded d-block mx-auto my-4" src="/doc/Landing.png">

When you visit the app, the landing page welcomes you with an interface and a prompts you to log in or register.

#### Register

New users can click **Login**, then **Sign Up** to create an account.

#### Sign In

Existing users can log in by clicking **Login → Sign In** and entering their credentials.

#### Home Page

After logging in, users are redirected to the home page with navigation options: **List Contacts**, **Add Contact**, and **Sign Out**.

#### Add Contact

<img width="600px" class="rounded d-block mx-auto my-4" src="../doc/Add.png">

Clicking **Add Contact** lets you input first name, last name, address, image URL, and a brief description to create a new contact.

#### List Contacts

<img width="600px" class="rounded d-block mx-auto my-4" src="../doc/Contacts.png">

The **List Contacts** page shows all your personal contacts. You can view their details, add notes, or edit them.

#### Add Notes

<img width="600px" class="rounded d-block mx-auto my-4" src="../doc/Note.png">
<img width="600px" class="rounded d-block mx-auto my-4" src="../doc/Note2.png">

Each contact has a form to add timestamped notes—ideal for tracking interactions or reminders.

#### Edit Contact

Click the **Edit** link under a contact to change any of their information.

#### Admin View

If logged in as an admin, a special **Admin** link appears in the navbar. It opens a page displaying all contacts from all users.

---

### 📸 Screenshots

**Home Page:**

<img width="600px" class="rounded d-block mx-auto my-4" src="../doc/Landing.png">

**Add Contact Page:**

<img width="600px" class="rounded d-block mx-auto my-4" src="../doc/Add.png">

**List Contact Page:**

<img width="600px" class="rounded d-block mx-auto my-4" src="../doc/Contacts.png">

**Add Note on Contact:**

<img width="600px" class="rounded d-block mx-auto my-4" src="../doc/Note.png">

**List Contact Page (with Notes):**

<img width="600px" class="rounded d-block mx-auto my-4" src="../doc/Note2.png">
