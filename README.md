## Laravel API

<h3>Installation/Guide
-   cd (project directory)
-   run <code>composer install</code>
-   run <code>npm install && npm run dev for auth routes.</code>
<h3>Database Seeders</h3>
-   This project contains seeders for both Users and Posts tables.
-   run <code>php artisan migrate:fresh --seed</code> to get started with some fresh data

<h3>Endpoints</h3>
-   GET /api/posts/
-   A GET request to this URI endpoint retrieves all posts
-   POST /api/posts/
-   A POST request to URI creates a post (a random user_id will be generated with the created post for testing purposes)
-   PUT /api/posts/
-   A PUT reques to this URI will update the post.
-   Note: Please include a "post_id": $post->id to the JSON object along with title and description when making this request.
-   DELETE /api/posts/{resource_id}
-   A DELETE request to this endpoint will delete the given resource.

## Eloquent ORM Relationships

-   As mentioned above the app comes with Database Seeders for testing purposes
-   run <code>php artisan tinker</code>
-   run <code>\$user = App\Models\User::find(1);</code>
-   run <code>\$user->posts</code> (This should return all posts for that user)

-   run <code>\$post = App\Models\Post::find(5);</code>
-   Run <code>\$post->user</code> (This returns the user associated with that post).

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
