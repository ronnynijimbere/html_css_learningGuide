Adding Images
Images are added with the <img> element. This is a self-closing tag, which means you shouldn’t include an end tag.

When adding an image, include the following four properties:

    src - the file path to the image
    width - the width of the image in pixels
    height - the height of the image in pixels
    alt - alternative text to display if the image doesn’t load correctly

If the image is purely decorative and adds no meaning to the page, you can leave the alt text blank.
You can use images in many formats, but jpeg, png, and gif are the most common. Choose the type that will give you the best image quality with the lowest file size.
Images are block elements by default, but if you want to wrap text around an image, you can float the image to the left or the right

Adding Video
You can add video with the <video> element.
When adding video, make sure to add the src property with the path to the video file.
You can also add the following properties if you’d like:

    autoplay - add this (with no value) to automatically start playing the video when it loads
    controls - add this (with no value) to display the controls on the video (pause, play, etc.)
    loop - add this (with no value) to make the video play over and over again in a loop
    poster - add the source to an image that will be the cover of your video

Popular video formats are ogv and mp4.
This element is used for directly hosting videos on your site, but it may be better to host videos on YouTube or Vimeo and include them on your page. This will be covered in the section below called Adding Other Media.

Adding Audio
You can add audio with the <audio> element.
When adding audio, make sure to add the src property with the path to the audio file.

You can use many of the same attributes as video on an <audio> element:

    autoplay - add this (with no value) to automatically start playing the audio file when it loads
    controls - add this (with no value) to display the controls on the audio file (pause, play, etc.)
    loop - add this (with no value) to make the audio file play over and over again in a loop

Adding Other Media
Have you ever seen a YouTube video or Google Map embedded into a page?
You can add rich and interactive media onto your web page using something called inline frames.
These create a little frame that loads a new HTML page, allowing you to embed rich content from other websites.

You can find iframe codes for popular services like YouTube and Google Maps on each service’s website. They’re usually under a section called “Share” or “Embed.”
