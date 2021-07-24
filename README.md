# DottedDashedLine

![](https://github.com/gzeinnumer/DottedDashedLine/blob/master/preview/example1.jpg)

* dotted_line.xml
```xml
<?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android"
    android:shape="rectangle">
    <!--    android:shape="line">-->

    <corners android:radius="16dp" />

    <stroke
        android:width="1dp"
        android:color="@color/purple_700"
        android:dashWidth="10px"
        android:dashGap="10px" />
</shape>
```

* dotted_line_background.xml
```xml
<?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android"
    android:shape="rectangle">
    <!--    android:shape="line">-->

    <corners android:radius="16dp" />

    <solid android:color="#2D3700B3"/>

    <stroke
        android:width="1dp"
        android:color="@color/purple_700"
        android:dashWidth="10px"
        android:dashGap="10px" />
</shape>
```

* main_activity.xml
```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
    ...>

    <LinearLayout
        android:background="@drawable/dotted_line"
        ...>

        <TextView
            ...
            android:text="TextView Top" />

    </LinearLayout>

    <LinearLayout
        android:background="@drawable/dotted_line_background"
        ...>

        <TextView
            ...
            android:text="TextView Bottom" />

    </LinearLayout>
</LinearLayout>
```

---

```
Copyright 2021 M. Fadli Zein
```