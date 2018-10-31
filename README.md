# BootstrpGridSystem
## Learning Objectives
* Using bootstrap grid system

## The Walkthrough

1. Create a Spring Boot Application
	* Name it BootsrapButtons
	* Add the dependencies for the web and for thymeleaf
	* Hit next until you finish the wizard, and then wait until it's done.

2. Create a Controller
	* Right click on com.example.demo and click New -> Class
	* Name it HomeController.java
	* Edit it to look like this:
```java
import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.RequestMapping;

@Controller
public class HomeController {

    @RequestMapping("/")
    public String index(){
        return "index";
    }
}
```

3. Create a Template
  * Right click on templates and click New -> Html
	* Name it index.html
	* Edit it to look like this:
```html
<!DOCTYPE html>
<html lang="en" xmlns:th="www.thymeleaf.org">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width,initial-scale=1">
    <title>Bootstrap 101 template</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
</head>
<body>
	<div class="container">
    <h1>Grid system</h1>
    <br>
    <div class="row">
        <div class="col">
            <h3>This is the first column - 1 of 2</h3>
            <p>
							Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
                Aenean commodo ligula eget dolor. Aenean massa. Cum sociis
                natoque penatibus et magnis dis parturient montes, nascetur
                ridiculus mus.
                Donec quam felis, ultricies nec, pellentesque eu, pretium quis,
                sem. Nulla consequat massa quis enim
							</p>
        </div>
        <div class="col">
            <h3>This is the second column - 2 of 2</h3>
            <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
                Aenean commodo ligula eget dolor. Aenean massa. Cum sociis
                natoque penatibus et magnis dis parturient montes, nascetur
                ridiculus mus.
                Donec quam felis, ultricies nec, pellentesque eu, pretium quis,
                sem. Nulla consequat massa quis enim
							</p>
        </div>
    </div>
    <br>
    <!--<h4>3 Columns</h4>-->
    <div class="row">
        <div class="col">
            <h3>First Column</h3>
            <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
                Aenean commodo ligula eget dolor. Aenean massa. Cum sociis
                natoque penatibus et magnis dis parturient montes, nascetur
                ridiculus mus.
                Donec quam felis, ultricies nec, pellentesque eu, pretium quis,
                sem. Nulla consequat massa quis enim
							</p>
        </div>
        <div class="col">
            <h3>Second Column</h3>
            <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
                Aenean commodo ligula eget dolor. Aenean massa. Cum sociis
                natoque penatibus et magnis dis parturient montes, nascetur
                ridiculus mus.
                Donec quam felis, ultricies nec, pellentesque eu, pretium quis,
                sem. Nulla consequat massa quis enim
							</p>
        </div>
        <div class="col">
            <h3>Third Column</h3>
            <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
                Aenean commodo ligula eget dolor. Aenean massa. Cum sociis
                natoque penatibus et magnis dis parturient montes, nascetur
                ridiculus mus.
                Donec quam felis, ultricies nec, pellentesque eu, pretium quis,
                sem. Nulla consequat massa quis enim
							</p>
        </div>
    </div>
</div>
</body>
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js" integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
</html>
```

4. Run your application and open a browser, if you type in the URL http://localhost:8080

## What is Going On

### The Controller
Here, the default route maps to index.html.

### The View
Bootstrap's grid system allows up to 12 columns to layout and align content.
When using grid system rows must be placed within a container or container-fluid class for proper alignment and padding.
With the grid system you can have one column takes up the entire width of the grid, or you can specify
a column takes up two, three, or 12 spaces on the grid if you want to.

