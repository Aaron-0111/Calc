# Ex.08 Design of a Standard Calculator
## Date:13.05.2024

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>Calculator</title>

        <script>
        function calculate(args)
        {
            res = document.getElementById("result");
            expression = res.innerText;
            cmd = args.srcElement.innerText;
            if(cmd == "=")
            {
                expression = "" + eval(expression)
            }
            else if(cmd == "C")
            {
                expression=""
            }
            else if(cmd == "DEL")
            {
                expression = expression.slice(0, -1);

            }
            else if(cmd == "√")
            {
                expression = "" + Math.sqrt(eval(expression));
            }
            else if(cmd == "%")
            {
                expression = expression % 1;
            }
            else if(cmd == "log")
             {
        expression = Math.log10(expression);
           }
       
            else{
                expression = expression + cmd;
            }
            res.innerText = expression;
            

        }
         
        </script>

        <style>
          
            .calculator-container {
                width: 400px;
                background-color:rgb(15, 150, 222);
                margin: 0 auto; 
                margin-top: 160px;
                text-align: center;
                
            }

           
            button {
                width: 50px;
                height: 50px;
                margin: 10px; 
                font-size: 20px; 
                
                background-color:rgb(201, 237, 22); 
                color: black; 
                border: none;
            }

          
            #result {
                
       background-color:rgb(197, 239, 9);
    text-align: right;
    padding-right: 50px;
    font-size: 20px;
    margin-bottom: 20px; 
    border: solid black 0.5px;
    color: black;
    width: 348px;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: flex-end;

            }
            h1 {
                padding-top: 10px;
                color:black;
                font-size: 50px;
            }
            .redd {
                background-color: rgb(190, 15, 15);
            }
            .bluee {
                
                background-color: lavender;
            }
            body {
                background-color: lavender;
            }
           .bottomdiv{
            	    color:rgb(18, 220, 153);
            	    text-align: center;
                    position:relative;
           }

        </style>

    </head>
<body>
    <div class="bottomdiv">
    <h1> AARON RAJESH R CALCULATOR</h1>
<h1>Register no : 212223100001</h1>
	 
    <div class="calculator-container">
        
        <div id="result">0</div>
        <button onclick="calculate(event);">7</button>
        <button onclick="calculate(event);">8</button>
        <button onclick="calculate(event);">9</button>
        <button class="bluee"  onclick="calculate(event);">/</button>
        <button class="bluee"  onclick="calculate(event);"> DEL </button><br>
        <button onclick="calculate(event);">4</button>
        <button onclick="calculate(event);">5</button>
        <button onclick="calculate(event);">6</button>
        <button class="bluee"  onclick="calculate(event);">*</button>
        <button class="bluee"  onclick="calculate(event);">√ </button><br>
        <button onclick="calculate(event);">1</button>
        <button onclick="calculate(event);">2</button>
        <button onclick="calculate(event);">3</button>
        <button class="bluee"  onclick="calculate(event);">-</button>
        <button class="bluee"  onclick="calculate(event);">log</button><br>
        <button onclick="calculate(event);">0</button>
        <button onclick="calculate(event);">.</button>
        <button class="redd" onclick="calculate(event);">C</button>
        <button class="bluee"  onclick="calculate(event);">+</button>
        <button class="bluee" onclick="calculate(event);">=</button><br>
    </div>
    </body>
</html>
```
## OUTPUT:
![Screenshot 2024-05-13 134503](https://github.com/Aaron-0111/Calc/assets/149347631/a45c3f47-1a84-4d8c-9c9a-b02283b2982e)
![Screenshot 2024-05-13 134524](https://github.com/Aaron-0111/Calc/assets/149347631/b5b7979b-2d7e-4927-ace7-9f28f7a6ee55)

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
