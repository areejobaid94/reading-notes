#  Audio, Video, Images

## Images

![](https://i.morioh.com/2019/10/26/7be606912b97.jpg)

The HTML `<img>` tag is used to embed an image in a web page.

Images are not technically inserted into a web page; images are linked to web pages. The <img> tag creates a holding space for the referenced image.

The `<img>` tag is empty, it contains attributes only, and does not have a closing tag.

The `<img>` tag has two required attributes:

src - Specifies the path to the image
alt - Specifies an alternate text for the image

###### Example:
```
<img src="url" alt="alternatetext">
```

#### SRC:

The required src attribute specifies the path (URL) to the image.

Note: When a web page loads; it is the browser, at that moment, that gets the image from a web server and inserts it into the page. Therefore, make sure that the image actually stays in the same spot in relation to the web page, otherwise your visitors will get a broken link icon. The broken link icon and the alt text are shown if the browser cannot find the image.

###### Example:
```
<img src="img_chania.jpg" alt="Flowers in Chania">
```

#### Image Size:

You can use the style attribute to specify the width and height of an image.

To use an image as a link, put the `<img>` tag inside the `<a>` tag:

Use the CSS float property to let the image float to the right or to the left of a text:

Use the HTML `<img>` element to define an image

Use the HTML src attribute to define the URL of the image

Use the HTML alt attribute to define an alternate text for an image, if it cannot be displayed

Use the HTML width and height attributes or the CSS width and height properties to define the size of the image

Use the CSS float property to let the image float to the left or to the right


## Video and Audio APIs

The HTML5 DOM has methods, properties, and events for the <audio> and <video> elements.
	
| Method | Description |
| ------ | ----------- |
| addTextTrack() | Adds a new text track to the audio/video |
| canPlayType() | Checks if the browser can play the specified audio/video type |
| load() | Re-loads the audio/video element |
| play() | Starts playing the audio/video |
| pause() | Pauses the currently playing audio/video |


#### HTML Audio/Video Events

| Event | Description |
| ----- | ----------- |
| abort | Fires when the loading of an audio/video is aborted | 
| canplay | Fires when the browser can start playing the audio/video | 
| canplaythrough | Fires when the browser can play through the audio/video without stopping for buffering |
| durationchange | Fires when the duration of the audio/video is changed |
| emptied | Fires when the current playlist is empty |
| ended | Fires when the current playlist is ended |
| error	| Fires when an error occurred during the loading of an audio/video| 
| loadeddata	| Fires when the browser has loaded the current frame of the audio/video| 
| loadedmetadata	| Fires when the browser has loaded meta data for the audio/video| 
| loadstart	| Fires when the browser starts looking for the audio/video| 
| pause	| Fires when the audio/video has been paused| 
| play	| Fires when the audio/video has been started or is no longer paused| 
| playing	| Fires when the audio/video is playing after having been paused or stopped for buffering| 
| progress	| Fires when the browser is downloading the audio/video| 
| ratechange	| Fires when the playing speed of the audio/video is changed| 
| seeked	| Fires when the user is finished moving/skipping to a new position in the audio/video| 
| seeking	| Fires when the user starts moving/skipping to a new position in the audio/video| 
| stalled	| Fires when the browser is trying to get media data, but data is not available| 
| suspend	| Fires when the browser is intentionally not getting media data| 
| timeupdate	| Fires when the current playback position has changed| 
| volumechange	| Fires when the volume has been changed| 
| waiting	| Fires when the video stops because it needs to buffer the next frame| 

### The HTMLMediaElement API

#### Part of the HTML5 spec, the HTMLMediaElement API provides features to allow you to control video and audio players programmatically 

