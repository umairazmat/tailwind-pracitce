<h1>Project Setup: Tailwind CSS</h1>
  <h2>Lesson 01</h2>

  <p>To set up Tailwind CSS for your project, please follow the instructions below:</p>

  <h3>Step 1: Initialization</h3>
  <p>Run the following command to initialize Tailwind CSS in your project:</p>
  <pre><code>npx tailwindcss init</code></pre>
  <p>This command creates a <code>tailwind.config.js</code> file in your project directory, which allows you to customize the framework's settings according to your needs.</p>

  <h3>Step 2: Configure Content</h3>
  <p>Open the <code>tailwind.config.js</code> file and locate the <code>content</code> property. Add <code>['./build/*.html']</code> to the array of content, as shown below:</p>
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
  <p>During development, you can watch for changes in your CSS file and automatically rebuild it with the updated Tailwind CSS styles. Use the following command:</p>
  <pre><code>npx tailwindcss -i ./src/input.css -o ./build/css/style.css --watch</code></pre>
  <p>This command enables the watch mode, which monitors the <code>input.css</code> file for changes and updates the output file accordingly.</p>

  <p>By following these instructions, you'll be able to integrate and utilize Tailwind CSS effectively in your project.</p>

  <h2>Lesson 01</h2>

  <p>Please ensure you have the <code>lesson01.png</code> file in your project directory and reference it accordingly in your <code>Readme.md</code> file.</p>
  <img src="lesson01.png" alt="Lesson 01 Screenshot">
