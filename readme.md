# Blink Effect
## _A very simple android lib to apply Blink Effect to a view_

[![N|Solid](https://pngimg.com/uploads/android_logo/small/android_logo_PNG34.png)](https://nodesource.com/products/nsolid)

Blink effect is a very simple library that allows us to apply blink effet to:

- a view element

## How to import

- Step 1: Add it in your root build.gradle at the end of repositories:
```
allprojects {
	repositories {
		maven { url 'https://jitpack.io' }
	}
}
```
- Step 2: Add the dependency
````
dependencies {
    implementation 'com.github.emanoellucasml:blink-effect-android-lib:Tag'
}
````

## Usage

    private lateinit var btn : Button

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)
        actionBar?.hide()
        btn = findViewById(R.id.buttonView)
        btn.setOnClickListener {
            // use of blink-library
            BlinkEffect.blink(btn)
        }
    }

## Demonstration

![](https://github.com/emanoellucasml/blink-effect-android-lib/blob/master/demonstration.gif)
