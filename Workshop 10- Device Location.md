# W5- Device Location 

Key Terms

.The info p.list= file contains some information about settings and other information about your app. 
.CoreLocation= A libray that enables classes to use location "stuff".

**What is requesting permission?**

Requesting that you have access to that information.

**How do you request permision?**

There are two ways you can do it in which the user can accept or deny. 

1) Go to info.plist 
2) right click 
3) Click on add row tab 
4) one of the tabs to click on are: Privacy- Location Always and when in usage.
5) The other tab: Location always and when in usage

**What is the role of the location manager?**

Is the entry point to the location services.

**How do you create the location manager?

This must be created as a property of a class.

```swift 

let locationmanager = CLLocationManager()

```

What is the code for the extension and why is it important?

```swift 

extenstion ViewController: CLLocationManager Delegate{
}

```
This is done outside the curly bracket and it is important because it is saying that the viewcontroller can act on behalf (delegate) on the CLLlocation Manger. Therefore explaiing it can do the same role whilst executing that this role is optional






