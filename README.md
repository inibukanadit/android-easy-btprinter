## Android BTPrinter - Easy Bluetooth Device (Printer) Manager

[![](https://jitpack.io/v/inibukanadit/android-easy-btprinter.svg)](https://jitpack.io/#inibukanadit/android-easy-btprinter)

No more struggle on discovering, storing or picking stored devices to print directly.


Favorite Devices
---
![](https://i.ibb.co/jf3kV78/image.png "Title")
![](https://i.ibb.co/s90FL2h/image.png "Title")


Device Discoveries
---
![](https://i.ibb.co/zmN0ybh/image.png "Title")
![](https://i.ibb.co/Jr5DsD9/image.png "Title")


Test Printing
---
![](https://i.ibb.co/FYrtTDg/image.png "Title")


[Currently under development state]

Add the activity into your `AndroidManifest.xml` :
```Androidmanifest.xml
<activity
  android:name="com.inibukanadit.easybtprinter.ui.BTPrinterActivity"
  android:theme="@style/AppTheme.NoActionBar" />
```

Ensure to use only `.NoActionBar` themes :
```styles.xml
<style name="AppTheme.NoActionBar" parent="Theme.AppCompat.Light.NoActionBar">
  <item name="colorPrimary">@color/colorPrimary</item>
  <item name="colorPrimaryDark">@color/colorPrimaryDark</item>
  <item name="colorAccent">@color/colorAccent</item>
</style>
```

Start the activity through your application :
```kotlin
startActivity(Intent(this, BTPrinterActivity::class.java))
```

**Warning** - This library needs DataBinding feature enabled to run completely. (will be improved in the future)

In Development
- [x] Device discoveries
- [x] Store a printer device - possible even on before or after test print
- [x] Test print directly - in discovery page
- [x] Test print directly - in stored devices page
- [ ] Reusable dialog call - callable everywhere, to print on choosen favorite (stored) device
- [ ] Make a stored device as 'default'

Improvements
- [ ] Remove data binding dependent
