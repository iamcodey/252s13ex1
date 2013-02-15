<!DOCTYPE html>
<html>

<head>
<script>
function validateForm()
{
var x=document.forms["Exam"]["Ad1"].value;
if (x==null || x=="")
   {
   alert("All Required Fields Not Filled");
   return false;
   }
 }
var x=document.forms["Exam"]["email"].value; 
var atpos=x.indexOf("@");
var dotpos=x.lastIndexOf(".");
if (atpos<1 || dotpos<atpos+2 || dotpos+2>=x.length)
  {
  alert("All Required Fields Not Filled");
  return false;
  }
var y=document.forms["Exam"]["zip"].value;
if (y.length!=5)
  {
  alert("All Required Fields Not Filled");
  return false;
  }
}

</script>
</head>
<body>
<form name="myForm" action="demo_form.asp" onsubmit="return validateForm()" method="post">
Address 1: <input type="text" name="Ad1"><br>
Address 2: <input type="text" name="Ad2"><br>
City: <input type="text" name="city">
<select name="states">
<option value="Alabama">AL</option>
<option value="Alaska">AK</option>
<option value="Arizona">AZ</option>
<option value="Arkansas">AR</option>
<option value="California">CA</option>
<option value="Colorodo">CO</option>
<option value="Connecticut">CT</option>
<option value="Delaware">DE</option>
<option value="Florida">FL</option>
<option value="Georgia">GA</option>
<option value="Hawaii">HI</option>
<option value="Idaho">ID</option>
<option value="Illinois">IL</option>
<option value="Indiana">IN</option>
<option value="Iowa">IA</option>
<option value="Kansas">KS</option>
<option value="Louisana">LA</option>
<option value="Maine">ME</option>
<option value="Maryland">MD</option>
<option value="Massachusetts">MA</option>
<option value="Michigan">MI</option>
<option value="Minnesota">MN</option>
<option value="Mississippi">MS</option>
<option value="Missouir">MO</option>
<option value="Montana">MT</option>
<option value="Nebraska">NE</option>
<option value="Nevada">NV</option>
<option value="New Hampshire">NH</option>
<option value="New Jersey">NJ</option>
<option value="New Mexico">NM</option>
<option value="New York">NY</option>
<option value="North Carolina">NC</option>
<option value="North Dakota">ND</option>
<option value="Ohio">OH</option>
<option value="Oklahoma">OK</option>
<option value="Oregon">OR</option>
<option value="Pennsylvania">PA</option>
<option value="Rhode Island">RI</option>
<option value="South Carolina">SC</option>
<option value="South Dakota">SD</option>
<option value="Tennessee">TN</option>
<option value="Texas">TX</option>
<option value="Utah">UT</option>
<option value="Vermont">VT</option>
<option value="Virginia">VA</option>
<option value="Washington">WA</option>
<option value="West VIrginia">WV</option>
<option value="Wisconsin">WI</option>
<option value="Wyoming">WY</option>
Zip:<input type="text" name="zip"><br>
Phone:<input type="text" name="phone"><br>
Email: <input type="text" name="email"><br>
<input type="submit" value="Submit">
</form>

</body>
</html>
