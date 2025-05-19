
This class handles user account creation, including secure password hashing and salting using PBKDF2.  
Both the hashed password and the generated salt are stored in the SQL database:  
[UserAccount.cs](https://github.com/Markus9920/CSharp/blob/main/BudgetManager/Models/UserAccount.cs)

This controller manages user-related API endpoints such as account creation and login.  
It also handles token generation using JWT:  
[UserController.cs](https://github.com/Markus9920/CSharp/blob/main/BudgetManager/Controllers/UserController.cs) <br>
[TokenService.cs](https://github.com/Markus9920/CSharp/blob/main/BudgetManager/Services/TokenService.cs) <br>
[TokenValidationMiddleware.cs](https://github.com/Markus9920/CSharp/blob/main/BudgetManager/Services/TokenValidationMiddleware.cs)<br>

This controller allows users to add and manage recurring expenses.
It uses enums to define recurrence types and categories, which are also inserted into the database when new values are added.
This ensures that both the backend logic and the database remain aligned: [RecurrinExpenseController.cs](https://github.com/Markus9920/CSharp/blob/main/BudgetManager/Controllers/RecurrinExpenseController.cs) <br>

Defines the enum values for expense categories: [Categories.cs](https://github.com/Markus9920/CSharp/blob/main/BudgetManager/Models/Categories.cs) <br><br>
Processes the category enums and inserts them into the database.  
The integer value of each enum is used as the category ID.: [CategoryManager.cs](https://github.com/Markus9920/CSharp/blob/main/BudgetManager/Data/CategoryManager.cs)<br><br>
Enums that defines how frequently a recurring expense occurs: [RecurrenceType.cs](https://github.com/Markus9920/CSharp/blob/main/BudgetManager/Models/RecurrenceType.cs) [RecurrExpenseService.cs](https://github.com/Markus9920/CSharp/blob/main/BudgetManager/Services/RecurrExpenseService.cs)<br>
Makes a list of enums to show in frontend as strings: [ReferenceDataController.cs](http://github.com/Markus9920/CSharp/blob/main/BudgetManager/Controllers/ReferenceDataController.cs)

Most of the code in this repository was written or modified by me during the project.  
You can browse the full source code here:
[BudgetManager](https://github.com/Markus9920/CSharp/tree/main/BudgetManager)
