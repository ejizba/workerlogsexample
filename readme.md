# Worker logs in app insights

This app is meant to help reproduce the problem where worker system logs are not showing up in app insights. These show up in core tools and the kusto FunctionsLogs table, just not app insights. It has one warning and one error you can reproduce.

The first is a warning that happens when the app starts up:

> [2023-04-20T23:34:24.356Z] Worker was unable to load entry point "index.js": example failed entry point

The second is an error that happens when you execute the HttpTrigger1 function

> [2023-04-20T23:34:30.672Z] Error: Choose either to return a promise or call 'done'. Do not use both in your script. Learn more: https://go.microsoft.com/fwlink/?linkid=2097909
