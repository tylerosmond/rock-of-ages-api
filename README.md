# Django REST API - Rock of Ages

## Notes

There are no views, models, or serializers in this boilerplate project. The only code that is included is the ability to register and login. The `urls.py` file already imports the required functions from `views/auth.py`.

## Getting Started

1. Clone this repository and `cd` to the project directory
2. Run `pipenv shell`
3. Run `pipenv install`
4. Run `python3 manage.py migrate` to create the default Django tables in your database
5. Open the project directory in VS Code
6. Press <kbd>⌘</kbd><kbd>SHIFT</kbd><kbd>P</kbd> (Mac), or <kbd>Ctrl</kbd><kbd>SHIFT</kbd><kbd>P</kbd> (Windows) to open the Command Palette, and select "Python: Select Interpreter".
4. Search for "rock" and select the interpreter that starts with those characters. There should only be one to choose from.
7. Start the debugger
   1. Mac: **Shift+Option+D**
   2. Windows: **Shift+Alt+D**
8. Verify that the process starts with no exceptions
9. Open Postman and create a POST request to http://localhost:8000/register with the following JSON body and verify that you can create a new user and get a token in the response body -
   ```json
   {
      "email": "admina@straytor.com",
      "password": "straytor",
      "first_name": "Admina",
      "last_name": "Straytor"
   }
   ```
