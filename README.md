# php-autoclassloader
This is an Automatic ClassFile Loader for PHP.

<h2>How To</h2>
<ol type="1">
    <li>Include "init.php" file in the project at the start.</li>
    <li>Put all your class files organized under "lib" directory in the server root.</li>
    <li>There you go!</li>
</ol type="1">

<p>Whenever a class is referenced throughout the PHP runtime environment, if the classFile is not yet included into the runtime, the system automatically calls the "spl-autoload-register" for the classFile. And this call is directed to the "lib" directory in the server root, and all the class files under the subdirectories are included into the project.</p>
<p>This is the preferred method for autoloading classes in PHP 7.2 onwards</p>