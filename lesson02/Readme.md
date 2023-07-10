<h1>Project Setup: Tailwind CSS</h1>
<h2>Lesson 02</h2>

<p>To set up Tailwind CSS for your project, please follow the instructions below:</p>

<h3>Step 1: Initialization</h3>
<p>Run the following command to initialize Tailwind CSS in your project:</p>
<pre><code>npx tailwindcss init</code></pre>
<p>This command creates a <code>tailwind.config.js</code> file in your project directory, allowing customization of the framework's settings according to your needs.</p>

<h3>Step 2: Configure Content</h3>
<p>Open the <code>tailwind.config.js</code> file and locate the <code>content</code> property. Add <code>['./build/*.html']</code> to the array of content:</p>
<pre><code>module.exports = {
  // other configurations...

  content: ['./build/*.html'],

  // other configurations...
}</code></pre>
<p>By specifying the HTML files to be scanned for utility classes, Tailwind CSS will apply the styles to the appropriate HTML files during the build process.</p>

<h3>Step 3: Apply Tailwind CSS</h3>
<p>If you have an existing CSS file that you want to apply Tailwind CSS to, run the following command:</p>
<pre><code>npx tailwindcss -i ./src/input.css -o ./build/css/style.css</code></pre>
<p>This command processes the <code>input.css</code> file and generates a new CSS file called <code>style.css</code>. The output file will be located in the specified directory (<code>./build/css/</code>), ready to be linked in your HTML files.</p>

<h3>Step 4: Watch for Changes (Optional)</h3>
<p>During development, you can watch for changes in your CSS file and automatically rebuild it with the updated Tailwind CSS styles. Add the following script to your <code>package.json</code> file:</p>
<pre><code>"scripts": {
  "tailwind": "npx tailwindcss -i ./src/input.css -o ./build/css/style.css --watch"
}</code></pre>
<p>Running <code>npm run tailwind</code> will enable watch mode, monitoring <code>input.css</code> for changes and updating the output file accordingly.</p>

<h3>Step 5: Install Prettier and Tailwind CSS Plugin</h3>
<p>Run the following command to install Prettier and the Tailwind CSS plugin as development dependencies:</p>
<pre><code>npm i -D prettier plugin tailwindcss</code></pre>

<h3>Step 6: Configure Prettier</h3>
<p>Open the <code>package.json</code> file and locate the <code>scripts</code> section. Add the following script for Prettier:</p>
<pre><code>"scripts": {
  "prettier": "npx prettier --write '**/*.html'"
}</code></pre>
<p>This script formats all HTML files using Prettier.</p>

<p>By following these instructions, you will set up Tailwind CSS, configure content scanning, apply Tailwind CSS styles to your CSS file, watch for changes (if desired), and configure Prettier for formatting HTML files in your web development project.</p>

<p>Please let me know if you need any further assistance or clarification.</p>
