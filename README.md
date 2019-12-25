# android-orientation
android layout orientation for beginners

##### Step 1: Create a new project in Android Studio.
              Go to File ⇒ New Project and fill all required details to create a new project.
              
              
##### Step 2: Add the following code to res/layout/activity_main.xml.

<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:gravity="center"
    android:orientation="vertical"
    android:padding="42dp"
    tools:context=".MainActivity">

    <androidx.appcompat.widget.AppCompatButton
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="Login" />

    <View
        android:layout_width="match_parent"
        android:layout_height="16dp" />

    <androidx.appcompat.widget.AppCompatButton
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="Register" />
</LinearLayout>



##### Step 3: Create *layout-land* directory under *res* directory
              Right click on *res* directory ⇒ New ⇒ Android Resource Directory
              Resource type ⇒ layout
              Available qualifiers ⇒ Orientation ⇒⇒ Landscape ⇒ Ok
              
              
##### Step 4: Copy *activity_main.xml* from *res* directory to *layout-land* directory
              
              
##### Step 5: Replace the following code to res/layout-land/activity_main.xml.

<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:gravity="center"
    android:orientation="horizontal"
    android:padding="42dp"
    tools:context=".MainActivity">

    <androidx.appcompat.widget.AppCompatButton
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_weight="1"
        android:text="Login" />

    <View
        android:layout_width="16dp"
        android:layout_height="match_parent" />

    <androidx.appcompat.widget.AppCompatButton
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_weight="1"
        android:text="Register" />
</LinearLayout>


##### Step 6: Run app on your device. Voila! It's working!

### NB: Make sure your device orientation is set to auto.
