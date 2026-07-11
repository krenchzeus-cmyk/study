<!doctype html>
<html>
  <head>
   <meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title></title>
</head>
<body>
<print>
    <!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
</head>
<body>
    <script>
        var firstName = prompt("Enter your first Name:");
        var lastName = prompt("Enter your last Name:");
        var birthyear = prompt("Enter your birthyear:");
        var numberofhours = prompt("Enter the Hours you studied:");

        if (
            firstName.trim() === "" ||
            lastName.trim() === "" ||
            birthyear.trim() === "" ||
            numberofhours.trim() === ""
        ) {
            alert("Error: ");
            console.log("Error: .");
        } else if (isNaN(birthyear) || birthyear < 1900 || birthyear > 2026) {
            alert("Error: Please enter a valid birth year between 1900 and 2026.");
            console.log("Error: Please enter a valid birth year between 1900 and 2026.");
        } else {
            var birthYear = parseInt(birthyear);
            var age = 2026 - birthYear;
            var stage = age < 18 ? "a minor." : "an adult.";
            var habit = numberofhours < 10 ? "Needs More Study Time." : "Good Study Habit."
            var message =
                "Hello! My Name is " +
                firstName +
                " " +
                lastName +
                "I am " + age
                + "years old and I am "
                + stage +
                " I study " + numberofhours
                + " hours per week."
                + " Study Evaluation: " + habit
            alert(message);
            console.log(message);
        }
    </script>
</body>
</html>
