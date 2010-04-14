PyNotify
========

A python based super simplified notification system. This project is designed to give basic notification capabilities with minimal requirements.

## Requirements

	* Python (Only tested with 2.4, others may work)
	* GTK+ >= 2.x
	* PyGTK >= 2.10
	
## Usage

### Server

By default the server runs on port 2199. Start the server by running `./notify_daemon`
	
### Send messages

To send a notification run `./notify <message to display>`

### Scripting

This program can be used to alert you when a command completes. You can even have different messages for success and failure. 

Create an alias like the following:

	alias all_done="./notify Operation Successful Message || ./notify Operation Failed Message"
	
Now you can run a long command and add this to the and to get feedback when it is done.

	command_that_takes_a_while && alldone
	
## Issues

Please report any bugs to the [issue tracker][1]

[1]: <http://github.com/sionide21/PyNotify/issues> "Issue Tracker".