# Ex.05 Design a Website for Server Side Processing
## Date:17.12.24

## AIM:
 To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side. 


## FORMULA:
P = I<sup>2</sup>R
<br> P --> Power (in watts)
<br> I --> Intensity
<br> R --> Resistance

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
math.html

<!DOCTYPE html>
<html>
<head>
<meta charset='utf-8'>
<meta http-equiv='X-UA-Compatible' content='IE=edge'>
<title>Power Calculation (P = I²R)</title>
<meta name='viewport' content='width=device-width, initial-scale=1'>
<style type="text/css">
body {
    background-color:  #caf75b;
}
.edge {
    width: 100%;
    padding-top: 250px;
    text-align: center;
}
.box {
    display: inline-block;
    border: thick double rgb(59, 8, 116);
    width: 500px;
    min-height: 300px;
    font-size: 20px;
    background-color: #fefbd8;
}
.formelt {
    color: black;
    text-align: center;
    margin-top: 7px;
    margin-bottom: 6px;
}
h1 {
    color: black;
    padding-top: 20px;
}
</style>
</head>
<body>
<div class="edge">
    <div class="box">
        <h1>Power Calculation</h1>
        <h3>Vishnurathan</h3>
        <form method="POST">
            {% csrf_token %}
            <div class="formelt">
                Current (I): <input type="text" name="current" value="{{current}}"> A<br/>
            </div>
            <div class="formelt">
                Resistance (R): <input type="text" name="resistance" value="{{resistance}}"> Ω<br/>
            </div>
            <div class="formelt">
                <input type="submit" value="Calculate"><br/>
            </div>
            <div class="formelt">
                Power (P): <input type="text" name="power" value="{{power}}"> W<br/>
            </div>
        </form>
    </div>
</div>
</body>
</html>
```

## SERVER SIDE PROCESSING:
![Screenshot 2024-12-16 104144](https://github.com/user-attachments/assets/9d39e64f-fd0e-4965-956f-12d2b65711f3)


## HOMEPAGE:
![Screenshot 2024-12-17 154327](https://github.com/user-attachments/assets/644088d0-b798-4a9c-a70f-3c167939834c)


## RESULT:
The program for performing server side processing is completed successfully.
