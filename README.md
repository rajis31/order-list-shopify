<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

## Introduction
This app will allow users to create custom order statuses and send out email notifications during various stages of the account order.  This is my first shopify app and I'm pretty excited to get this started 

## Project Setup 

    - I will be using MAC OS for this.  
    - Install Composer, Valet (Optional) and npm
    - Run `composer create-project laravel/laravel proj_name` 
    - Run `composer require laravel/ui`
    - Run `php artisan ui vue`
    - Run `npm install`
    - Run `composer require osiset/laravel-shopify`  # This connects your app to your shopify store
    - Run `php artisan vendor:publish --tag=shopify-config` # Creates shopify config file 
    - Create a new public app on the shopify partner store 
    - Also make sure that you have created a store with the app installed
    - Add SHOPIFY_API_VERSION=2021-01       
          SHOPIFY_API_KEY=
          SHOPIFY_API_SECRET=
          to your .env file 
    - Visit https://github.com/osiset/laravel-shopify/wiki/Installation to find out more information
      on setting up the plugin to work with your shopfiy store 
    - Run `valet park` if you are on a MAC 
    - Run `valet link <link name>` which will link your project to run in the background 
    - Run `valet <link name> secure` to have your app run with https connection
    - Finally run `php artisan vendor:publish --tag=shopify-migrations && php artisan migrate`
    - Note - In your app settings on shopify use https://link_name.test and https:link_name.test/authenticate for both the APP URL & APP REDIRECT 
    - You should now see your app rendered in your shopify app store 

