### :camel: HTML examples
---

#### Task1: Create the below form using HTML

![Screenshot](html1-form2.png)

```
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>
<h2>Welcome To GFG</h2>
<form>
	

<p>
	<label>Username : <input type="text" /></label>
	</p>


	

<p>
	<label>Password : <input type="password" /></label>
	</p>


	

<p>
	<button type="submit">Submit</button>
	</p>


</form>
</body>

```

#### Task2: Create the below form using HTML

![Screenshot](html1-form2.png)

```
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>
<h2>Select your gender</h2>
<form>
	<label>Male<input type="radio" name="gender" value="male" /></label>
	<label>Female<input type="radio" name="gender" value="female" /></label>
</form>
</body>
</html>

```

#### Task3: Create the below form using HTML

![Screenshot](html1-form3.png)

```
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>
<h2>Choose Language</h2>
<form>
	<ul style="list-style-type:none;">
	<li><input type="checkbox" name="language" value="hindi" />Hindi</li>
	<li><input type="checkbox" name="language" value="english" />English</li>
	<li><input type="checkbox" name="language" value="sanskrite" />Sanskrit</li>
	</ul>
</form>
</body>
</html>

```

#### Task4: Create the below form using HTML

![Screenshot](html1-form4.png)
```
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>
<h2>Select Your Nationality</h2>
<form>
<select name="language">
	<option value="indian">Indian</option>
	<option value="nepali">Nepali</option>
	<option value="others">Others</option>
</select>
</form>
</body>
</html>
```

#### Task5: Create the below form using HTML

![Screenshot](html1-form5.png)

```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GfG</title>
</head>
<body>
<form>
	<fieldset>
	<legend>Personal Details</legend>
	

<p>
		<label>
		Salutation
		<br />
		<select name="salutation">
			<option>--None--</option>
			<option>Mr.</option>
			<option>Ms.</option>
			<option>Mrs.</option>
			<option>Dr.</option>
			<option>Prof.</option>
		</select>
		</label>
	</p>


	

<p>
		<label>First name: <input name="firstName" /></label>
	</p>


	

<p>
		<label>Last name: <input name="lastName" /></label>
	</p>


	

<p>
		Gender :
		<label><input type="radio" name="gender" value="male" /> Male</label>
		<label><input type="radio" name="gender" value="female" /> Female</label>
	</p>


	

<p>
		<label>Email:<input type="email" name="email" /></label>
	</p>


	

<p>
		<label>Date of Birth:<input type="date" name="birthDate"></label>
	</p>


	

<p>
		<label>
		Address :
		<br />
		<textarea name="address" cols="30" rows="3"></textarea>
		</label>
	</p>


	

<p>
		<button type="submit">Submit</button>
	</p>


	</fieldset>
</form>
</body>
</html>


```

#### Task6: Create the below form using HTML

![Screenshot](html1-form6.png)

```
<html>
    <head>
        <script>
            function GEEKFORGEEKS() {
                var name =
                    document.forms.RegForm.Name.value;
                var email =
                    document.forms.RegForm.EMail.value;
                var phone =
                    document.forms.RegForm.Telephone.value;
                var what =
                    document.forms.RegForm.Subject.value;
                var password =
                    document.forms.RegForm.Password.value;
                var address =
                    document.forms.RegForm.Address.value;
                var regEmail=/^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$/g;  //Javascript reGex for Email Validation.
                var regPhone=/^\d{10}$/;                                        // Javascript reGex for Phone Number validation.
                var regName = /\d+$/g;                                    // Javascript reGex for Name validation
 
                if (name == "" || regName.test(name)) {
                    window.alert("Please enter your name properly.");
                    name.focus();
                    return false;
                }
 
                if (address == "") {
                    window.alert("Please enter your address.");
                    address.focus();
                    return false;
                }
                 
                if (email == "" || !regEmail.test(email)) {
                    window.alert("Please enter a valid e-mail address.");
                    email.focus();
                    return false;
                }
                  
                if (password == "") {
                    alert("Please enter your password");
                    password.focus();
                    return false;
                }
 
                if(password.length <6){
                    alert("Password should be atleast 6 character long");
                    password.focus();
                    return false;
 
                }
                if (phone == "" || !regPhone.test(phone)) {
                    alert("Please enter valid phone number.");
                    phone.focus();
                    return false;
                }
 
                if (what.selectedIndex == -1) {
                    alert("Please enter your course.");
                    what.focus();
                    return false;
                }
 
                return true;
            }
        </script>
 
        <style>
            div {
                box-sizing: border-box;
                width: 100%;
                border: 100px solid black;
                float: left;
                align-content: center;
                align-items: center;
            }
 
            form {
                margin: 0 auto;
                width: 600px;
            }
        </style>
    </head>
 
    <body>
        <h1 style="text-align: center;">REGISTRATION FORM</h1>
        <form name="RegForm" onsubmit="return GEEKFORGEEKS()" method="post">
             
<p>Name: <input type="text"
                            size="65" name="Name" /></p>
 
            <br />
             
<p>Address: <input type="text"
                            size="65" name="Address" />
        </p>
 
            <br />
             
<p>E-mail Address: <input type="text"
                            size="65" name="EMail" /></p>
 
            <br />
             
<p>Password: <input type="text"
                        size="65" name="Password" /></p>
 
            <br />
             
<p>Telephone: <input type="text"
                        size="65" name="Telephone" /></p>
 
            <br />
 
             
<p>
                SELECT YOUR COURSE
                <select type="text" value="" name="Subject">
                    <option>BTECH</option>
                    <option>BBA</option>
                    <option>BCA</option>
                    <option>B.COM</option>
                    <option>GEEKFORGEEKS</option>
                </select>
            </p>
 
            <br />
            <br />
             
<p>Comments: <textarea cols="55"
                            name="Comment"> </textarea></p>
 
             
<p>
                <input type="submit"
                    value="send" name="Submit" />
                <input type="reset"
                    value="Reset" name="Reset" />
            </p>
 
        </form>
    </body>
</html>

```