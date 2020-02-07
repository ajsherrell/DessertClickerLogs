# Dessert Clicker Logs
- An app to demonstrate use of logs.
- Made with Google Code Labs!
- Uses Timber library for logging.
- Implements LifecycleObserver.
- Implements onSaveInstanceState.

## Logging with Timber.
Timber is a logging library with several advantages over the Android logging API. In particular, the Timber library:

- Generates the log tag for you based on the class name.
- Helps avoid showing logs in a release version of your Android app.
- Allows for integration with crash reporting libraries.
- To use Timber, add its dependency to your Gradle file and extend the Application class to initialize it:

Application is a base class that contains global application state for your entire app. There is a default Application class that is used by Android if you don't specify one. You can create your own Application subclass to initialize app-wide libraries such as Timber.
Add your custom Application class to your app by adding the android:name attribute to the <application> element in the Android manifest. Do not forget to do this!
Use Timber.i() to write log messages with Timber. This method only takes one argument: the message to write. The log tag (the name of the class) is added for you automatically.
