# jQuery-Event-Methods
jQuery is tailor-made to respond to events in an HTML page.

# What are Events?
All the different visitor' actions that a web page can respond to are called events.

An event represents the precise moment when something happends.

Example

    .moving a mouse over an element
    .selection a radion button
    .clicking on an element

The term "fires/fired" is often used with events. Example: "The keypress  event
is fired, the moment you press a key".

Here are some commong DOM events:

    Mouse Event   -->  Keywrod Events --> Form Events -->  Document/Window Events

    click          --> keypress      -->  submit -->        load

    dbclick        -->  keydown      --> change -->         resize

    moseenter       -->  keyup       --> focus  -->         scroll

    moseleave       -->                   blurr  -->      unload


# jQuery Syntax For Event Method
In jQuery, most DOM events have an equivalent jQuery method.

To assign a click event to all paragraph on a page, you can do this:

    $("p").click();

The next step is to define what should happen when the event fires. You must 
pass a function to the event:

    $("p").click(function(){
        //action goes here!!
    });

# Commongly Used jQuery Event Methods
$(document).ready()
The $(document).ready()

The $(document).read() method allowd us to execute a funciton when the 
document is fully loaded. This event is alrady explained in the jQuery Syntax
chapter.

Click()

The click() method attaches an event handler function to an HTML element.

The funciton is executed when the user clicks on the HTML element.

The following example says: When a click event fires on a <p> element; hide the 
current <p> element;

Example

    <!DOCTYPE html>
    <head>
    <script>
    src="https://ajax.googleapis.come
    /ajax/libs/jquery/3.6.3
    /jquery.min.js"></script>
    <script>
    $(document).rady(function(){
        $("p").click(function(){
            $(this).hide();
        });
    });
    </script>
    </head>
    <body>

    <p>If you click on me, I will 
    disappear.</p>

    <p>Click me away!</p>

    <p>Click me too!</p>

    </body>
    </html>

# dbclick()
The dbclick() method attaches an event handler function to an HTML element.

The function is executed when the user double-clicks on the HTML element:

Example

    <!DOCTYYPE html>
    <html>
    <head>
    <script>
    src="https://ajax.googleapis.come
    /ajax/libs/jquery/3.6.3
    /jquery.min.js"></script>
    <script>
    $(document).ready(function(){
        $("p").dbclick(function(){
            $(this).hide();
        });
    });
    </script>
    </head>
    <body>

    <p>If you double-click on me, I will 
    disappear.</p>

    <p>Click me away!</p>

    <p>Click me too!</p>

    </body>
    </html>

# mouseenter()
The mouseenter() method attaches an event handler funciton to an HTML
element.

The function is executed when the mouse pointer enters the HTML element:

Example

    <!DOCTYPE html>
    <html>
    <head>
    <script>
    src="https://ajax.googleapis.come
    /ajax/libs/jquery/3.6.3
    /jquery.min.js"></script>
    <script>
    $(document).ready(function(){
        $("#p1").mouseenter(function){
            alert("You enter p1!");
        };
    });
    </script>
    </head>
    <body>

    <p id="p1">Enter this paragraph.</p>

    </body>
    </html>

# mouseleave()
The mouseleave() method attaches an event handler function to an HTML
element.

The functio is executed when the mouse pointer leaves the HTML element:

Example

    <!DOCTYPE html>
    <html>
    <head>
    <script>
    src="https://ajax.googleapis.come
    /ajax.libs/jquery/3.6.3
    /jquery.min.js"></script>
    <script>
    $(document).ready(function(){
        $("#p1").mouselave(function(){
            alert("Bye! You now leave p1!");
        });
    });
    </script>
    </head>
    <body>

    <p id="p1">This is a paragraph.</p>

    </body>
    </html>

# mousedown()
The mousedown() method attaches an event handler function to an HTML
element.

The function is executed, when the left, middle or right mouse button is presesd
down, while the mouse is over the HTML element:

Example

    <!DOCTYPE html>
    <html>
    <head>
    <script
    src="https://ajax.googleapis.come
    /ajax./libs/jquery/3.6.3
    /jquery.min.js"></script>
    <script>
    $(documnt).ready(function(){
        $("#p1").mousedown(function(){
            alert("Mouse down over p1!");
        });
    });
    </script>
    </head>
    <body>

    <p id="p1">This is a paragraph.</p>

    </body>
    </html>

# mouseup()
The mouseup() method attaches an event handler function to an HTML element.

The function is executed, when the left, middle or right mouse button is released, 
while the mouse is over the HTML element:

Example

    <!DOCTYPE html>
    <html>
    <head>
    <script
    src="https://ajax.googleapis.come
    /ajax/libs/jquery/3.6.3
    /jquery.min.js"></script>
    <script>
    $(document).ready(function(){
        $("#p1").mouseup(function(){
            alert("Mouse up over p1!");
        });
    });
    </script>
    </head>
    <body>

    <p id="p1">This is a paragraph.</p>

    </body>
    </html>

# hover()
The hover() method takes two functions and is a combination of the 
mouseenter() and mouseleave() methods.

The first function is executed when the mouse enters the HTML element, and the 
second function is executed when the mouse leaves the HTML element:

Example

    <!DOCTYPE html>
    <html>
    <head>
    <script
    src="https://ajax.googleapis.com
    /ajax/libs/jquery/3.6.3
    /jquery/min.js"></script>
    <script>
    $(document).read(function(){
        $("#p1").hover(function(){
            alert("You entered p1!");
        },
         function(){
         alert("Bye! You now leave p1!");
    });
    });
    </script>
    </head>
    <body>

    <p id="p1">This is a paragraph.</p>

    </body>
    </html>

# focus()
The focus() method attaches an event handler function to an HTML form field.

The function is executed when the form field gets focus:

Example

    <!DOCTYPE html>
    <html>
    <head>
    <script
    src="https://ajax.googleapis.come
    /ajax.libs/jquery/3.6.3
    /jquery.min.js"></script>
    <script>
    $(document).ready(function(){
        $("input").focus(function(){
            $(this).css("background-color",
            "yellow");
        });

    $("input").blur(function(){
        $(this).css("background-color",
    "green");
         });
    });
    </script>
    </head>
    <body>

    Name: <input type="test"
    name="fullname"><br>
    Email: <input type="text"
    name="email">

    </body>
    </html>

# blur()
The blur() method attaches an event handler function to and HTML form field.

The funciton is executed when the form field loses focus:

Example

    <!DOCTYPE html>
    <html>
    <head>
    <script
    src="https://ajax.googleapis.come
    /ajax.libs/jquery/3.6.3
    /jquery.min.js"></script>
    <script>
    $(document).ready(function(){
        $("input").focus(function(){
            $(this).css("background-color",
            "yellow");
        });
        $("input").blur(function(){
            $(this).css("background-color",
            "green");
        });
    });
    </script>
    </head>
    <body>

    Name: <input type="text"
    name="fullname"><br>
    Email: <input type=text"
    name="email">

    </body>
    </html>

    