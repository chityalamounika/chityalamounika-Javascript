# chityalamounika-Javascript
Registration Form


<html>
<head>
<title>Registrationform
</title>
<script language="javascript">
function validate()
{
var msg="";
var Uname=document.register.txtUN.value;
var rUN=new RegExp("[A-Za-z]{6,}$");

var pwd=document.register.txtPWD.value;
var rPWD=new RegExp("[\\w]{6,}$");

var email=document.register.txtEmail.value;
var rEmail=new RegExp("[\\w]+.com");

var phone=document.register.txtPhone.value;
var rPhone=new RegExp("^[0-9]{10}$");

if(!Uname.match(rUN))
msg+="\nUsername should contain only alphabets of length atleast 6 character";

if(!pwd.match(rPWD))
msg+="\npaassword should contain atleast 6 character";

if(!email.match(rEmail))
msg+="\nemail should be of abc@xyz.com pattern";

if(!phone.match(rPhone))
msg+="\n enter a 10 digit number";
if(msg!="")
{
alert(msg);
return false;
}
else
{
alert('Registered');
return true;
}
}
</script>
</head>
<body>
<form  name="register" onSubmit="return validate()">
<table align="center">
<caption>Registration form</caption>
<tr><td>Username</td>
<td><input type="text" name="txtUN"></td>
</tr>
<tr><td>password</td>
<td><input type="password" name="txtPWD"></td>
<tr>			
<td>Email Address:</td>			
<td><input type="text" name="txtEmail"></td>		
</tr>
<tr>
<td>Gender</td>
<td><input type="radio" name="male">male</td>
<td><input type="radio" name="female">female</td>
</tr>
<tr>
<td>Mobile Number</td>
<td><input type="text" name="txtPhone"</td>
</tr> 
<tr>
<td>DateofBirth</td>
<td><input type="date" name="Dateofbirth"></td>
</tr>
<tr><td>knownlanguages</td>
<td><input type="checkbox" name="language" value="Telugu">Telugu</td>
<td><input type="checkbox" name="language" value="Hindi">Hindi</td>
<td><input type="checkbox" name="language" value="English">English</td>
<td><input type="checkbox" name="language" value="Other">Other</td>
</tr>
<tr><td>Technical Skills</td>
<td><input type="checkbox" name="language" value="c">c</td>
<td><input type="checkbox" name="language" value="c++">c++</td>
<td><input type="checkbox" name="language" value="Java">Java</td>
<td><input type="checkbox" name="language" value="Other">Other</td>
</tr>
<tr><td>Address:</td>
<td><textarea="Address" rows="5" cols="15" maxlength="20">
</textarea></td>
</tr>
<tr><td>state</td>
<td><select name="state" size=2>
<option value="Telangana" selected>Telangana</option>
<option value="Andhrapradesh" selected>Andhrapradesh</option>
<option value="TamilNadu" selected>TamilNadu</option>
</select></td>
</tr>
<tr><td>district</td>
<td><select name="district" size=2>
<option value="rangareddy" selected>rangareddy</option>
<option value="warangal" selected>warangal</option>
</select></td>
</tr>
<tr><td align=center><input type="Submit" value="Register"></td>
</tr>
</table>
</form>
</body>
</html>
















#LoginForm

<html>
<head>
<title>Loginform
</title>
<script language="javascript">
function validate()
{
var msg="";
var Uname=document.register.txtUN.value;
var rUN=new RegExp("[A-Za-z]{6,}$");
var pwd=document.register.txtPWD.value;
var rPWD=new RegExp("[\\w]{6,}$");
if(!Uname.match(rUN))
msg+="\nUsername should contain only alphabets of length atleast 6 character";
if(!pwd.match(rPWD))
msg+="\npaassword should contain atleast 6 character";

if(msg!="")
{
alert(msg);
return false;
}
else
{
alert('Logined Sucessfully');
return true;
}
}
</script>
</head>
<body>
<form  name="register" onSubmit="return validate()">
<table align="center">
<caption>Login form</caption>
<tr><td>Username</td>
<td><input type="text" name="txtUN"></td>
</tr>
<tr><td>password</td>
<td><input type="password" name="txtPWD"></td>
</tr>	
<tr><td align=center><input type="Submit" value="LOGIN"></td>
</tr>
</table>
</form>
</body>
</html>		










