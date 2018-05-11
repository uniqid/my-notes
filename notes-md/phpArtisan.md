# Laravel Framework 5.5.40

Usage:
  command [options] [arguments]

### Options:
	-h, --help            Display this help message
	-q, --quiet           Do not output any message
	-V, --version         Display this application version
	    --ansi            Force ANSI output
	    --no-ansi         Disable ANSI output
	-n, --no-interaction  Do not ask any interactive question
	    --env[=ENV]       The environment the command should run under
	-v|vv|vvv, --verbose  Increase the verbosity of messages: 1 for normal output, 2 for more verbose output and 3 for debug

### Available commands:
	  list                 Lists commands
	  help                 Displays help for a command
	  serve                Serve the application on the PHP development server
	  clear-compiled       Remove the compiled class file
	  down                 Put the application into maintenance mode
	  up                   Bring the application out of maintenance mode
	  env                  Display the current framework environment
	  migrate              Run the database migrations
	  preset               Swap the front-end scaffolding for the application
	  tinker               Interact with your application
	  inspire              Display an inspiring quote
	  optimize             Optimize the framework for better performance (deprecated)

	 app
	  app:name             Set the application namespace

	 auth
	  auth:clear-resets    Flush expired password reset tokens

	 cache
	  cache:clear          Flush the application cache
	  cache:forget         Remove an item from the cache
	  cache:table          Create a migration for the cache database table

	 config
	  config:cache         Create a cache file for faster configuration loading
	  config:clear         Remove the configuration cache file

	 db
	  db:seed              Seed the database with records

	 debugbar
	  debugbar:clear       Clear the Debugbar Storage

	 event
	  event:generate       Generate the missing events and listeners based on registration

	 key
	  key:generate         Set the application key

	 make
	  make:auth            Scaffold basic login and registration views and routes
	  make:command         Create a new Artisan command
	  make:controller      Create a new controller class
	  make:event           Create a new event class
	  make:exception       Create a new custom exception class
	  make:factory         Create a new model factory
	  make:job             Create a new job class
	  make:listener        Create a new event listener class
	  make:mail            Create a new email class
	  make:middleware      Create a new middleware class
	  make:migration       Create a new migration file
	  make:model           Create a new Eloquent model class
	  make:notification    Create a new notification class
	  make:policy          Create a new policy class
	  make:provider        Create a new service provider class
	  make:request         Create a new form request class
	  make:resource        Create a new resource
	  make:rule            Create a new validation rule
	  make:seeder          Create a new seeder class
	  make:test            Create a new test class

	 migrate
	  migrate:install      Create the migration repository
	  migrate:fresh        Drop all tables and re-run all migrations
	  migrate:refresh      Reset and re-run all migrations
	  migrate:reset        Rollback all database migrations
	  migrate:rollback     Rollback the last database migration
	  migrate:status       Show the status of each migration

	 notifications
	  notifications:table  Create a migration for the notifications table

	 package
	  package:discover     Rebuild the cached package manifest

	 queue
	  queue:work           Start processing jobs on the queue as a daemon
	  queue:failed         List all of the failed queue jobs
	  queue:flush          Flush all of the failed queue jobs
	  queue:forget         Delete a failed queue job
	  queue:listen         Listen to a given queue
	  queue:restart        Restart queue worker daemons after their current job
	  queue:retry          Retry a failed queue job
	  queue:table          Create a migration for the queue jobs database table
	  queue:failed-table   Create a migration for the failed queue jobs database table

	 route
	  route:cache          Create a route cache file for faster route registration
	  route:clear          Remove the route cache file
	  route:list           List all registered routes

	 schedule
	  schedule:run         Run the scheduled commands

	 session
	  session:table        Create a migration for the session database table

	 storage
	  storage:link         Create a symbolic link from "public/storage" to "storage/app/public"

	 vendor
	  vendor:publish       Publish any publishable assets from vendor packages

	 view
	  view:clear           Clear all compiled view files
