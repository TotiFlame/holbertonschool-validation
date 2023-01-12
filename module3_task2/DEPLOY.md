# DEPLOY.md
## What is in the archive and how to unarchive it?
An archive is a single file that contains one or more other files, as well 
as metadata about those files. Archives are used to package and distribute 
large collections of files or to compress large files to save space. Some 
common formats for archives include ZIP, RAR, and TAR.
## What are the commands to start and stop the application?
The commands depend on how was biult the application, in this case this 
is the command to start: /awesome-api, to stop the application ctrl + c.
## How to customize where the application logs are written?
The process for customizing where an application's logs are written will 
depend on the specific application. However, many applications allow you 
to specify a custom log file location through a configuration file or command 
line option.
## How to “quickly” verify that the application is running (healthcheck)?
You can quickly verify with curl "http://localhost:8000/health"