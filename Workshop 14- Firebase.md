Static content is where things are set in stone by things you have coded.

Dynamic is where you have built code which allpws you to update the app. 

Firebase is an external storage to store data to update your app. 

when you write ref you are telling xcode where you want the data to be stored in this case firbase. 

```swift

 let ref = Firestore.firestore().collection("locations").document("rgomez")
 
 ```
Gepoint is firebase represenataion of a coordinate. 

