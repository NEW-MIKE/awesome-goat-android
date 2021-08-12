<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="42dp"
    android:background="@color/colorPrimary"
    android:paddingLeft="24dp"
    android:paddingRight="24dp">

    <ImageView
        android:id="@+id/ivHomePage"
        android:layout_width="23dp"
        android:layout_height="23dp"
        android:src="@drawable/sel_btn_home_page"
        app:layout_constraintBottom_toTopOf="@+id/tvHomePage"
        app:layout_constraintEnd_toStartOf="@id/ivCommunity"
        app:layout_constraintHorizontal_chainStyle="spread_inside"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/tvHomePage"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:enabled="false"
        android:gravity="center"
        android:text="1111"
        android:textColor="@color/sel_bottom_navigation_bar_radio_color"
        android:textSize="8sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="@id/ivHomePage"
        app:layout_constraintStart_toStartOf="@id/ivHomePage"
        app:layout_constraintTop_toBottomOf="@id/ivHomePage"
         />

    <ImageView
        android:id="@+id/ivCommunity"
        android:layout_width="23dp"
        android:layout_height="23dp"
        android:padding="2dp"
        android:src="@drawable/sel_btn_home_page"
        app:layout_constraintBottom_toTopOf="@id/tvCommunity"
        app:layout_constraintEnd_toStartOf="@id/ivRelease"
        app:layout_constraintStart_toEndOf="@id/ivHomePage"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/tvCommunity"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:enabled="false"
        android:gravity="center"
        android:text="2222"
        android:textColor="@color/sel_bottom_navigation_bar_radio_color"
        android:textSize="8sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="@id/ivCommunity"
        app:layout_constraintStart_toStartOf="@id/ivCommunity"
        app:layout_constraintTop_toBottomOf="@+id/ivCommunity"
      />

    <ImageView
        android:id="@+id/ivRelease"
        android:layout_width="30dp"
        android:layout_height="30dp"
        android:src="@drawable/sel_btn_home_page"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toStartOf="@id/ivNotification"
        app:layout_constraintStart_toEndOf="@id/ivCommunity"
        app:layout_constraintTop_toTopOf="parent" />

    <ImageView
        android:id="@+id/ivNotification"
        android:layout_width="23dp"
        android:layout_height="23dp"
        android:padding="1dp"
        android:src="@drawable/sel_btn_home_page"
        app:layout_constraintBottom_toTopOf="@id/tvNotification"
        app:layout_constraintEnd_toStartOf="@id/ivMine"
        app:layout_constraintStart_toEndOf="@id/ivRelease"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/tvNotification"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:enabled="false"
        android:gravity="center"
        android:text="3333"
        android:textColor="@color/sel_bottom_navigation_bar_radio_color"
        android:textSize="8sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="@id/ivNotification"
        app:layout_constraintStart_toStartOf="@id/ivNotification"
        app:layout_constraintTop_toBottomOf="@+id/ivNotification"
         />

    <ImageView
        android:id="@+id/ivMine"
        android:layout_width="23dp"
        android:layout_height="23dp"
        android:padding="2dp"
        android:src="@drawable/sel_btn_home_page"
        app:layout_constraintBottom_toTopOf="@id/tvMine"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toEndOf="@id/ivNotification"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/tvMine"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:enabled="false"
        android:gravity="center"
        android:text="4444"
        android:textColor="@color/sel_bottom_navigation_bar_radio_color"
        android:textSize="8sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="@id/ivMine"
        app:layout_constraintStart_toStartOf="@id/ivMine"
        app:layout_constraintTop_toBottomOf="@+id/ivMine"

    />


    <androidx.constraintlayout.widget.Group
        android:id="@+id/btnHomePage"
        android:layout_width="0dp"
        android:layout_height="0dp"
        app:layout_constraintBottom_toBottomOf="@+id/tvHomePage"
        app:layout_constraintEnd_toEndOf="@id/ivHomePage"
        app:layout_constraintStart_toStartOf="@id/ivHomePage"
        app:layout_constraintTop_toTopOf="@+id/ivHomePage"
        tools:background="@color/blackAlpha50" />

    <androidx.constraintlayout.widget.Group
        android:id="@+id/btnCommunity"
        android:layout_width="0dp"
        android:layout_height="0dp"
        app:layout_constraintBottom_toBottomOf="@+id/tvCommunity"
        app:layout_constraintEnd_toEndOf="@id/ivCommunity"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="@id/ivCommunity"
        app:layout_constraintTop_toTopOf="@+id/ivCommunity"
        app:layout_constraintVertical_bias="0.0"
        tools:background="@color/blackAlpha50" />

    <androidx.constraintlayout.widget.Group
        android:id="@+id/btnNotification"
        android:layout_width="0dp"
        android:layout_height="0dp"
        app:layout_constraintBottom_toBottomOf="@+id/tvNotification"
        app:layout_constraintEnd_toEndOf="@id/ivNotification"
        app:layout_constraintStart_toStartOf="@id/ivNotification"
        app:layout_constraintTop_toTopOf="@+id/ivNotification"
        tools:background="@color/blackAlpha50" />

    <androidx.constraintlayout.widget.Group
        android:id="@+id/btnMine"
        android:layout_width="0dp"
        android:layout_height="0dp"
        app:layout_constraintBottom_toBottomOf="@+id/tvMine"
        app:layout_constraintEnd_toEndOf="@id/ivMine"
        app:layout_constraintStart_toStartOf="@id/ivMine"
        app:layout_constraintTop_toTopOf="@+id/ivMine"
        tools:background="@color/blackAlpha50" />

</androidx.constraintlayout.widget.ConstraintLayout>