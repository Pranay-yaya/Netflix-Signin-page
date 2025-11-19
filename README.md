# Netflix-Signin-page
<?xml version="1.0" encoding="utf-8"?>
<ScrollView xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#000000"
    android:fillViewport="true"
    tools:context=".MainActivity">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        android:padding="24dp">

        <ImageView
            android:id="@+id/iv_netflix_logo"
            android:layout_width="400dp"
            android:layout_height="250dp"
            android:layout_gravity="center_horizontal"
            android:layout_marginBottom="48dp"
            android:src="@drawable/n"
            android:contentDescription="Netflix Logo" />

        <TextView
            android:id="@+id/tv_sign_in_title"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginBottom="24dp"
            android:fontFamily="sans-serif-medium"
            android:gravity=""
            android:text="Sign In"
            android:textColor="#FFFFFF"
            android:textSize="42sp"
            android:textStyle="bold" />

        <com.google.android.material.textfield.TextInputLayout
            android:id="@+id/til_email"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginBottom="16dp"
            android:hint="Email or phone number"
            app:boxStrokeColor="#FFFFFF"
            app:boxStrokeWidth="1dp"
            app:hintTextColor="#B3FFFFFF"
            style="@style/Widget.MaterialComponents.TextInputLayout.OutlinedBox">

            <com.google.android.material.textfield.TextInputEditText
                android:id="@+id/et_email"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:background="@android:color/transparent"
                android:inputType="textEmailAddress"
                android:padding="16dp"
                android:text="Your Name"
                android:textColor="#FFFFFF"
                android:textColorHint="#B3FFFFFF"
                android:textSize="16sp" />

        </com.google.android.material.textfield.TextInputLayout>

        <com.google.android.material.textfield.TextInputLayout
            android:id="@+id/til_password"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginBottom="24dp"
            android:hint="Password"
            app:boxStrokeColor="#E50914"
            app:boxStrokeWidth="1dp"
            app:endIconMode="password_toggle"
            app:hintTextColor="#B3FFFFFF"
            style="@style/Widget.MaterialComponents.TextInputLayout.OutlinedBox">

            <com.google.android.material.textfield.TextInputEditText
                android:id="@+id/et_password"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:background="@android:color/transparent"
                android:inputType="textPassword"
                android:padding="16dp"
                android:text="Registration Number"
                android:textColor="#FFFFFF"
                android:textColorHint="#B3FFFFFF"
                android:textSize="16sp" />

        </com.google.android.material.textfield.TextInputLayout>

        <Button
            android:id="@+id/btn_sign_in"
            android:layout_width="match_parent"
            android:layout_height="48dp"
            android:layout_marginBottom="16dp"
            android:backgroundTint="#E50914"
            android:text="Sign In"
            android:textAllCaps="false"
            android:textColor="#FFFFFF"
            android:textSize="16sp"
            android:textStyle="bold" />
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginBottom="24dp"
            android:orientation="horizontal"
            android:gravity="center_vertical">

            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:orientation="horizontal"
                android:gravity="center_vertical">

                <CheckBox
                    android:id="@+id/cb_remember_me"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:buttonTint="#B3FFFFFF"
                    android:checked="false"
                    android:background="?android:attr/selectableItemBackgroundBorderless"
                    android:focusable="false" />

                <TextView
                    android:id="@+id/tv_remember_me"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_marginStart="8dp"
                    android:text="Remember me"
                    android:textColor="#B3FFFFFF"
                    android:textSize="14sp" />

            </LinearLayout>

            <View
                android:layout_width="0dp"
                android:layout_height="0dp"
                android:layout_weight="1" />

            <TextView
                android:id="@+id/tv_need_help"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="Need help?"
                android:textColor="#B3FFFFFF"
                android:textSize="14sp"
                android:textStyle="bold" />

        </LinearLayout>

        <Button
            android:id="@+id/btn_login_facebook"
            android:layout_width="match_parent"
            android:layout_height="48dp"
            android:layout_marginBottom="48dp"
            android:backgroundTint="#4267B2"
            android:text="Login with Facebook"
            android:textAllCaps="false"
            android:textColor="#FFFFFF"
            android:textSize="16sp" />

        <TextView
            android:id="@+id/tv_display"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:background="#333333"
            android:gravity="center"
            android:padding="16dp"
            android:text="@string/output_will_appear_here_on_sign_in_click"
            android:textColor="#FFFFFF"
            android:textSize="14sp"
            android:visibility="visible" />

    </LinearLayout>

</ScrollView>
