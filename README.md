# android-accessibility-overlay
Small example demonstrating overlay windows with accessibility service on Android.

Class `MyAccessibilityService` creates a small overlay view at a fixed location and adds it to the window manager with type
`LayoutParams.TYPE_ACCESSIBILITY_OVERLAY`. This ensures that the view is (almost?) always displayed even in e.g. the Android
settings menu. The overlay view can receive touch events and will change color when touched.

Class `MyActivity` is the main activity and registered with the launcher. It provides a button for directly navigating to the
Android accessibility settings.

For further details please refer to the Android developer documentation about
[creating an accessibility service](https://developer.android.com/guide/topics/ui/accessibility/service) and 
[TYPE_ACCESSIBILITY_OVERLAY](https://developer.android.com/reference/android/view/WindowManager.LayoutParams#TYPE_ACCESSIBILITY_OVERLAY)
in particular.
