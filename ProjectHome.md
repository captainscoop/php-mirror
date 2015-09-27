php-mirror is a PHP-based download mirror script.  It requires no installation and runs from your server immediately after downloading it.  It's a 1 file program that has the ability to:
  * Download files
  * Give out the md5 checksum
  * Show a "thank you" page
  * Create projects
  * Manage files
  * Use short (4 character) URLs (can be set on a project by project basis).
  * Compress a file on the fly

php-mirror is free so give it a try - no database required! php-mirror can also be used to create a powerful downloads server and can easily be modified to be accessed on a subdomain (eg: mirror.example.com).

php-mirror relies on an aphabetical folder structure that is similar to below.

/mirror.php
> a/
> > android/
> > > android-0.6.iso
> > > > php-mirror.xml

It uses an XML file (php-mirror.xml) in each projects folder to give information about the project.  This can include links to websites, authors and short descriptions. Information about each projects disk usage, number of downloads, etc is also recorded.

3 pages can be managed using php-mirror - the index page, error page and thank you/downloading page.  On each page dynamic information can be displayed.  This includes md5 check sums, file size, project information and more.  On any page a search box can also be used.

php-mirror has the ability to search projects and downloads for a certain term.  This is done without the need for a database, however for very large download sites/mirrors (3 TB+) customization is recommended so that a database is used.

php-mirror can also edit a download on each request.  This can include "zipping" (creating a ZIP file) of the requested file as well as editing the name of a file.

Features such as "zipping" are set on a per-basis in the web-based control panel.  This control panel allows uploads, management of projects and downloads, viewing of statistics, the design of some pages and the backing up or mirroring of the php-mirror.

To make it easy for URLs to be remembered, short URLs that are similar to http://tr.im/ and http://tinyurl.com/ can be used.  This means that instead of a user entering the following: `http://example.com/mirror.php?a=dl&p=android&f=android-0.6.iso`, the user can enter: `http://example.com/mirror.php?k=7y9T`.

**php-mirror is coming soon.**

_Note:  The [Android Project](http://code.google.com/android/) is used as an example.  It has NO connection with php-mirror._