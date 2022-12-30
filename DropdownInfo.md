to use the dropdowns and nav bar, use this code:
```html
<!DOCTYPE html>
<html>
<head>
    <title>DropDown Skeleton</title>
    <link rel="stylesheet" href="https://csslib.altiesgamingstudios.com/Dropdown.css">
</head>
<body>
        <div class="navbar">
            <a href="{site location/url}>Always viewable link</a>
            <div class="dropdown">
                <button class="dropbtn" onclick="myFunction()">More Options
                    <i class="fa fa-caret-down"></i>
                </button>
                <div class="dropdown-content" id="myDropdown">
                    <a href="{site location/url}">name</a>
                </div>
            </div> 
        </div>
    <script>
        /* When the user clicks on the button, 
        toggle between hiding and showing the dropdown content */
        function myFunction() {
          document.getElementById("myDropdown").classList.toggle("show");
        }
        
        // Close the dropdown if the user clicks outside of it
        window.onclick = function(e) {
          if (!e.target.matches('.dropbtn')) {
          var myDropdown = document.getElementById("myDropdown");
            if (myDropdown.classList.contains('show')) {
              myDropdown.classList.remove('show');
            }
          }
        }
    </script>
</body>
</html>
```
