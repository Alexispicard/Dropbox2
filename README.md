# Dropbox2
I built a new file from scratch for the assignment after the first one bugged down completely
Unfortuntately I have a few questions left:
1)
How do I copy a complete file to have a second copy of my work (if I want to make changes but I am afraid it will crash everything)? Basically I completely re-created my dropbox file, now it’s a “dropbox2” version

2) I get the same bug that I get with my first “dropbox” File, when I built the scroll in settings view

The code of my settingsViewController.swift file is: 

class settingsViewController: UIViewController {

    @IBOutlet weak var settingsScrollView: UIScrollView!
    @IBOutlet weak var settingsImage: UIImageView!
    
    override func viewDidLoad() {
        super.viewDidLoad()
        
        settingsScrollView.contentSize = CGSize(width: 320, height: 1200)
        settingsScrollView.contentSize = settingsImage.image!.size
        
        // Do any additional setup after loading the view.
    }

    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.

But then I run the simulator, successfully until I get to the actual view controller with the scroll and there it bugs down. I get two error messages.
First one is on this line of code below in the AppDelegate.swift file.  I get a “ Thread 1:signal SIGABRT” error message

 class AppDelegate: UIResponder, UIApplicationDelegate {



And in the bottom right corner I get the following error message:

libc++abi.dylib: terminating with uncaught exception of type NSException
(lldb) 

Any idea??

Note: I still have to work on:

back button in code
gesture recognizer
scroll view that don’t bug
log out button at the end
