# PHP/Xdebug/Docker example

Thi is an example intial repo for debuging PHP with Xdebug inside Docker. Using VS Code.

## Usage

The Nginx, Dockerfile, docker-compose.yml and xbebug.ini are a start point for developing php web applications locally. 

You should modified these files to your need and I do not advice using these sample files into production.

 To run everything you must run the following command (positioned in the same folder as yout docker-compose.yml file):
 
``docker-compose -p <desired-name> up -d``.

## VS Code configuration

Install the [felixfbecker.php-debug](https://marketplace.visualstudio.com/items?itemName=felixfbecker.php-debug) extension.

You can create a debug configuration by going to `Debug > Add Configuration... > PHP`, but configuration file is included in  `.vscode/launch.json` file in the repo, with the correct folder maping.

Add a breakpoint, and click on "Listen for XDebug" in the top left hand corner. Load your page, and you should get debugging information:

![](https://i.imgur.com/B8dnAj7.png)

Credits to [Sajjad Ashraf](https://github.com/sajjad26)
