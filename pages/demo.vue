<template>
  <div class="remove-al-styles">
    <h3>Sign in</h3>
<form >
  <label for="uname">Username</label><br>
  <input type="text" id="uname" name="uname"><br>
  <label for="pwd">Password</label><br>
  <input type="password" id="pwd" name="pwd"><br><br>
  <p>Don't have a login? Click here.</p>
  <input type="submit" value="Sign in">
  
</form>

<h1 style="text-align:center;">TechieScribes Demo Site</h1>
<p>You have succeeded in logging in to the TechieScribes demo pages.</p>
<p>Here you can discover how the new inline tutorial will work. Below are a number of examples. Click the link to get to the respective pages and go through the tutorials.</p>
<p><b>For the examples in these pages, you do not have to enter your real data or valid information, the information entered just must conform to the format indicated for the respective field</b>.</p>
<p><b>Use case examples</b></p>
<ul>
<li>Create Account</li>
<li>Declare VAT</li>
</ul>


<h1 style="text-align:center;">Your Account</h1>
<p>Please fill in the fields below to create your account.<br>If you need help, click <b>Shift + F1</b>.</p>

<form>
  <label for="fname">First name</label><br>
  <input type="text" id="fname" name="fname" size="50"><br>
  <label for="lname">Last name</label><br>
  <input type="text" id="lname" name="lname" size="50"><br>
  <label for="uname">User name</label><br>
  <input type="text" id="uname" name="uname" size="50"><br>
  <label for="birthday">Birthday</label><br>
  <input type="date" id="birthday" name="birthday"><br>
  <label for="email">Email Address</label><br>
  <input type="email" id="email" name="email" size="50"><br>
  <label for="pwd">Password</label><br>
  <input type="password" id="pwd" name="pwd"><br>
  <label for="pwd">Confirm Password</label><br>
  <input type="password" id="pwd" name="pwd"><br><br>
  <input type="submit" value="Reset">   <input type="submit" value="Confirm">
  
</form>

<h1 style="text-align:center;">Company account</h1>
<p>Please fill in the form below.<br>If you need help, click <b>Shift + F1</b>.</p>





<h1 style="text-align:center;">VAT Declaration</h1>
<p>Please check the corresponding boxes for everyhting you need to declare.</p>



  </div>
</template>

<script>
// import Logo from '~/components/Logo.vue'
// import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    // Logo,
    // VuetifyLogo
  }
}
</script>
<style scoped>

 .remove-all-styles {
    all: revert;
  }

  p {
    margin: 35px;;
  }

  h3 {
    margin: 35px;;
  }

  ul {
    margin: 35px;;
  }

  form {
    margin: 35px;;
  }

  input[type=text] {
    border-style: solid;
    border-color: black;
  }

  input[type=password] {
    border-style: solid;
    border-color: black;
  }

  input[type=date] {
    border-style: solid;
    border-color: black;
  }
  
  input[type=email] {
    border-style: solid;
    border-color: black;
  }

  input[type=number] {
    border-style: solid;
    border-color: black;
  }

  input[type=month] {
    border-style: solid;
    border-color: black;
  }

   input[type=submit] {
    background-color: lightgray;
  }

  table th {
  background-color: #89A1FF;
}

</style>
