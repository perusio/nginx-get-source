# Shell Script for Safely Downloadind a New Nginx release

## Introduction

This is a small shell script that downloads a new
[Nginx](http://nginx.org) release from the
[downloads page](http://nginx.org/download) together with its GPG
signature and verifies that the source is **correctly** signed.

Thus giving you some degree of confidence on the download sources.

You must **always inspect** the result of the signature verification
**yourself**.

## Installation and Usage

Just put the script somewhere and invoke it like this:
    
    nginx_get_src <nginx version>
    
For example, for downloading the 1.1.8 version and verify its
signature do:
    
    nginx_get_src 1.1.8
    
Note that if the signature verification **fails** the script exits with 1.
