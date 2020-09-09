# data-collection-on-android-devices
This is an apk to collect data from sensors on android devices.

 First, you need to make your Android devices turn on the developer options:
 settings->...->Build number, Quick continuous click it then it will pop up and tell you that "developer model is turned on".

 Second, connect your android device and the computer. Check the connection:
# adb devices
 then you will see the information of your android device on the computer.

 Third, install the apk:
# adb install \apkname
 you can also drop the apk to the window instead of typing \apkname

 Fourth, open the sensor data collect app on your android device and select sensors you want to use.
 To pull the data to the computer, the command is:
# adb pull '/sdcard/Sensor Data Collection/default' .
 To remove the data on your android device, the command is:
# rm -rf sdcard/Sensor\ Data\ Collection   

