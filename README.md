# BottomNavigation

## Download  
build.gradle (project path)  
```groovy  
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```   
dependencies {  
 implementation 'com.github.chetankoli1.BottomNavigation:chetanbottomnavigation:0.0.3'
 }  
``` 

## Listeners  
```java  
bottomNavigation.setOnClickMenuListener(new MeowBottomNavigation.ClickListener() {  
    @Override  
  public void onClickItem(MeowBottomNavigation.Model item) {  
        // your codes
  }  
});  
  
bottomNavigation.setOnShowListener(new MeowBottomNavigation.ShowListener() {  
    @Override  
  public void onShowItem(MeowBottomNavigation.Model item) {  
        // your codes
  }  
});  
  
bottomNavigation.setOnReselectListener(new MeowBottomNavigation.ReselectListener() {  
    @Override  
  public void onReselectItem(MeowBottomNavigation.Model item) {  
        // your codes
  }  
});
```
  
## Counter Badge  
Setting One Tab  
```java  
bottomNavigation.setCount(TAB_ID, STRING)  
```  
  
Clearing One Tab  
```java
bottomNavigation.clearCount(TAB_ID)  
```  
  
Clearing All Tabs  
```java
bottomNavigation.clearAllCounts(TAB_ID)  
```  
  
## Set Default Tab  
Use this function  
```java
bottomNavigation.show(TAB_ID)  
```
