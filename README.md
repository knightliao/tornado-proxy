## Asynchronous HTTP proxy with tunnelling support

Built using Tornado Latest Version, supports HTTP GET, POST and
CONNECT methods.

Can be used as standalone script, or integrated with your Tornado app.

And I will maintenance this project.


### Setup

    # run self tests
    python setup.py test

    # install it
    python setup.py install

### Command-line usage

    python tornado_proxy/proxy.py 8888
    
if you want to see tornado debug log:

    python tornado_proxy/proxy.py 8888 --logging=debug


### Module usage

    from tornado_proxy import run_proxy
    run_proxy(port, start_ioloop=False)
    ...
    tornado.ioloop.IOLoop.instance().start()


