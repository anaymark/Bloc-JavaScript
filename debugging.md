# Open your browser. Open up the Chrome DevTools. Click on the Network tab on the DevTools. Go to your bloc roadmap page. What Request Url is being used to get your information from the API?

* https://www.bloc.io/users/alexander-sydorenko/checkpoints

# Where can I find the cookies being used on the webpage using the Chrome DevTools?

* The cookies being used on the webpage are under the Application tab in the storage divider.

# Where can you execute JavaScript in the DevTools?

* JavaScript can be executed in the Console and in the js documents under the Sources tab.


# How can you modify existing CSS on your webpage using the Dev Tools?
What happens to code you have modified through the DevTools, when you refresh the page?

* CSS elements can be modified from the elements tab using the Styles tab.

# What are the different ways you can add breakpoints to your JavaScript for debugging?

1.) Use chrome dev tools or firebug to locate the source and the line of JavaScript. 
	* Select the Sources tab in Dev Tools
	* Find the JS source doc you want to edit
	* Find the line in the doc you want to add the breakpoint
	* Click the line number and a little blue highlighted triangle will appear
	* When the breakpoint is fired, you can use the Watch Tab next to Scope where you can run arbitrary expressions, see all variables in the scope, and the call stack.

2.) Use the **debugger** statement
	* debugger; - this will fire every time. If a complex JS file exists that is difficult to navigate into, use 
	* Conditional breakpoint firing can be used as well for times that if/when/while a set condition occurs, the breakpoint will fire.

3.) Use WebStorm JavaScript IDE
	* Will use Firefox or Chrome plug-in and must be configured to map JavaScript on the dev server to JavaScript files in your enviroment. 

4.) Stack Tracing may be useful as well for minor debugging of relatively 
simple code.

