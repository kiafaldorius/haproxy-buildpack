# haproxy-buildpack

This is a Heroku buildpack for haproxy.

You can specify the haproxy version by putting the full link in the VERSION file.

You must have a haproxy.cfg file in your app's root.

## Why?

Why would anyone want haproxy on Heroku when it has a perfectly good load balancer and its own routing mesh?

If you're here, you were probably searching for a haproxy buildpack anyway, so you know why you want/need it.

For those who wandered here through their escape from spiders and/or adventures with robotic bretheren, you may consider the following:

You have an AwesomeApp at www.example.com and AwesomeApp has an API at api.example.com, but for whatever reason you also need to provide it at www.example.com/api/. HaProxy can help here.

# Usage

This buildpack compiles and generates a haproxy binary in your app's root directory.

You are encouraged to fork this repository and edit it to your needs (particularly the VERSION file that points to the haproxy archive that you want to compile/install). You should then use the link to your fork and changes as the BUILDPACK_URL on heroku rather than this one. (It's for your own good; I'm not liable for any changes that I may make to this repository in the future.)
