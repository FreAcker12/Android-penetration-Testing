<h1># Android-penetration-Testing</h1>
<h2>Quick Alert 🚨</h2>
<h4>&nbsp;&nbsp;&nbsp;&nbsp&nbsp;•&nbsp;&nbsp;This repo meant to get you familiar very quickly with Android penetration testing.</h4>
<h4>&nbsp;&nbsp;&nbsp;&nbsp&nbsp;•&nbsp;&nbsp;This repo does not include installations guidance.</h4>
<hr>
<h2>The ADB (Android Debug Bride)</h2>
<b>P.S. Please add youe adb to the user/system environment path so you can access it easier, if you're using USB connected device, please install scrcpy to mirror your screen</b>
<br><br>
<b>1. Root your shell on the device automatically - This helps with port forward/reverse, files trasnfer etc.</b>
<pre>
C:\Users\user>adb root
Result: restarting adbd as root
</pre>
<b>2. List all devices</b>
<pre>
C:\Users\user>adb devices
List of devices attached
emulator-5554   device
</pre>
<b>3. Connect to your device (If multiple)</b>
<pre>
C:\Users\user>adb -s &lt;Device Name&gt; shell
generic_x86_arm:/ #
</pre>
<b>or via IP address</b>
<pre>
adb connect &lt;IP_ADD&gt;:&lt;PORT&gt;
</pre>
<b>4. Install your APK file</b>
<pre>
C:\Users\user>adb install file.apk
</pre>
<b>5. Upload (push) / Download (pull) files</b>
<pre>
C:\Users\user>adb pull / push &lt;source&gt &lt;destination&gt;
</pre>
<b>6. Extract network and log details such as HCI (can be opened via wireshark)</b>
<pre>
C:\Users\user>adb bugreport &lt;file&gt.zip
</pre>
<b>7. Get logs</b>
<pre>
C:\Users\user>adb logcat
</pre>
