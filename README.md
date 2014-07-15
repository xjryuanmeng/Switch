# Switch - iOS (Objective-C)

`Switch` is a `UIControl` subclass that creates a UISwitch like control with provided image.

## Requirements
* iOS 6.0 or later
* QuartzCore.framework
* ARC (either project has ARC ON or Switch is compiled with `-fobjc-arc`)

## How To Use
Using Switch is quite simple :
    UIImage* image = [UIImage imageNamed:@"switch.png"];
    Switch* mySwitch = [Switch switchWithImage:image visibleWidth:200];
    [mySwitch addTarget:self action:@selector(switchToggled:) forControlEvents:UIControlEventValueChanged];
    [self.view addSubview:mySwitch];
* Switch uses the image and visible width combination to toggle between states.
* You can provide cornerRadius of your choice to make it appear roundedCorner style or any other.

## What's the catch ?
You can provide any image, just one complete image containing ON-THUMB-OFF both states
(for reference, see `SwitchArtwork` in demo app) 
and visibleWidth to toggle between states, and that's it.

All that appearance depends on how creative your artwork is.

## How It Looks
![Screenshot1] (https://raw.githubusercontent.com/taruntyagi697/Switch/master/Screenshots/Screenshot1.png)
![Screenshot2] (https://raw.githubusercontent.com/taruntyagi697/Switch/master/Screenshots/Screenshot2.png)

    
## Demo App
    Demo app includes the most basic regular example just for reference.