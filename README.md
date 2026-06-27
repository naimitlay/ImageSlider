# ImageSlider
===========================
ImageSlider


XML
----

<androidx.cardview.widget.CardView
        android:id="@+id/cardimg"
        android:layout_width="match_parent"
        android:layout_height="190dp"
        android:layout_marginHorizontal="10dp"
        android:layout_marginTop="10dp"
        app:cardCornerRadius="12dp"
        app:cardElevation="6dp"
        app:cardBackgroundColor="@android:color/white">

        <com.denzcoskun.imageslider.ImageSlider
            android:id="@+id/image_slider"
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            app:iss_auto_cycle="true"
            app:iss_delay="0"
            app:iss_period="3000"
            app:iss_text_align="CENTER"
            app:iss_title_background="@color/grey_font"
            tools:ignore="MissingClass" />

    </androidx.cardview.widget.CardView>
    
    ================================================================================
    
    java
    -----------
    
    // Initialize ImageSlider
        imageSlider = findViewById(R.id.image_slider);

        // Populate Image List
        imageList.add(new SlideModel(R.drawable.islame,  ScaleTypes.CENTER_CROP));
        imageList.add(new SlideModel(R.drawable.islame,  ScaleTypes.CENTER_CROP));

        // Set Image List to Slider
        imageSlider.setImageList(imageList);
        
        =============================================================================================
        
===================================================
Libery        
// Image Slider dependency ........
   
    implementation 'com.github.denzcoskun:ImageSlideshow:0.1.2'
============================================================================
