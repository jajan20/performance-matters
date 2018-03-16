## Performance Matters

### About
In this assignment for performance matters we were tasked with optimizing the bootstrap webpage.

### Results
!()[]

### Optimizations criteria
- [x] critical css
- [x] font loading
- [x] image optimization
- [x] aSync

### Other optimizations
- [x] minifyCSS
- [x] minifyJS
- [x] unCSS




### CSS
**Critical CSS:**
By analyzing what CSS is necessary with the initial load we can extract these lines and put them in our head tag inside HTML. This will make it feel the page renders faster because the user actually sees something almost right away. In the background data is still being loaded.

**unCSS:** 
The app uses a couple of libraries and not everything is used. With unCSS we can analyze the remaining CSS and see what isn’t used and then remove this from our code.

**aSync:** 
With loading CSS asynchronous the initial render shows plain HTML. Combining this with critical CSS the user sees a styled page, with a lot of styling being downloaded in the background.

### Images
There are a couple of ways you can optimize images. I choose to compress them so that every browser can load them. Other ways you can speed up loading times is by using new image formats like JPEG XR and WebP. These aren't supported by all browsers/devices.

### Font loading
Bootstrap uses custom fonts, this will block the rendering of the page while it's being loaded. With 

``` css
font-display: swap
```
We can tell the browser to first load regular font that are present on the user’s computer. When the customs are done loading everything gets "swapped".

### JavaScript
By minifying JavaScript (putting everything on one line, removing whitespace) the computer can actually read everything faster. This way loading times are sped up.



