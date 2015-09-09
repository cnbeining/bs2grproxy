#BS2GRProxy Introduction

## Introduction ##

A small app runs on Google App Engine as a reverse proxy to a specific site.

## Features ##
  * Reverse proxy
  * Web pages, css/js and media files can be redirected to different hosts
  * Configurable through Google App Database view

## How to use ##
  1. Download the source package
  1. Modify app name in app.yaml
  1. Upload the app
  1. Enjoy

## Configuration ##
You can set default config in bs2grpconfig.py. But how ever it's not encouraged to modify the source code unless you understand it.

After the first run on app engine, a data entry will be created in table "BS2GRPConfig". You can set run time options there using **Data View** in app admin page.

## Options in BS2GRPConfig ##
target\_host: HTML target url.

static\_host: Static target url.

cssjs\_redirect: Redirect css/js files to static host. Including: **.css .js**

media\_redirect: Redirect media files to static host. Including: **.jpg .jpeg .gif .png .avi .mov .mp3 .rm .rmvb .qt**
