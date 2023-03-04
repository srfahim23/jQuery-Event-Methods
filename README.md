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


