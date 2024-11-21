# Back End Module Project

## Situation

For the backend module, I created a <strong>Personal Finance Management App</strong>. The purpose of this app was to allow users to:

<ul>
    <li>Sign up and create an account.</li>
    <li>Open an account and perform transactions like deposits and withdrawals.</li>
    <li>Generate a report to view account information and all related transactions in an easy-to-read format.</li>
</ul>

## Task

As this was a backend-only project, my tasks included:

<ul>
    <li><strong>Creating models</strong>: Developed multiple models to represent entities such as accounts, transactions, and users.</li>
    <li><strong>Implementing CRUD operations</strong>: Developed methods to create, read, update, and delete records for each model.</li>
    <li><strong>Building API endpoints</strong>: Created API endpoints to interact with the database and call these methods, enabling users to:
        <ul>
            <li>Perform various actions on their accounts.</li>
            <li>View personalized account and transaction details.</li>
        </ul>
    </li>
</ul>

## Action

This app was a solo project, so I had to set up everything myself, including making the connection to the database, creating the models, setting up the associations to other models, and creating the API routes.

<p> --<strong>Account model</strong> which has associations to User, Budget, and Transaction</p>
<img src="../BackendProject/ImagesBP/AccountScreenshot.png" alt="Account model screenshot" />

<p> --<strong>Service Method</strong> for creating a new account, which will then be called by the API to create the account in the database</p>
<img src="../BackendProject/ImagesBP/AddNewAccount.png" alt="Add new account service method" />

<p> --<strong>Method</strong> that creates a user and hashes and salts the password for protection</p>
<img src="../BackendProject/ImagesBP/UserRegisterMethod.png" alt="User registration method with password hashing and salting" />

## Result

<a href = "https://github.com/andrewozo/PersonalFinanceManagementProject">Repo Link</a>

# Technologies

<ul>
    <li>C#</li>
    <li>.NET</li>
</ul>

## Job Competencies

<p><strong>JF 3.6 Can implement a RESTful API</strong><br>
In this project, I had endpoints like GET, POST, PUT, and DELETE that, when called, would send requests to the database and return data in the form of JSON.</p>

<p><strong>JF 3.7 Can implement authentication and authorization to an API</strong><br>
In order for a user to access the API, they would need to have proper authorization. Without it, they would not be able to make API calls. To gain access, the user would have to create an account, and after creating an account and signing in, a token would be generated that would allow them to make API calls.</p>

<p><strong>JF 3.8 Can encrypt sensitive data via hashing</strong><br>
Whenever a new user creates an account, their password is hashed and salted before being stored in the database.</p>
