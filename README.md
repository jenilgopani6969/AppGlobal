# AppGlobal

![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)

Global code for any Android App.

Add it in your root build.gradle at the end of repositories:

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
Step 2. Add the dependency

	dependencies {
	        implementation 'com.github.jenilgopani6969:AppGlobal:1.1.2'
	}
	
### Check Email
	
```sh
AppGlobal.checkEmail("xyz@gmail.com");
```	

### Check Email by Pattern
	
```sh
Pattern EMAIL_ADDRESS_PATTERN = Pattern.compile("[a-zA-Z0-9\\+\\.\\_\\%\\-\\+]{1,256}" + "\\@"
                    + "[a-zA-Z0-9][a-zA-Z0-9\\-]{0,64}" + "(" + "\\."
                    + "[a-zA-Z0-9][a-zA-Z0-9\\-]{0,25}" + ")+");

AppGlobal.checkEmailbyPattern("xyz@gmail.com", EMAIL_ADDRESS_PATTERN);
```	

### Check PhoneNumber
	
```sh
AppGlobal.checkPhoneNumber("passPhoneNumber");
```	

### Check PhoneNumber by Pattern
	
```sh
Pattern PHONE_NUMBER_PATTERN = Pattern.compile("^[7-9][0-9]{9}$");

AppGlobal.checkPhoneNumberbyPattern("passPhoneNumber", PHONE_NUMBER_PATTERN);
```	

### Check Password
	
```sh
AppGlobal.checkPassword("passPassword");
```	

### Check Password by Pattern
	
```sh
Pattern PASSWORD_NUMBER_PATTERN = Pattern.compile("^(?=.*[0-9])(?=.*[a-z])(?=.*[A-Z])(?=\\S+$).{8,}$");

AppGlobal.checkPasswordbyPattern("passPassword", PASSWORD_NUMBER_PATTERN);
```	
 
### Toast Message

```sh
AppGlobal.showToast(context,"Message");
```

### Check Network 

```sh
AppGlobal.isNetwork(context);

return boolean 
```

