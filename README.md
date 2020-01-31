# android-orientation
android layout orientation for beginners

##### Step 1: Create a new project in Android Studio.
              Go to File ⇒ New Project and fill all required details to create a new project.
              
              
##### Step 2: Add the following code to res/layout/activity_main.xml.

<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:orientation="vertical"
    android:layout_width="match_parent"
    android:gravity="center"
    android:background="@drawable/background"
    android:layout_height="match_parent">


    <EditText
        android:id="@+id/et_user_name"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginLeft="15dp"
        android:layout_marginRight="15dp"
        android:layout_marginBottom="10dp"
        android:background="@drawable/shape_corner"
        android:defaultFocusHighlightEnabled="false"
        android:hint="Username"
        android:inputType="textPersonName"
        android:padding="15dp"
        android:textAllCaps="false"
        android:textColor="@color/colorPrimary"
        android:textColorHint="@android:color/white"
        android:textSize="18sp"
        android:textStyle="italic" />

    <EditText
        android:id="@+id/et_password"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:inputType="numberPassword"
        android:defaultFocusHighlightEnabled="false"
        android:textColor="@color/colorPrimary"
        android:layout_marginLeft="15dp"
        android:layout_marginRight="15dp"
        android:background="@drawable/shape_corner"
        android:padding="15dp"
        android:textAllCaps="false"
        android:textSize="18sp"
        android:hint="Password"
        android:textStyle="italic"
        android:textColorHint="@android:color/white" />


    <LinearLayout
        android:layout_width="match_parent"
        android:orientation="horizontal"
        android:gravity="center"
        android:layout_marginTop="10dp"
        android:layout_height="wrap_content">

        <Button
            android:id="@+id/signUp_btn"
            android:layout_width="0dp"
            android:layout_weight="1"
            android:layout_height="wrap_content"
            android:defaultFocusHighlightEnabled="false"
            android:textColor="@android:color/white"
            android:layout_marginLeft="15dp"
            android:layout_marginRight="15dp"
            android:background="@drawable/buttons"
            android:padding="15dp"
            android:textAllCaps="false"
            android:textSize="15sp"
            android:hint="Sign Up"
            android:textStyle="italic"
            android:textColorHint="@android:color/white"/>

        <Button
            android:id="@+id/signIn_btn"
            android:layout_width="0dp"
            android:layout_weight="1"
            android:inputType="textPersonName"
            android:defaultFocusHighlightEnabled="false"
            android:textColor="@android:color/white"
            android:layout_height="wrap_content"
            android:layout_marginLeft="15dp"
            android:layout_marginRight="15dp"
            android:background="@drawable/buttons"
            android:padding="15dp"
            android:textAllCaps="false"
            android:textSize="15sp"
            android:hint="Sign In"
            android:textStyle="italic"
            android:textColorHint="@android:color/white"/>

    </LinearLayout>

</LinearLayout>


##### Step 3: Create *layout-land* directory under *res* directory
              Right click on *res* directory ⇒ New ⇒ Android Resource Directory
              Resource type ⇒ layout
              Available qualifiers ⇒ Orientation ⇒⇒ Landscape ⇒ Ok
              
              
##### Step 4: Copy *activity_main.xml* from *res* directory to *layout-land* directory
              
              
##### Step 5: Replace the following code to res/layout-land/activity_main.xml.

<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:orientation="vertical"
    android:layout_width="match_parent"
    android:gravity="center"
    android:background="@drawable/background"
    android:layout_height="match_parent">

    <LinearLayout
        android:layout_width="match_parent"
        android:orientation="horizontal"
        android:layout_height="wrap_content">

        <EditText
            android:id="@+id/et_user_name"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:layout_marginLeft="15dp"
            android:layout_marginRight="15dp"
            android:layout_marginBottom="10dp"
            android:background="@drawable/shape_corner"
            android:defaultFocusHighlightEnabled="false"
            android:hint="Username"
            android:inputType="textPersonName"
            android:padding="15dp"
            android:textAllCaps="false"
            android:textColor="@color/colorPrimary"
            android:textColorHint="@android:color/white"
            android:textSize="18sp"
            android:textStyle="italic" />

        <EditText
            android:id="@+id/et_password"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:inputType="numberPassword"
            android:layout_weight="1"
            android:defaultFocusHighlightEnabled="false"
            android:textColor="@color/colorPrimary"
            android:layout_marginLeft="15dp"
            android:layout_marginRight="15dp"
            android:background="@drawable/shape_corner"
            android:padding="15dp"
            android:textAllCaps="false"
            android:textSize="18sp"
            android:hint="Password"
            android:textStyle="italic"
            android:textColorHint="@android:color/white" />



    </LinearLayout>


    <LinearLayout
        android:layout_width="match_parent"
        android:orientation="horizontal"
        android:gravity="center"
        android:layout_marginTop="10dp"
        android:layout_height="wrap_content">

        <Button
            android:id="@+id/signUp_btn"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:defaultFocusHighlightEnabled="false"
            android:textColor="@android:color/white"
            android:layout_marginLeft="15dp"
            android:layout_marginRight="15dp"
            android:background="@drawable/buttons"
            android:padding="15dp"
            android:textAllCaps="false"
            android:textSize="15sp"
            android:hint="Sign Up"
            android:textStyle="italic"
            android:textColorHint="@android:color/white"/>

        <Button
            android:id="@+id/signIn_btn"
            android:layout_width="wrap_content"
            android:inputType="textPersonName"
            android:defaultFocusHighlightEnabled="false"
            android:textColor="@android:color/white"
            android:layout_height="wrap_content"
            android:layout_marginLeft="15dp"
            android:layout_marginRight="15dp"
            android:background="@drawable/buttons"
            android:padding="15dp"
            android:textAllCaps="false"
            android:textSize="15sp"
            android:hint="Sign In"
            android:textStyle="italic"
            android:textColorHint="@android:color/white"/>

    </LinearLayout>

</LinearLayout>




##### Step 6: Run app on your device. Voila! It's working!

### NB: Make sure your device orientation is set to auto.

