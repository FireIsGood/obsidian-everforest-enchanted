# Custom Image Backgrounds

Custom image backgrounds are always fun! This extra style setting allows you to set an external or local background image.

There are some limitations made for the sake of performance. Image filters are not included as they cause too much lag. It's recommended to use smaller image files that have been pre-blurred as to load faster.

Backgrounds are split into dark and light mode backgrounds, though advanced users can override both with `--background-image-url` in a snippet.

## Settings

Mostly self-explanatory.

- Enable Background Image: Enables the background image
- Dark Mode Background URL: The dark mode background image url
- Light Mode Background URL: The light mode background image url
- Background Position: Which direction the background image will start from
- Pane Opacity: How opaque the page backgrounds are
- UI Opacity: How opaque the UI backgrounds are
- Tab Opacity: How opaque the **STACKED TABS** headers are

## External Images

Simply type in the url text as a link to any image file. Some good sources might be [Pexels](https://www.pexels.com/) or [Unsplash](https://unsplash.com/). After that, place the URL within the quotes of the url function `url()`. Simply drag the image preview to a new tab and remove text after the question mark `?` to get the shortest link.

You can use extra parameters in the url of these two sites to get smaller images. Just replace all the content after the question mark `?` if there is any or just add in the string with `?w=1920&q=80` for a width of 1920 pixels and a quality of 80. You can lower the width or quality to make it load faster.

### Examples

Image we want:

> ![Green Tree](https://images.pexels.com/photos/268533/pexels-photo-268533.jpeg?w=1920&q=80)  
> _Photo by Pixabay from Pexels: <https://www.pexels.com/photo/green-tree-268533/>_

We would use the following link:

<https://images.pexels.com/photos/268533/pexels-photo-268533.jpeg?w=1920&q=80>

And place it in the URL function:

```css
url("https://images.pexels.com/photos/268533/pexels-photo-268533.jpeg?w=1920&q=80")
```

Turns into:

![Theme dark with an image background](asssets/theme%20dark%20image.png)

---

Image we want:

> ![Selective Focus Photography of White Petaled Flower Plant](https://images.pexels.com/photos/997567/pexels-photo-997567.jpeg?w=1920&q=80)  
> _Photo by Alissa Nabiullina from Pexels: <https://www.pexels.com/photo/selective-focus-photography-of-white-petaled-flower-plant-997567/>_

We would use the following link:

<https://images.pexels.com/photos/997567/pexels-photo-997567.jpeg?w=1920&q=80>

And place it in the URL function:

```css
url("https://images.pexels.com/photos/997567/pexels-photo-997567.jpeg?w=1920&q=80")
```

Turns into:

![Theme light with an image background](asssets/theme%20light%20image.png)

## Local Images

Local images are a bit harder and you'll need to know how to create and use snippets due to security changes in 1.3 with how Obsidian allows file system access.

You can leave the Style Settings variables alone when using local images since snippets are always higher priority than style settings.

Using large local images **can cause lag**. If you're having issues, you can try using smaller images sizes and formats like avif. You may also want to just use one image for both modes so you aren't loading extra images for no reason.

If you want **different images** for both dark and light modes, you should use the following template:

<!-- prettier-ignore-start -->
```css
:root body.theme-dark {
  --background-image-url: url("");
}
:root body.theme-light {
  --background-image-url: url("");
}
```
<!-- prettier-ignore-end -->

If you want the **same image** for both modes, you should use the following template:

<!-- prettier-ignore-start -->
```css
:root body {
  --background-image-url: url("");
}
```
<!-- prettier-ignore-end -->

Now, you have to get yourself a [data URI](https://css-tricks.com/data-uris/) inside the quotation marks. Since the base64 text is really large and annoying to go back and edit, I would recommend resizing or doing any editing to the image to make it the size you want before the next step. If you don't care about the background being blurred, you could reduce the resolution down to a width of 960px and convert to the AVIF file format. I found [an online converter](https://avif.io/) that works in your browser for this.

Resizing and converting from a 1920x1080 PNG at 2.38 megabytes file to a 960x520 AVIF file at 56 kilobytes, a ~97% reduction! I personally use a high opacity and blurred background to increase legibility, so this was a worthwhile change.

To get a data URI, you will have to encode your image into base64. An easy online converter I found was [a github repo by jpillora](https://jpillora.com/base64-encoder/). Drag your file in, copy the text box, and paste the text inside the quotation marks on the corresponding url function.
