# PHP POS Print (Local Server)

**A [php](http://php.net/) application for printing POS receipts**


### Installation

To clone and run this repository you'll need
[git](https://git-scm.com),
[php](http://php.net/) &
[composer](https://getcomposer.org/).

From your command line:

```bash

# Clone this repository
git clone https://github.com/Tecdiary/ppp

# Go into the repository
cd ppp

# Install dependencies
composer install

# Start server from command line
php index.php

# Start app for settings
php -S localhost:8000 -t app/
```

Next time you can simply run `php index.php` in command line OR `server.sh` file to start the server.

This app runs at port 6441 ( ws://lcoalhost:6441 ) and listen for the print jobs.

### Local printers
Server will try to use the local printers if no printer has been provided.
You can access local app from your local web server url or just run `php -S localhost:8000 -t app/` and access the app in browser http://localhost:8000

**App Features**
- Main index page `index.php` to update your default printers
- Printers page `printers.php` to list all your printers
- Add Printer page `add_printer.php` to add new printer

The local settings will be saved in `dataabse/data.json` file.

**Screenshots**

Index page
![Index](app/images/default.png)

Printers page
![Printers](app/images/printers.png)

Add printer page
![Add Printer](app/images/add_printer.png)
