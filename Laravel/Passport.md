## Create a Resource
- So go to `php artisan make:resource ProjectResource`
- This will create a folder in the `app` directory called Resources and also a file `ProjectResource.php` inside the resources

## JSON Responses
- The first piece needed is the `ForceJsonResponse` middleware, which will convert all responses to JSON automatically.
- To do this, run: `php artisan make:middleware ForceJsonResponse`
- And this is the handle function of that middleware, in `App/Http/Middleware/ForceJsonReponse.php`
- `public function handle($request, Closure $next){$request->headers->set('Accept', 'application/json');return $next($request);}`
- Next, we’ll add the middleware to our `app/Http/Kernel.php` file in the `$routeMiddleware` array:
- `'json.response' => \App\Http\Middleware\ForceJsonResponse::class,`
- Then, we’ll also add it to the `$middleware` array in the same file:
- `\App\Http\Middleware\ForceJsonResponse::class,`
- That would make sure that the `ForceJsonResponse` middleware is run on every request.

## CORS (Cross-origin Resource Sharing)
- To allow the consumers of our `Laravel REST API` to access it from a different origin, we have to set up CORS. To do that, we’ll create a piece of middleware called `Cors`.
- directory and run `php artisan make:middleware Cors`
- Then, in `app/Http/Middleware/Cors.php,` add the following code:
- `public function handle($request, Closure $next){
        return $next($request)
            ->header('Access-Control-Allow-Origin', '*')
            ->header('Access-Control-Allow-Methods', 'GET, POST, PUT, DELETE, OPTIONS')
            ->header('Access-Control-Allow-Headers', 'X-Requested-With, Content-Type, X-Token-Auth, Authorization');
    }`