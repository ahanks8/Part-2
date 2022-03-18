# Part-2
<script>
    function calculation()
{
    var num1, num2, num3, sum, avg, product, result;

    num1 = parseInt(document.form.fnum1.value);
    num2 = parseInt(document.form.fnum2.value);
    num3 = parseInt(document.form.fnum3.value);

    sum = num1 + num2 + num3;
    avg = (num1 + num2 + num3)/3;
    product = num1 * num2 * num3;
    min = Math.min(num1, num2, num3);
    max = Math.max(num1, num2, num3);

   
    document.form.result1.value = sum;
    document.form.result2.value = avg;
    document.form.result3.value = product;
    document.form.result4.value = max;
    document.form.result5.value = min;
   
    }
  </script>
  <br>
 <form name="form">
  Input a value
  <input type="number" name="fnum1">
  Input a value
  <input type="number" name="fnum2">
  Input a value
  <input type="number" name="fnum3">
 <input type="button" value="submit" onclick="calculation()">
  <br>
  <br>
 The Sum of the 3 values are:
  <br>
  <input type="number" name="result1">
  <br>
 The Avgerage of the 3 values are:
  <br>
  <input type="number" name="result2">
  <br>
 The Product of the 3 values are:
  <br>
  <input type="number" name="result3">
  <br>
 The Highest Value of the 3 values is:
  <br>
  <input type="number" name="result4">
  <br>
 The Smallest Value of the 3 values is:
  <br>
  <input type="number" name="result5">
</form>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"> </script>
<script>
$(document).ready(function(){
  $("button").click(function(){
    $("#result1").fadeTo("slow", 0.15);
  });
});
</script>
<br>
<button>Click to fade boxes</button><br><br>
