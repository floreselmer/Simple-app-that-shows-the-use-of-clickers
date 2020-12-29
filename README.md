# Simple-app-that-shows-the-use-of-clickers
In this codelab, you work with a starter app called DessertClicker. In this app, each time the user taps a dessert on the screen, the app "purchases" the dessert for the user. 
The app updates values in the layout for the number of desserts that were purchased, and for the total amount the user spent.
The activity lifecycle is a set of states through which an activity migrates. 
The activity lifecycle begins when the activity is first created and ends when the activity is destroyed.
As the user navigates between activities and inside and outside of your app, each activity moves between states in the activity lifecycle.
Each state in the activity lifecycle has a corresponding callback method you can override in your Activity class. 
There are seven lifecycle methods: onCreate()onStart()onPause()onRestart()onResume()onStop()onDestroy()
To add behavior that occurs when your activity transitions into a lifecycle state, override that state's callback method.
To add skeleton override methods to your classes in Android Studio, select Code > Override Methods or press Control+o.

Timber is a logging library with several advantages over the Android logging API. In particular, the Timber library:

Generates the log tag for you based on the class name.
Helps avoid showing logs in a release version of your Android app.
Allows for integration with crash reporting libraries.
To use Timber, add its dependency to your Gradle file and extend the Application class to initialize it:

Application is a base class that contains global application state for your entire app. There is a default Application class that is used by Android if you don't specify one. You can create your own Application subclass to initialize app-wide libraries such as Timber.
Add your custom Application class to your app by adding the android:name attribute to the <application> element in the Android manifest. Do not forget to do this!
Use Timber.i() to write log messages with Timber. This method only takes one argument: the message to write. The log tag (the name of the class) is added for you automatically.
