# What is this image?

This image includes build tools like compass, grunt-cli, bower for customizing foundation framework with SCSS.
It is made with the install process described at [http://foundation.zurb.com/docs/sass.html](http://foundation.zurb.com/docs/sass.html).


## How to use this image

If you want to create new foundation project, you run the command as bellows. And, you'll get SCSS and so on under current directory.

```docker run -it --rm -u foundation -v `pwd`:/opt -w /opt uniqrn/foundation-docker foundation new MY_PROJECT```


Then, you can customize SCSS in MY_PROJECT.
If you want to compile SCSS into CSS, you can use ```compass``` command from this image.

```docker run -it --rm -u foundation -v `pwd`:/opt -w /opt uniqrn/foundation-docker /bin/bash```
```# compass watch```

