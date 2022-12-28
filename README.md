# FloatingTextField
Use UITextfield as Floating Text Field using Material Components

#Podfile:

#Material Design for UIComponents.

pod 'MaterialComponents'  (This will install updated version of library)

or

pod 'MaterialComponents', '~> 94.2' (I used this)

#ViewController.swift

import UIKit
import MaterialComponents

class ViewController: UIViewController, UITextFieldDelegate {


     @IBOutlet weak var textFld_EmailId: MDCTextField!

     @IBOutlet weak var textFld_Password: MDCTextField!

     @IBOutlet weak var textFld_MobileNo: MDCTextField!


     // MARK: Properties
     var emailIdController: MDCTextInputControllerOutlined?

     var passwordController: MDCTextInputControllerOutlined?

     var mobileNoController: MDCTextInputControllerOutlined?

override func viewDidLoad() {
     super.viewDidLoad()
        // Do any additional setup after loading the view, typically from a nib.
        emailIdController = MDCTextInputControllerOutlined(textInput: textFld_EmailId)
        passwordController = MDCTextInputControllerOutlined(textInput: textFld_Password)
        mobileNoController = MDCTextInputControllerOutlined(textInput: textFld_MobileNo)

  }
}
