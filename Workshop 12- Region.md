#W12- Regions

**What object is responsible for monitoring regions?**

```swft 

CLRegion() 

```

**What are the maximum number of regions you can monitor for in a single app?**

20 per app. 

**...What would be one way around this limit?**

Get users location and work out the coordinates to test how far the user is from each point. 

```swift

open func distance(from location: CLocation) -> CLLocationDistance

```
        
**What are the two functions that notify you about a user entering/exiting a region?**

```swift

  func locationManager(_ manager: CLLocationManager, didEnterRegion region: CLRegion) {
        Image.image = UIImage(named: region.identifier)
        Label.text = region.identifier

       func locationManager(_manager: CLLocationManager, didExitRegion: CLRegion)
        Image.image = nil
        Label.text = nil
        
        ```
