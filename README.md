# bs2grproxy
Automatically exported from code.google.com/p/bs2grproxy

#BS2GRProxy Introduction

Introduction
A small app runs on Google App Engine as a reverse proxy to a specific site.

Features
Reverse proxy
Web pages, css/js and media files can be redirected to different hosts
Configurable through Google App Database view
How to use
Download the source package
Modify app name in app.yaml
Upload the app
Enjoy
Configuration
You can set default config in bs2grpconfig.py. But how ever it's not encouraged to modify the source code unless you understand it.

After the first run on app engine, a data entry will be created in table "BS2GRPConfig". You can set run time options there using Data View in app admin page.

Options in BS2GRPConfig
target_host: HTML target url.

static_host: Static target url.

cssjs_redirect: Redirect css/js files to static host. Including: .css .js

media_redirect: Redirect media files to static host. Including: .jpg .jpeg .gif .png .avi .mov .mp3 .rm .rmvb .qt

Comment by amoiz.sh...@gmail.com, Mar 22, 2010
很有意义的项目，可以做个部署包么？ 方便我们这些不搞python的人.

Comment by lilel...@gmail.com, Dec 19, 2010
按照操作做了个反向代理希望，可以在墙内访问被墙的blogger，但访问http://lilelulu.appspot.com/ 时，提示 BS2Proxy Error: Requested host is not available. Please try again later.. 请高手相助～！ 多谢，邮件 lilelulu@gmail.com

Comment by chenyong...@gmail.com, Dec 19, 2010
(No comment was entered for this change.)
Comment by Symbia...@googlemail.com, Dec 27, 2010
http://mc2mirror.appspot.com/ BS2Proxy Error: Requested host is not available. Please try again later.. how do I fix this? Thanks

Comment by OzFal...@gmail.com, May 1, 2011
To fix error: BS2Proxy Error: Requested host is not available.

Adjust the host settings at the admin section. http://App-ID.appspot.com/_bs2admin/

Comment by yoursli...@gmail.com, Nov 19, 2011
速度怎么样啊？

Comment by freddyni...@gmail.com, Jan 19, 2012
Great work! Is the best reverse proxy to a specific site create in Google App Engine! :D

Thanks!!!

Comment by InstantW...@gmail.com, May 20, 2012
To change the proxy time out. In bs2grproxy.py, add the time out to the end like this: resp = urlfetch.fetch(new_path, self.request.body, method, newHeaders, False, False, 30)

