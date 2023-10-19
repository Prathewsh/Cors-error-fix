# Fixing CORS Issues in CodeIgniter

A step-by-step guide on resolving CORS (Cross-Origin Resource Sharing) errors in a CodeIgniter PHP application.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Instructions](#instructions)
  - [Enable CORS in .htaccess](#enable-cors-in-htaccess)
  - [Configure CodeIgniter](#configure-codeigniter)
  - [Testing](#testing)
- [Contributing](#contributing)
- [License](#license)

## Introduction

CORS (Cross-Origin Resource Sharing) errors occur when a web application tries to make requests to a different domain than the one that served the web page. This repository provides a solution for fixing CORS issues in a CodeIgniter PHP application.

## Prerequisites

- A CodeIgniter PHP application.
- Access to the `.htaccess` file for configuring the server.

## Instructions

### Enable CORS in .htaccess

1. Open your `.htaccess` file in your CodeIgniter project.

2. Add the following CORS rules at the top of your `.htaccess` file to enable cross-origin requests:
