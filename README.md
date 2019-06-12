# fullstack
A full stack base template for using Laravel with VueJS. Typescript, SCSS, Babel, ESLINT, Jest, and PHPUnit included.

# Stack

### Server
Utilizes the [Laravel](https://laravel.com/) PHP framework to handle server functionality providing an out of the box MVC framework.

With this repository, the easiest way to get up and running fast is by using [Laravel Valet](https://laravel.com/docs/5.8/valet) to handle PHP execution.

However, it can easily be configured to be served through a Vagrant environment or Docker container as well.

### Client

The client side is handled with [Vue.JS](https://github.com/vuejs/vue) and is completely separated from the server side Laravel application.  Requests from the front end are sent via proxy (configured in the vue.config.js file) to the server side.  This means you can work on the front end and back end independently allowing for a true separation of concerns in this fullstack environment.

### Niceties

Testing ready.  PHPUnit and Jest are included out of the box.

No more Laravel Mix.  Run the serve script inside of the front end and you will be utilizing Webpack out of the box.  Waiting for laravel mix to compile is a thing of the past.

Configure to your liking.  This is just a base template that I like. If you want to change anything about it, you are welcome and encouraged to do it.

# **Utilization**
1. `Clone this repo`
2. Run this command from project root: `composer install && cd frontend && npm install && npm run serve`
3. You should now have a front end being served on localhost.


#### Watch out.

If Laravel Valet is misconfigured or the devServer.proxy in your vue.config.js file is not pointed to the right domain the Laravel application cannot interpret requests coming from the front end.  Make sure that Valet is configured correctly.
