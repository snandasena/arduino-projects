### Download & Install Arduino in Linux
```
wget https://downloads.arduino.cc/arduino-1.8.13-linux64.tar.xz
```
```
tar -xvf arduino-1.8.13-linux64.tar.xz
```
```
cd arduino-1.8.13
```
```
chmod +x install.sh
```
```
sudo ./install.sh
```
### Run fist Arduio program
Step 01: Connect your Arduino board using the USB cable  
Step 02: Open Arduio editor (commandline)
```
arduino 
```
Step 03: Run your first program. Sample can be found in bellow.  
```
void setup() {
  // put your setup code here, to run once:
  pinMode(13,OUTPUT);

}

void loop() {
  // put your main code here, to run repeatedly:
  digitalWrite(13, HIGH);
  delay(1000);
  digitalWrite(13, LOW);
  delay(100);
}
```

Step 04: Verify and upload it.  
If you get any permission issues, Goto Tools -> Port and and find the device ( sample /dev/ttyUSB0) 
```
sudo chmod a+rw /dev/ttyUSB0
```
### Tips
01: How can be compile and upload arduino sketch using commandline
```
arduino --upload /path/to/file.ino
```

### Acknowledgement
[Ref:01](https://github.com/arduino/Arduino/blob/master/build/shared/manpage.adoc)
