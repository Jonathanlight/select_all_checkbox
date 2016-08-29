# select_all_checkbox
Select All checkbox input


<html>
  <head>
    <title>select all checkbox </title>
    <script src="https://code.jquery.com/jquery-3.1.0.min.js"></script>
  </head>
  
  <body>
<h1>Select All checkbox input</h1>
    
    <input type='checkbox' id="all"/> Select All<br> <hr>
    <input type='checkbox' name="day" />lundi <br>   
    <input type='checkbox' name="day" />mardi <br> 
    <input type='checkbox' name="day" />mercredi <br> 
    <input type='checkbox' name="day" />jeudi <br> 
    <input type='checkbox' name="day" />vendredi <br> 
    <input type='checkbox' name="day" />samedi <br> 
    <input type='checkbox' name="day" />dimanche <br> 
      
      
      <script>
        $('#all').click(function(event) {
      		if(this.checked) {
      			// Iterate each checkbox
      			$(':checkbox').each(function() {
      				this.checked = true;
      			});
      		}else{
      			$(':checkbox').each(function() {
      				this.checked = false;
      			});
      		}
      	});
      
      </script>
    
  </body>
</html>
