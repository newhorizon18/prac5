# Experiment No. 5

## Title: Program Using JavaScript to Validate an Email Address

## 1. Program Code

**File Name: index.html**

```html
<!DOCTYPE html>
<html>

<head>
    <title>Email Validation</title>

    <script>
        function validateEmail() {

            var email =
                document.getElementById("email").value;

            // Check presence of @ and .
            if (email.indexOf("@") === -1 ||
                email.indexOf(".") === -1) {

                alert(
                    "Invalid Email! '@' and '.' are required."
                );

                // Clear input field
                document.getElementById("email").value = "";

                // Ask user to re-enter
                document.getElementById("email").focus();

                return false;
            }

            alert("Email is valid!");

            return true;
        }
    </script>

</head>

<body>

    <h2>Email Validation Using JavaScript</h2>

    <form onsubmit="return validateEmail()">

        <label>Enter Email:</label>

        <input type="text" id="email" required>

        <br><br>

        <input type="submit" value="Validate">

    </form>

</body>
</html>
```

## 2. Aim

To write a JavaScript program to validate an email address by checking the presence of the `@` and `.` characters.

## 3. Theory

- **JavaScript:** Used to make webpages interactive.
- **Email Validation:** Checks whether the entered email follows a basic format.
- **getElementById():** Accesses an HTML element using its ID.
- **indexOf():** Searches for a character in a string.
- **alert():** Displays a popup message.
- **if-else Condition:** Helps check whether the email is valid or invalid.

## 4. Output

### Invalid Email

**Input:**

```text
studentgmailcom
```

**Alert Message:**

```text
Invalid Email! '@' and '.' are required.
```

### Valid Email

**Input:**

```text
student@gmail.com
```

**Alert Message:**

```text
Email is valid!
```

## 5. Conclusion

Thus, a JavaScript program was successfully implemented to perform basic email validation.

The program checks for the presence of `@` and `.` and displays an appropriate alert message.
