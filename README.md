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

Optionally, you can configure CORS on a per-controller basis in CodeIgniter. To do this, create a custom MY_Controller.php in your application/core directory. Ensure that your other controllers extend MY_Controller.

Here's an example of a custom MY_Controller.php:



<?php
class MY_Controller extends CI_Controller {
    public function __construct() {
        parent::__construct();
        header('Access-Control-Allow-Origin: *');
        header('Access-Control-Allow-Methods: POST, GET, OPTIONS, PUT, DELETE');
        header('Access-Control-Allow-Headers: Content-Type, Content-Range, Content-Disposition, Content-Description');
        header('Access-Control-Allow-Credentials: true');
    }
}
