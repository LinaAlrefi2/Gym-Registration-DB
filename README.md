# Gym Registration System

Welcome to the **Gym Registration System**! This system is designed to manage member registrations, workout plans, coaches, classes, and dependents in a gym environment. The system is built using SQL to store and manage data for various gym activities, ensuring seamless registration and interaction for gym members.

---

## 🌟 Key Features

1. **Member Registration**: Register gym members, store personal information, and assign them to a chosen package.
2. **Package Management**: Manage gym membership packages that include details such as cost, duration, and description.
3. **Workout Plans**: Track and manage workout plans that members can participate in, including coaches, classes, and associated details.
4. **Coaches Management**: Store information about coaches, including their contact details, salary, and assigned workout plans.
5. **Classes Management**: Schedule and manage gym classes by storing class details, including date, time, and class name.
6. **Branch Management**: Track the gym branches where members are registered, including branch locations and offered services.
7. **Dependent Management**: Allow members to register their dependents (children) for care services at the gym.

---

## 📊 Database Structure

The system is built on an SQL database and includes the following entities:

- **Members**: Contains information about gym members such as name, contact information, age, and package registration details.
- **Packages**: Represents different membership packages offered by the gym, including the name, cost, period, and description.
- **Workout Plans**: Details about available workout plans, including plan description, start/end dates, and the associated coach and classes.
- **Coaches**: Information about gym coaches, including their personal details, salary, and classes they lead.
- **Classes**: Represents gym classes with class name, date, and time.
- **Branches**: The different branches of the gym, where members can register.
- **Dependents**: Child dependents of the gym members, storing their personal information for care services at the gym.

---



## 📋 Business Rules

- **Member Registration**: Each member must register for a **Package** and choose a **Branch**. The registration date will be stored in the system when a member is registered.
  
- **Package Selection**: A member is assigned to one **Package** upon registration. Each package has a unique ID, name, cost, and description.
  
- **Workout Plan Participation**: Members can participate in specific **Workout Plans**. Each plan has a start date, end date, price, and description. Workout plans include **Coaches** and **Classes**.

- **Coach Information**: Coaches are responsible for leading **Classes** and are associated with **Workout Plans**. Each coach has a salary and contact details.

- **Class Scheduling**: Classes have unique IDs, names, and scheduled times. Members can sign up for classes available under their workout plans.

- **Branch Information**: A member must select one **Branch** where they will register. Each branch has an address and a list of services or **Offers**.

- **Dependent Care**: Each member can have up to several **Dependents**. The gym offers care services for dependents, and the personal details of the dependents are stored in the system.

---

## 🚀 Getting Started

To use the Gym Registration System:

1. **Set up the Database**:
   - Create a new SQL database and run the provided schema SQL scripts to create the tables.
   - Ensure all necessary relationships (foreign keys) are established between tables.

2. **Use SQL Queries**:
   - **Insert Members**: Add new members using `INSERT INTO` statements for the `Members` table.
   - **Register for Packages**: Link members to packages using `UPDATE` to set `Package_ID` for each member.
   - **Add Dependents**: Use `INSERT INTO` to add dependents for each member.
   - **Workout Plans & Classes**: Add new workout plans and classes, associating them with the right coach and member.

---



## 🛠 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for more details.

---

## 🙏 Acknowledgements

Special thanks to the community for supporting open-source databases and gym management systems.

---

With the **Gym Registration System**, managing members, packages, workout plans, coaches, and dependents becomes straightforward and efficient. Let’s get started with a healthier future! 🏋️‍♂️💪
