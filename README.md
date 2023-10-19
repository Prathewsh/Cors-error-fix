# Fixing CORS Issues in CodeIgniter

A step-by-step guide on resolving CORS (Cross-Origin Resource Sharing) errors in a CodeIgniter PHP application.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Instructions](#instructions)
  - [Enable CORS in .htaccess](#enable-cors-in-htaccess)
  - [Configure CORS in controller](#configure-cors-in-controller)

## Introduction

CORS (Cross-Origin Resource Sharing) errors occur when a web application tries to make requests to a different domain than the one that served the web page. This repository provides a solution for fixing CORS issues in a CodeIgniter PHP application.

## Prerequisites

- A CodeIgniter PHP application.
- Access to the `.htaccess` file for configuring the server.

## Instructions

### Enable CORS in .htaccess

1. Open your `.htaccess` file in your CodeIgniter project.

2. Add the CORS rules given in allowcors at the top of your `.htaccess` file to enable cross-origin requests


### Configure CORS in controller

1. Optionally, you can configure CORS on a per-controller basis in CodeIgniter. To do this, create a custom MY_Controller.php in your application/core directory. Ensure that your other controllers extend MY_Controller. Example given in allowcorsincontroller file
