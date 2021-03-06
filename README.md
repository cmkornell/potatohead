potatohead
==========

Template View Machine

<p> Potatohead is a simple node app that spawns a BB Frontend and displays configuration for it</p>

<h2> Concepts </h2>
* Decoupled from Frontend server
* Uses an "adapter" to communicate with external frontend
* Uses build tools (Gulp) for easy customization to the UI

<h2> Requirements </h2>
* Potatohead requires to be in the same directory as the frontend server 
* Frontend server must have middleware (lib/template-queries) that facilitates communication between the two apps
* Frontend server must use the aforementioned middleware in server.js (frontend 1)


<h2> Server configuration </h2>
* Potatohead runs on port 2000 (IP/DNS should be configured to this port)
* Modified frontend runs on port 3008
* Potatohead can take a command line argument to specify the frontend server address
<code> gulp -s http://localhost:3008</code>

<h2> Startup </h2>
<em> note: Potatohead's adapters will spawn and automate the Frontend it consumes </em>
* <b> Production </b> To start Potatohead <code>cd</code> into main directory and run <code> gulp server </code>
* <b> Development </b> When developing in Potatohead use <code> gulp </code> to run all dev tools

<h2> Writing a new adapter </h2>
<i>coming soon</i>
