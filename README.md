# Layout

## 1.利用线性布局实现如下界面  

![Image text](https://github.com/chenzifeng123/image/blob/master/2_001.png)

    <LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical">
    
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">

        <Button
            android:id="@+id/btn_11"
            style="?android:attr/buttonStyle"
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:text="@string/One_One"
            android:textAllCaps="false" />

        <Button
            android:id="@+id/btn_12"
            style="?android:attr/buttonStyle"
            android:layout_width="112dp"
            android:layout_height="wrap_content"
            android:text="@string/One_Two"
            android:textAllCaps="false" />

        <Button
            android:id="@+id/btn_13"
            style="?android:attr/buttonStyle"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/One_Three"
            android:textAllCaps="false" />

        <Button
            android:id="@+id/btn_14"
            style="?android:attr/buttonStyle"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/One_Four"
            android:textAllCaps="false" />
    </LinearLayout>

    <LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">

        <Button
            android:id="@+id/btn_21"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            style="?android:attr/buttonStyle"
            android:textAllCaps="false"
            android:text="@string/Two_One" />

        <Button
            android:id="@+id/btn_22"
            style="?android:attr/buttonStyle"
            android:layout_width="112dp"
            android:layout_height="wrap_content"
            android:text="@string/Two_Two"
            android:textAllCaps="false" />

        <Button
            android:id="@+id/btn_23"
            style="?android:attr/buttonStyle"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textAllCaps="false"
            android:text="@string/Two_Three" />

        <Button
            android:id="@+id/btn_24"
            style="?android:attr/buttonStyle"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/Two_Four"
            android:textAllCaps="false" />
    </LinearLayout>


    <LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">

        <Button
            android:id="@+id/btn_31"
            style="?android:attr/buttonStyle"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/Three_One"
            android:textAllCaps="false" />

        <Button
            android:id="@+id/btn_32"
            style="?android:attr/buttonStyle"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/Three_Two"
            android:textAllCaps="false" />
        <Button
            android:id="@+id/btn_33"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            style="?android:attr/buttonStyle"
            android:textAllCaps="false"
            android:text="@string/Three_Three"/>
        <Button
            android:id="@+id/btn_34"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            style="?android:attr/buttonStyle"
            android:textAllCaps="false"
            android:text="@string/Three_Four"/>
    </LinearLayout>


    <LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">

        <Button
            android:id="@+id/btn_41"
            style="?android:attr/buttonStyle"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/Four_One"
            android:textAllCaps="false" />

        <Button
            android:id="@+id/btn_42"
            style="?android:attr/buttonStyle"
            android:layout_width="111dp"
            android:layout_height="wrap_content"
            android:text="@string/Four_Two"
            android:textAllCaps="false" />
        <Button
            android:id="@+id/btn_43"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            style="?android:attr/buttonStyle"
            android:textAllCaps="false"
            android:text="@string/Four_Three"/>
        <Button
            android:id="@+id/btn_44"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            style="?android:attr/buttonStyle"
            android:textAllCaps="false"
            android:text="@string/Four_Four"/>
    </LinearLayout>


 </LinearLayout>


## 2.利用ConstraintLayout实现如下界面：

![Image text](https://github.com/chenzifeng123/image/blob/master/2_002.png)   

    
    <RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:paddingBottom="300dp"
    >
    <Button
        android:id="@+id/btn_red"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentStart="true"
        android:layout_alignParentTop="true"
        android:text="@string/red"
        android:background="@color/colorAccent" />
    <Button
        android:id="@+id/btn_orange"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentTop="true"
        android:layout_marginStart="9dp"
        android:layout_marginTop="0dp"
        android:layout_toEndOf="@+id/btn_green"
        android:background="@android:color/holo_orange_dark"
        android:text="@string/orange" />
    <Button
        android:id="@+id/btn_yellow"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentTop="true"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_marginTop="0dp"
        android:layout_marginEnd="0dp"
        android:layout_marginRight="0dp"
        android:text="@string/yellow"
        android:background="@android:color/holo_orange_light" />

    <Button
        android:id="@+id/btn_green"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignTop="@+id/btn_blue"
        android:layout_alignParentStart="true"
        android:layout_marginStart="51dp"
        android:layout_marginTop="1dp"
        android:background="@android:color/holo_green_light"
        android:text="@string/green" />

    <Button
        android:id="@+id/btn_blue"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentStart="true"
        android:layout_alignParentTop="true"
        android:layout_marginStart="147dp"
        android:layout_marginTop="83dp"
        android:background="@android:color/holo_blue_bright"
        android:text="@string/blue" />
    <Button
        android:id="@+id/btn_indigo"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentTop="true"
        android:layout_alignParentEnd="true"
        android:layout_marginStart="7dp"
        android:layout_marginTop="84dp"
        android:layout_marginEnd="51dp"
        android:layout_toEndOf="@+id/btn_blue"
        android:background="@android:color/holo_blue_dark"
        android:text="@string/indigo" />
    <Button
        android:id="@+id/btn_violet"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_alignParentStart="true"
        android:layout_alignParentBottom="true"
        android:layout_marginStart="0dp"
        android:layout_marginBottom="0dp"
        android:text="@string/violet"
        android:background="@android:color/holo_purple" />
     </RelativeLayout>


   
## 3.利用表格布局实现如下界面：

<img width="400" height="300" src="https://github.com/chenzifeng123/image/blob/master/2_004.png"/>

    <TableLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:stretchColumns="1"
    >
    <TableRow>
    <TextView
            android:layout_marginLeft="13dp"
            android:layout_width="268dp"
            android:padding="3dip"
            android:text="@string/table_open" />
        <TextView
            android:gravity="end"
            android:padding="3dip"
            android:text="@string/table_open_shortcut" />
    </TableRow>
    <TableRow>
        <TextView
            android:layout_marginLeft="13dp"
            android:padding="3dip"
            android:text="@string/table_save" />
        <TextView
            android:text="@string/table_save_shortcut"
            android:gravity="end"
            android:padding="3dip"/>
    </TableRow>
    <TableRow>
        <TextView
            android:layout_marginLeft="13dp"
            android:text="@string/table_save_as"
            android:padding="3dip"/>
        <TextView
            android:gravity="end"
            android:padding="3dip"
            android:text="@string/table_save_as_shortcut" />
    </TableRow>

    <View
        android:layout_height="1px"
        android:background="#000000"
        android:layout_width="fill_parent"></View>

    <TableRow>
        <TextView
            android:text="@string/table_x_import"
            android:padding="3dip"/>
    </TableRow>
    <TableRow>
        <TextView
            android:text="@string/table_x_export"
            android:padding="3dip"/>
        <TextView
            android:gravity="end"
            android:padding="3dip"
            android:text="@string/table_x_export_shortcut" />
    </TableRow>
    <View
        android:layout_height="1px"
        android:background="#000000"
        android:layout_width="fill_parent"></View>

    <TableRow>
        <TextView
            android:layout_marginLeft="13dp"
            android:text="@string/table_quit"
            android:padding="3dip"/>
    </TableRow>

    </TableLayout>





