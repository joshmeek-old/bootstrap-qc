<h1>Bootstrap QC</h1>

<h3>Quick Conversion forms for Twitter Bootstrap!</h3>

Download
<a href="http://twitter.github.io/bootstrap/">Bootstrap</a> 2.3.2

------
View the live <a href="http://josmek.github.io/bootstrap-qc/">demo</a> using Fahrenheit and Celsius
------

Script for Input / Calculations
```javascript
<script>
  function convert(degree){
		if (degree=="C"){
 			F=document.getElementById("ce").value * 9 / 5 + 32;
 			document.getElementById("fa").value=F;
 		}
		else{	
 			C=(document.getElementById("fa").value -32) * 5 / 9;
 			document.getElementById("ce").value=C;
 		}
	}
</script>
```

Code for design of form
```html
<div class="container">
    <form class="form-signin">
      <h2 class="form-signin-heading">Temperature</h2>
      <input type="text" class="input-block-level" placeholder="Celsius" id="ce" name="ce" onkeyup="convert('C')">
      <input type="text" class="input-block-level" placeholder="Fahrenheit" id="fa" name="fa" onkeyup="convert('F')">
    </form>
</div>
```

CSS to give the form the shape from the demo
```css
<style type="text/css">
      body {
        padding-top: 40px;
        padding-bottom: 40px;
        background-color: #f5f5f5;
      }

      .form-signin {
        max-width: 300px;
        padding: 19px 29px 29px;
        margin: 0 auto 20px;
        background-color: #fff;
        border: 1px solid #e5e5e5;
        -webkit-border-radius: 5px;
           -moz-border-radius: 5px;
                border-radius: 5px;
        -webkit-box-shadow: 0 1px 2px rgba(0,0,0,.05);
           -moz-box-shadow: 0 1px 2px rgba(0,0,0,.05);
                box-shadow: 0 1px 2px rgba(0,0,0,.05);
      }
      .form-signin .form-signin-heading,
      .form-signin .checkbox {
        margin-bottom: 10px;
      }
      .form-signin input[type="text"],
      .form-signin input[type="password"] {
        font-size: 16px;
        height: auto;
        margin-bottom: 15px;
        padding: 7px 9px;
      }
</style>
```
