# W5- View Controllers

**Generally describe what a View Controller is.**

A function that controls what display screen you use. 

**All your view controllers are "sub classes" of what?**

They are subclasses of content (called "UIViewController".UIViewControllers are snippets of code which includes data for one "view " to allow you to  customise the method of the way the views flow between eachhother. I.E press yes and to the home page (sub class) or pick yes and remian on same page. 

**What is the life cycle of the view controller?**

It is how content is portrayed through a sub hierarchy of views.

**Name at least two (other than the one given) of the functions we can use in this life cycle.**

```swift 

  viewDidLoad()
  
  
``` 
  
**What is a segue?**

A operation that controls transition of pages.

**What is the segue "Identifier"**

The name for the the page.

**How do you setup a segue from a button in your storyboard?**

you click the "+" bar and go down to view conrtoller. Another screen should appear on the page. then you click the button on one of the screem and drag it to connect te two screen displays then right click and click show to connect them.

**How do you setup a segue between view controllers (ie without using a button)?**

Click ctrl and drag the top bar to the other display screen to connect them. 

**How do you call a segue programatically?**

Select segue from story 
Atrributes tab then click inspect
Give it a name '

To trigger the segue type in code...

```swift 

PerformSegue(with identifier:home", sender: nil)

```

**Briefly describe how you pass data between two view controllers (you may want to save some snippets of code here)?**

Set up sege in soryboard
Give it a name
PerformSegue 
Set property i.e score 
