# RippleEffect

How to Use : 

Step 1 : Add the JitPack repository to your build file

Add it in your root build.gradle at the end of repositories:

allprojects {

	repositories {
	
		...
		
		maven { url 'https://jitpack.io' }
		
	}
	
}

Step 2. Add the dependency

dependencies {

	implementation 'com.github.jainam69:RippleEffect:1.0.0'

}

In Android App,


<com.jainamdoshi.effectripple.RippleBackground

	android:layout_width="match_parent"
	
	android:layout_height="match_parent"
	
	android:id="@+id/content"
	
	app:rb_color="#0099CC"
	
	app:rb_radius="32dp"
	
	app:rb_rippleAmount="6"
	
	app:rb_duration="3000"
	
	app:rb_scale="6">

	<ImageView
		android:layout_width="64dp"
		android:layout_height="64dp"
		android:layout_centerInParent="true"
		android:id="@+id/centerImage"
		android:src="@drawable/phone1"/>
</com.jainamdoshi.effectripple.RippleBackground>


final RippleBackground rippleBackground=(RippleBackground)findViewById(R.id.content);

rippleBackground.startRipple();

