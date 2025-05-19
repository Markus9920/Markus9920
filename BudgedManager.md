
This class handles user account creation, including secure password hashing and salting using PBKDF2.  
Both the hashed password and the generated salt are stored in the SQL database. 
[UserAccount.cs](https://github.com/Markus9920/CSharp/blob/main/BudgetManager/Models/UserAccount.cs)

This controller manages user-related API endpoints such as account creation and login.  
It also handles token generation using JWT.  
[UserController.cs](https://github.com/Markus9920/CSharp/blob/main/BudgetManager/Controllers/UserController.cs)
[TokenService.cs](https://github.com/Markus9920/CSharp/blob/main/BudgetManager/Services/TokenService.cs)
This controller allows users to add and manage recurring expenses.  
It uses enums to define recurrence types and categories, ensuring clean and consistent data handling.
[]()

Most of the code in this repository was written or modified by me during the project.  
You can browse the full source code here:
[]()
