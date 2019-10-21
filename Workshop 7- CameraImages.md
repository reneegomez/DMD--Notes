**What type of View controller allows us to select images from the photo library?**

```swift

let imagePicker = UIImagePickerController()
 imagePicker.sourceType = .photoLibrary
 
 ```
 
 **Try and explain what happens when we write an extension.**
 
 Without the extension the class can not be delegated as it has nothing to do on behalf of something. Therefore the extenstion adss to the stuff if it can do so when you do delgated it has somehting to be assigned to. It also organises your code so everything is together. 
 
 Example:
 
 ```swift
 
extension ViewController: UIImagePickerControllerDelegate, UINavigationControllerDelegate {
    
    func imagePickerController(_ picker: UIImagePickerController, didFinishPickingMediaWithInfo info: [UIImagePickerController.InfoKey : Any]) {
        print("Finished picking Image")
        
        let selectedImage = info[.originalImage] as? UIImage
        Imageview.image = selectedImage
        picker.dismiss(animated: true, completion: nil)
   
  ```

**What are the different sourceTypes?**

photolibrary and camera roll 

**What is a delegate?**

a form of code that assigns the class (in this case the view controller) to do something.
