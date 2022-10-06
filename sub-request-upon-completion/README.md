# Sub-Request Upon Completion
There are some cases that you want to pass the request to another backend in addition to and after serving it. One use case is to track the number of completed downloads by calling an API after user completed download a file. Another use case is for tracking request where you want to return as fast as possible (perhaps with an empty_gif) and then do the actual recording in background. The [post_action](http://wiki.nginx.org/HttpCoreModule#post_action) that allows you to define a sub-request that will be fired upon completion of the current request are [perfect solution](http://mailman.nginx.org/pipermail/nginx/2008-April/004524.html) for these use cases.