# tugas

<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.example.mytask">

    <application
        android:allowBackup="true"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/AppTheme">
        <activity android:name=".MainActivity">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>

</manifest>


<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_height="match_parent"
    android:layout_width="match_parent"
    xmlns:app="http://schemas.android.com/apk/res-auto">

    <TextView
        android:id="@+id/taskText"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textStyle="bold"
        android:text="@string/todo_list"
        android:textColor="@android:color/black"
        android:layout_marginStart="16dp"
        android:layout_marginBottom="16dp"
        android:layout_marginTop="16dp"
        android:textSize="36sp"/>
    <androidx.recyclerview.widget.RecyclerView
        android:id="@+id/taskTextRecylerView"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/taskText"
        app:layoutManager="androidx.recyclerview.widget.LinearLayoutManager"
        android:nestedScrollingEnabled="true"/>
    <com.google.android.material.floatingactionbutton.FloatingActionButton
        android:id="@+id/default_activity_button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentBottom="true"
        android:layout_alignParentEnd="true"
        android:layout_margin="32dp"
        android:backgroundTint="@android:color/holo_green_dark"
        android:src="@drawable/ic_playlist_add"/>


</RelativeLayout>

<androidx.cardview.widget.Cardview xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_height="wrap_content"
    android:layout_width="wrap_content"
    xmlns:tool="http://schemas.android.com/tools"
    app:cardElevation="4dp"
    app:cardCornerRadius="8dp"
    android:layout_marginHorizontal="16dp"
    android:layout_marginVertical="8dp">

    <RelativeLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:padding="8dp"/>
    <CheckBox
        android:id="@+id/todoCheckBox"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        tool:text="This is an sample"
        android:paddingStart="8dp"
        android:buttonTint="@android:color/holo_green_light"
    <RelativeLayout


</androidx.cardview.widget.Cardview>



