# Mars-rover-panoarama-viewer
View and manipulate Mars panoramas from MSL and MARS2020 rovers. Feed croppings to AI video generator to create a video with smooth transition between start and end frame.


Source images for Curiosity: https://stevealbers.net/allsky/sites/curiosity/cyl_mosaics/

## Instructions
- Open the [panorama viewer/marker](https://jumpjack.github.io/Mars-rover-panorama-viewer/curiosity-pano.html)
- Press left and right keys on keyboard to browse through panoramas (first time it will take a while to load each one)
   - Left-click mouse to rotate the view
   - Use mouse wheel to zoom
   - Right-click to set a marker on each image, then if "center" checkbox is checked, each image will be centered on its marker upon browsing
   - Activate "crop" checkbox to show the area to be cropped
   - Click on "save crop" to save a screenshot of the cropped area
   - Click on "export markers" to save all markers of all images for future use; click on "import" to load them back in memory
 - Once you exported the needed frames, you can open them into [this page](https://jumpjack.github.io/Mars-rover-panorama-viewer/fotogrammetria.html) to manually match same features in two different images, and save the marked images as separate images
 - Once you have two different images matched with same features, feed them into [Pixverse.ai](https://app.pixverse.ai/creation/video) to get a video-transition between two frames

## Example of prompts 

Notes: 
- the more you repeat, the better it understands... 
- if AI keeps adding random rocks or dust devils, it means it does not have enough markers in that area

### Getting closer to horizon:
 _Simulate camera motion from first position to second position,  move closer to horizon,  some features disappear under bottom edge of frame, keep consistency of color markers,  keep consistency of  terrain,  keep consistency of  rocks, don't add rocks, don't add anything, smooth transition, don't add dust devils, remove color markers, don't add rocks, don't add any object, all rocks are static, only camera moves,  don't add moving rocks, don't add rocks,  keep consistency of color markers, there are no moving rocks, don't add moving rocks, all rocks stick to terrain, keep consistency of all features,there are no moving rocks, don't add moving rocks_

 _**Note**: getting closer to horizon is easier for AI because it doesn't need to invent features entering the scene, it has just to move them away._
  
