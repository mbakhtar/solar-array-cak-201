# Solar Array CAK V2.0 - Jacdac

```package
jacdac=github:microsoft/pxt-jacdac
jacdac-servo=github:microsoft/pxt-jacdac/servo
jacdac-light-level=github:microsoft/pxt-jacdac/light-level
```
## @showhint
Create a ``||Variables:Variable position||`` and nest ``||Variables:set position to -90||`` 
under ``||basic:on start||`` block
```blocks
let position = -90
```

## @showhint
Now add ``||modules:set servo4 ON||``
```blocks
let position = -90
modules.servo4.setEnabled(true)
```
## @showhint
Now nest an ``||logic:If true then else||`` block under the ``||basic:forever||`` loop
```blocks
let position = -90
modules.servo4.setEnabled(true)
basic.forever(function(){
    if(true){
    }
    else{
    }
})
```
## @showhint
Add a ``||logic:comparison block||`` from the ``||logic:Logic drawer||`` place it in the true
condition of the ``||logic: if then else||`` loop
```blocks
let position = -90
modules.servo4.setEnabled(true)
basic.forever(function(){
    if(||){
    }
    else{
    }
})
```
## @showhint
Insert the block ``||modules:light level2 light level %||`` under ``||i||``
and insert ``||75||`` under ``||j||``
```blocks
modules.servo4.setEnabled(true)
modules.servo4.setAngle(0)
let position = -90
basic.forever(function () {
    if (modules.lightLevel2.lightLevel() > 75) {
            } else {
            }
})
```
## @showhint
If the condition is true add ``||basic:show icon||`` block and 
select ``||basic:target icon||``
```blocks
modules.servo4.setEnabled(true)
modules.servo4.setAngle(0)
let position = -90
basic.forever(function () {
    if (modules.lightLevel2.lightLevel() > 75) {
        basic.showIcon(IconNames.Target)
    } else {
            }
})
```
## @showhint
If the condition is false add ``||basic:show icon||`` block under the 
``||logic:else||`` and select ``||basic: small diamond icon||``
```blocks
modules.servo4.setEnabled(true)
modules.servo4.setAngle(0)
let position = -90
basic.forever(function () {
    if (modules.lightLevel2.lightLevel() > 75) {
        basic.showIcon(IconNames.Target)
    } else {
        basic.showIcon(IconNames.SmallDiamond)
        }
    }
})
```

## @showhint
Now add ``||Variables:change position by 10||`` block under 
the ``||basic:small diamond icon||``
```blocks
modules.servo4.setEnabled(true)
modules.servo4.setAngle(0)
let position = -90
basic.forever(function () {
    if (modules.lightLevel2.lightLevel() > 75) {
        basic.showIcon(IconNames.Target)
    } else {
        basic.showIcon(IconNames.SmallDiamond)
        position += 10
            }
})
```

## @showhint
Add ``||logic:if true then||`` block under the 
``||logic:else||`` condition below the 
``||Variables:change position by 10||``
```blocks
modules.servo4.setEnabled(true)
modules.servo4.setAngle(0)
let position = -90
basic.forever(function () {
    if (modules.lightLevel2.lightLevel() > 75) {
        basic.showIcon(IconNames.Target)
    } else {
        basic.showIcon(IconNames.SmallDiamond)
        position += 10
        if () {
              }
        }
})
```
## @showhint
For the true condition replace it by a ``||logic:comparison||`` block
```blocks
modules.servo4.setEnabled(true)
modules.servo4.setAngle(0)
let position = -90
basic.forever(function () {
    if (modules.lightLevel2.lightLevel() > 75) {
        basic.showIcon(IconNames.Target)
    } else {
        basic.showIcon(IconNames.SmallDiamond)
        position += 10
        if ( > ) {
                 }
        }
})
```
## @showhint
For the comparison add ``||Variables:position||`` on the left side and 
compare with ``||90||``
```blocks
modules.servo4.setEnabled(true)
modules.servo4.setAngle(0)
let position = -90
basic.forever(function () {
    if (modules.lightLevel2.lightLevel() > 75) {
        basic.showIcon(IconNames.Target)
    } else {
        basic.showIcon(IconNames.SmallDiamond)
        position += 10
        if (position > 90) {
            
        }
        
    }
})
```
## @showhint
For the true condition add ``||Variables:set position to -90||`` 
nested under the ``||logic:if position>90 then||``
```blocks
modules.servo4.setEnabled(true)
modules.servo4.setAngle(0)
let position = -90
basic.forever(function () {
    if (modules.lightLevel2.lightLevel() > 75) {
        basic.showIcon(IconNames.Target)
    } else {
        basic.showIcon(IconNames.SmallDiamond)
        position += 10
        if (position > 90) {
            position = -90
        }
        
    }
})
```
## @showhint
Add ``||modules: set servo4 angle to||`` block and insert ``||Variables:position||`` 
block in it. This is places after the ``||logic:if then||`` block 
Also add a ``||basic:pause||`` block and set it to ``||basic:20ms||``
```blocks
modules.servo4.setEnabled(true)
modules.servo4.setAngle(0)
let position = -90
basic.forever(function () {
    if (modules.lightLevel2.lightLevel() > 75) {
        basic.showIcon(IconNames.Target)
    } else {
        basic.showIcon(IconNames.SmallDiamond)
        position += 10
        if (position > 90) {
            position = -90
        }
        modules.servo4.setAngle(position)
        basic.pause(20)
    }
})
```
## @showhint
This is the final code
```blocks
modules.servo4.setEnabled(true)
modules.servo4.setAngle(0)
let position = -90
basic.forever(function () {
    if (modules.lightLevel2.lightLevel() > 75) {
        basic.showIcon(IconNames.Target)
    } else {
        basic.showIcon(IconNames.SmallDiamond)
        position += 10
        if (position > 90) {
            position = -90
        }
        modules.servo4.setAngle(position)
        basic.pause(20)
    }
})
```

Congratulations, you did it!