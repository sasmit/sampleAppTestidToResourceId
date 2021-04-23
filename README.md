# sampleAppTestidToResourceId
Same react-native app to test testID replacement to resource-id while UI automation on android device. Please use UI Automator Viewer tool to test this feature.

Verified below componets with testID and accessibilityLabel props.

1) View
2) Text
3) Image
4) ScrollView
5) StausBar
6) Flatlist

**How to use**

1) Make sure your project is on react-native 0.64.0 version
2) Add the above props to your component like below
For ex:  <View style={styles.sectionContainer} testID={"main-view"} accessibilityLabel={"titleView"}>
3) Build and run your app in emulator/actual device
4) Open uiautomatorviewer.bat file from the below path
C:\Users\xyz\AppData\Local\Android\Sdk\tools\bin (in my windows machine this is the path. Please check yours)
6) Once uiautomatorviewer is launched please click on the icon "Device screeshot" from the top left screen of the tool
7) then in the top right side of the tool you see all of your component nodes, please select the one where you have used testID props
8) Now you should see testID is mapped to resource-id and acessibilityLabel mapped to content-desc. this is there in bottom right side of your tool.

screenshot attached 
![image](https://user-images.githubusercontent.com/1374490/115840898-d0e9b380-a439-11eb-8c3c-399188f8724c.png)
