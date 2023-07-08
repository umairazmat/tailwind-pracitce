To set up Tailwind CSS for your project, follow these steps:

Run the command (npx tailwindcss init) to initialize Tailwind CSS in your project. This command creates a tailwind.config.js file that allows you to customize the framework's settings.

Open the tailwind.config.js file and locate the content property. Add ['./build/*.html'] to the array of content, specifying the HTML files that should be scanned for utility classes. This ensures that Tailwind CSS is applied to the appropriate HTML files during the build process.

If you have an existing CSS file (e.g., input.css) that you want to apply Tailwind CSS to, run the following command:

npx tailwindcss -i ./src/input.css -o ./build/css/style.css

This command generates a new CSS file (styles.css) in the specified output directory (./build/css/), which includes the processed Tailwind CSS classes from the input.css file.

By following these instructions, you'll be able to integrate and utilize Tailwind CSS in your project effectively.


npx tailwindcss -i ./src/input.css -o ./build/css/style.css --watch
