# Audio, Video, Images

- Supporting audio formats in HTML

There are three formats that are supported: 

1. MP3 which is Audio format from MPEG (Moving/Motion Pictures Experts Group)

2. AAC which is Advanced Audio Coding

3. OGG which is An Open container and free audio format

- Supported file formats for video tag:
There are three supported video formats in HTML: MP4, WebM, and OGG.

There are a number of other features you can include when displaying an HTML video. Take a look at our next example:

               <video controls width="400" height="400"
                         autoplay loop muted preload="auto"
                          poster="poster.png">
                            <source src="rabbit320.mp4" type="video/mp4">
                            <source src="rabbit320.webm" type="video/webm">
                  <p>Your browser doesn't support HTML video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
                 </video>

The new features are:

1. width and height : You can control the video size either with these attributes or with CSS. In both cases, videos maintain their native width-height ratio — known as the aspect ratio. If the aspect ratio is not maintained by the sizes you set, the video will grow to fill the space horizontally, and the unfilled space will just be given a solid background color by default.
2. autoplay : Makes the audio or video start playing right away, while the rest of the page is loading. You are advised not to use autoplaying video (or audio) on your sites, because users can find it really annoying.
3. loop : Makes the video (or audio) start playing again whenever it finishes. This can also be annoying, so only use if really necessary.
4. muted : Causes the media to play with the sound turned off by default.
5. poster : The URL of an image which will be displayed before the video is played. It is intended to be used for a splash screen or advertising screen.
6. preload : Used for buffering large files; it can take one of three values:

"none" does not buffer the file
"auto" buffers the media file
"metadata" buffers only the metadata for the file.

The`<audio>` element works just like the `<video>` element, with a few small differences as outlined below. A typical example might look like so:

           <audio controls>
                 <source src="viper.mp3" type="audio/mp3">
                  <source src="viper.ogg" type="audio/ogg">
                  <p>Your browser doesn't support HTML5 audio. Here is a <a href="viper.mp3">link to the audio</a> nstead.</p>
            </audio>


if u want to learn how to do this exactly vist [ this page](https://www.google.jo/url?sa=i&url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DLGL-ggEzECc&psig=AOvVaw058zoDc8h0c07k_rLofFnI&ust=1628464132131000&source=images&cd=vfe&ved=0CAsQjhxqFwoTCMDD7OuDoPICFQAAAAAdAAAAABAD) is a gold resource.
