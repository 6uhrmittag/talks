# Tasks either via gitpich or reveal-md.

- [View SMB_CIFS on gitpitch.com](https://gitpitch.com/6uhrmittag/talks/master?grs=github&t=beige&p=SMB_CIFS)

# reveal-md setup
[https://github.com/webpro/reveal-md](https://github.com/webpro/reveal-md)

````cmd
npm install -g reveal-md
````

# usage
````cmd
cd talk-directory
reveal-md PITCHME.md -w
````


# setup slides

## reveal options

1. place _reveal.json_ inside talk-directory
2. see [https://github.com/hakimel/reveal.js#configuration](https://github.com/hakimel/reveal.js#configuration)

````json
{
  "controls": true,
  "progress": true,
  "controls": true,
  "slideNumber": true
}
````
