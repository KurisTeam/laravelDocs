## After installation
-So go to app/Providers/AppServiceProvider.php
-add this to the top of the class `use Illuminate\Support\Facades\Schema;`
-add this to the boot function `Schema::defaultstringLength(191);`
