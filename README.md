<!DOCTYPE html>
<html>
<head>
 <title>Factorial Calculator</title>
</head>
<body>
 <h2>Factorial Calculator</h2>
 <form method="post">
 <input type="number" name="number" placeholder="Enter a number" 
required>
 <button type="submit">Calculate</button>
 </form>
 <?php
 // Function to calculate factorial
 function factorial($n) {
 $result = 1;
 for ($i = 1; $i <= $n; $i++) {
 $result *= $i;
 }
 return $result;
 }
 // Check if the form was submitted
 if (isset($_POST['number'])) {
 $number = $_POST['number'];
 // Call the factorial function
 $factorial = factorial($number); DEPARTMENT OF COMPUTER SCIENCE
 // Display the result
 echo "<p>Factorial of $number is $factorial.</p>";
 }
 ?>
</body>
</html> DEPARTMENT OF COMPUTER SCIENCE
OUTPUT
Factorial Calculator
Enter a numbe
Factorial of 10 is 3628800
Calculate
localhost/fact.php
Factorial Calculator
Calculate
Factorial of 6 is 720.
