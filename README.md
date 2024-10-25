# Photos from R Contributor Events

This repository stores original photos taken at R Contributor Events. 

## Rescaling/optimizing

As high-resolution photos, they should likely be rescaled and potentially 
optimized before use, e.g.

```r
library(magick)
img <- image_read("R Project Sprint 2023/IMG_4049.jpg")
scaled_img <- image_scale(img, geometry_size_pixels(width = 600))
opt_img <- image_resize(img, geometry_size_pixels(width = 600), 
                        filter = "Triangle")
image_write(scaled_img, "R Project Sprint 2023/IMG_4049_scaled.jpg")
image_write(opt_img, "R Project Sprint 2023/IMG_4049_opt.jpg")
```

`magick::image_chop` or `magick::image_crop` can also be used to select a 
subregion of the photo, though it may be easier to crop manually.

## Re-use

People in these photos have given their consent for these photos to be used in 
the following ways:

– In reports of the event (e.g. in R Journal News, R-devel GitHub, sponsor blog)
– On official social media channels (e.g. R Foundation/R Contributor accounts, 
sponsor accounts)
– On participants' social media (e.g. blog posts, Mastodon sharing their 
experience)

For other use, consent must be requested from the individuals pictured. An 
index is provided naming individuals for small group photos.