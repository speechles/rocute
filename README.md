# rocute
beautiful ui components for roku development

## About
rocute is an open source component library to aid developers in creating beautiful roku apps in a 
timely manner. Our library includes styled components, animations, and screensavers ready for easy 
out of the box implementation.

## Example and Setup
### Example
```xml
<!-- The SceneGraph component you are working in -->
<?xml version="1.0" encoding="utf-8" ?>
<component name="BounceEffectExampleComponent" extends="Panel" >
  <script type="text/brightscript" uri="pkg:/components/examples/BounceEffectExample/BounceEffectExample.brs"/>
  <children>
    <!-- Implementation of our component -->
    <BounceEffect id="BounceEffectExample" imageUri="pkg:/images/test.png" startPoint="[250, 250]" maxHeight="100" bounceType="descending" totalBounces="3" duration="2" repeat="false" />
  </children>
</component>
```
### Setup
#### To utilize a component:
 - Navigate to `./src/main/components` in the rocute directory.
 - Dependent on if you want a general styled component, or an animation, or a video-overlay, select either the `styled-components`, or `animations`, or `video-overlays` directory.
 - Copy the directory of the component you want into an appropriate place in your codebase.
 - For component specific documentation, refer to the ThatComponent.md file in the component's example directory.
#### For access to all components:
 - Copy the components directory out of `./src/main` into your project structure in an appropriate place.
 - Import any and all components into your project.
 - For component specific documentation, refer to the ThatComponent.md file in the component's example directory.
#### To run our app:
 - Install ukor: `npm install -g @willowtreeapps/ukor`.
 - Install [vscode.](https://code.visualstudio.com/)
 - Install [vscode brightscript.](https://marketplace.visualstudio.com/items?itemName=celsoaf.brightscript)
 - Open the root directory of our repo in vscode.
 - Modify `.vscode/launch.json` so the inputs resemble `"default": "0.0.0.0",` to your roku ip address, and `"default": "password",` to your roku password.
 - Click the debug tab in vscode.
 - Press the dropdown button next to the play button and select `Brightscript Debug: Launch`.
 - Press the play button next to the dropdown.


## Components

**ArchInterpolator -**
A type of Vector2DInterpolator which can be used to animate a smooth arc through three points. 

**BounceEffect -**
A customizable bounce which can be applied to any image.

**CardRotator -**
A card rotary which moves on the y axis.

**CardZoomDiagonal -**
An overlapping card rotator where cards slide from the top left to front center, and the cards
that will be shown sooner overlap the ones that will be shown later.

**CardZoomRotary -**
An overlapping card rotator where cards are visually pulled from the back to the front center.

**CircularImageClip -**
A circular border to be placed on images, which will stretch to oval bounds 
if proper heights and widths are provided.

**Clock -**
A Clock component similar to the clock inside of the Overhang component.

**DatePicker -**
A Date Picker component comprised of three LabelLists. Includes localization options.

**DisappearingLogo -**
An image overlay for a video which appears in a corner (or anywhere) and fades away after a certain amount of time.

**DisappearingNav -**
A Horizontal Nav Bar which fades up (or down) and away when it loses focus.

**HorizontalCardRotator -**
A card rotary which moves on the x axis.

**LiveIcon -**
A video overlay displayed on Live video steams but not on prerecorded content.

**NavBar -**
A Horizontal Nav Bar component. 

**Next -**
The 'Next' component is an stubbed out component for development. If you are interested in
contributing, this component is here to help. Instructions can be found in the NextExample
directory.

**RandomColoredFontList -**
RandomColoredFontList is a LabelList component that will randomly change the font color of the 
selected element.

**RandomColoredList -**
RandomColoredList is a LabelList component that will randomly change the color of the 
selected element.

**RatingIcon -**
A video overlay which displays the rating of the video if given, and then fades out after a certain amount of time.

**ResizeList -**
ResizeList is a LabelList component that will resize so the currently selected element 
takes up more space.

**Ticker -**
A news ticker component which scrolls text from right to left across the screen.

**TiledBackground -**
A rectangle with an image tiled to fill its area.

**TriangularCornerClip -**
TriangularCornerClip is a way to clip an image to fit into the bounds of a right triangle. 

**TriangularImageClip -**
TriangularImageClip is a way to clip an image to fit in a triangle. As opposed to 
TriangularCornerClip, this triangular clip component will stretch to your image and remain 
centric on the middle of the image.

## Screensavers

**BouncingLogoScreensaver -**
A screensaver channel where a provided logo will bounce around the edges of the screen. 

**ExpandingLogoScreensaver -**
A screensaver channel where a provided logo will expand and contract in the center of the screen.

## Questions
Join us in the #tooling channel on the [Roku Developers Slack](https://rokudevelopers.slack.com).

## Contributing
Contributions and suggestions are more than welcome. Please see our [Code of Conduct](/CODE_OF_CONDUCT.md)
as well as our [Contributing Guidelines ](/CONTRIBUTING.md) for more information.