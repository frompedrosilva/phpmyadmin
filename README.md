<h1 align="center">URL Redirect Script</h1>

<p align="center">
  <strong>A lightweight JavaScript-based redirect system designed for simple and efficient URL routing.</strong>
</p>

<p align="center">
  Automatically redirecting users to configured destinations through a minimal and dependency-free implementation.
</p>

<hr>

<h2>Overview</h2>

<p>
  URL Redirect Script is a lightweight web utility designed to automatically redirect users from one entry point to a configured destination URL.
</p>

<p>
  The project uses a simple JavaScript-based routing mechanism combined with Apache configuration support, providing a fast and efficient solution for managing redirects.
</p>

<p>
  The system can be extended to support multiple destinations, random routing, traffic distribution, landing page redirection, and temporary URL forwarding scenarios.
</p>

<hr>

<h2>Why This Project?</h2>

<p>
  Simple redirect systems are useful for managing traffic flows, temporary destinations, and controlled access points without requiring a complete backend application.
</p>

<p>
  This project focuses on keeping the implementation lightweight, fast, and easy to deploy on standard web hosting environments.
</p>

<hr>

<h2>Features</h2>

<ul>
  <li>🔗 Automatic URL redirection</li>
  <li>⚡ Instant browser-based execution</li>
  <li>🎲 Random destination selection support</li>
  <li>📦 No external dependencies required</li>
  <li>🛠️ Simple URL configuration</li>
  <li>🌐 Compatible with Apache hosting environments</li>
  <li>🚀 Lightweight and fast execution</li>
  <li>📁 Organized project structure</li>
</ul>

<hr>

<h2>Tech Stack</h2>

<p>
  <img src="https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?logo=javascript&logoColor=black">
  <img src="https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/Apache-D22128?logo=apache&logoColor=white">
</p>

<h3>Frontend</h3>

<ul>
  <li>JavaScript</li>
  <li>HTML5</li>
</ul>

<h3>Server Configuration</h3>

<ul>
  <li>Apache</li>
  <li><code>.htaccess</code></li>
</ul>

<hr>

<h2>Architecture</h2>

<pre>
User Browser
      ↓
Apache Server
      ↓
.htaccess Configuration
      ↓
index.html
      ↓
JavaScript Redirect Logic
      ↓
Destination URL
</pre>

<hr>

<h2>Project Structure</h2>

<pre>
phpmyadmin/
│
├── error/
│   └── Error handling pages
│
├── modules/
│   └── Additional scripts and resources
│
├── .htaccess
└── index.html
</pre>

<hr>

<h2>Core Functionality</h2>

<p>
  The application is built around a simple redirect workflow:
</p>

<ul>
  <li>Loads the main entry page.</li>
  <li>Initializes the JavaScript redirect logic.</li>
  <li>Selects a configured destination URL.</li>
  <li>Automatically forwards the user.</li>
</ul>

<hr>

<h2>How It Works</h2>

<p>
  The redirect system stores available destinations inside a JavaScript array:
</p>

<pre>
var urls = new Array();

urls[0] = "https://example.com/";
</pre>

<p>
  A random index is generated and the browser is redirected automatically:
</p>

<pre>
var random = Math.floor(Math.random()*urls.length);

window.location = urls[random];
</pre>

<hr>

<h2>Technical Challenges</h2>

<p>
  Building this project involved several considerations:
</p>

<ul>
  <li>Creating a lightweight redirect mechanism without backend dependencies.</li>
  <li>Ensuring fast execution during page loading.</li>
  <li>Maintaining compatibility with standard web hosting environments.</li>
  <li>Structuring the project for future expansion.</li>
  <li>Supporting flexible destination management.</li>
</ul>

<hr>

<h2>Installation</h2>

<p>Clone the repository:</p>

<pre>
git clone https://github.com/frompedrosilva/phpmyadmin.git
</pre>

<p>Navigate to the project directory:</p>

<pre>
cd phpmyadmin
</pre>

<p>
  Upload the project files to an Apache-compatible web server.
</p>

<p>
  Access the project through your browser:
</p>

<pre>
https://your-domain.com
</pre>

<hr>

<h2>Configuration</h2>

<p>
  Update the destination URLs inside <code>index.html</code>:
</p>

<pre>
var urls = new Array();

urls[0] = "https://your-destination-url.com/";
</pre>

<p>
  Multiple destinations can be added:
</p>

<pre>
urls[0] = "https://example-one.com/";
urls[1] = "https://example-two.com/";
urls[2] = "https://example-three.com/";
</pre>

<p>
  The system will automatically select one destination.
</p>

<hr>

<h2>Use Cases</h2>

<ul>
  <li>Landing page redirects</li>
  <li>Temporary URL forwarding</li>
  <li>Traffic distribution</li>
  <li>Multiple destination routing</li>
  <li>Quick deployment redirects</li>
</ul>

<hr>

<h2>Screenshots</h2>

<p>
  🚧 Screenshots and interface previews will be added soon.
</p>

<hr>

<h2>Roadmap</h2>

<ul>
  <li>✅ Basic redirect functionality</li>
  <li>✅ Multi-URL support</li>
  <li>✅ Apache compatibility</li>
  <li>⬜ Redirect analytics</li>
  <li>⬜ Admin interface</li>
  <li>⬜ Weighted traffic distribution</li>
  <li>⬜ Redirect history tracking</li>
</ul>

<hr>

<h2>Future Improvements</h2>

<p>
  Planned improvements and future development include:
</p>

<ul>
  <li>Dashboard for URL management</li>
  <li>Redirect statistics</li>
  <li>Custom routing rules</li>
  <li>Advanced traffic distribution</li>
  <li>Improved logging system</li>
</ul>

<hr>

<h2>Vision</h2>

<p>
  This project aims to provide a simple and reliable redirect solution focused on speed, simplicity, and easy deployment.
</p>

<p>
  Built with minimal technologies, it demonstrates how small utilities can solve practical web infrastructure problems efficiently.
</p>

<hr>

<h2>Live Demo</h2>

<p>
  🚧 A public demo will be available soon.
</p>

<hr>

<h2>Contributing</h2>

<p>
  Contributions, suggestions, and feedback are welcome.
</p>

<p>
  If you would like to contribute:
</p>

<ol>
  <li>Fork the repository.</li>
  <li>Create a feature branch.</li>
  <li>Commit your changes.</li>
  <li>Open a pull request.</li>
</ol>

<hr>

<h2>Author</h2>

<p>
  <strong>Pedro Silva</strong>
</p>

<p>
  Software Engineer · Full-Stack Developer
</p>

<p>
  🌐 Website:
  <a href="https://frompedrosilva.nl">
    frompedrosilva.nl
  </a>
</p>

<p>
  📧 Email:
  <a href="mailto:hello@frompedrosilva.nl">
    hello@frompedrosilva.nl
  </a>
</p>

<hr>

<h2>License</h2>

<p>
  This project is open-source and available for personal and educational use.
</p>
