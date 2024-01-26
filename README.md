## Design: Responsive Web App with Google Collections Graph Visualization

### HTML Files

1. `index.html`:
   - The main HTML file that serves as the entry point for the web application.
   - This file will contain the necessary HTML structure and elements to display the user interface.
   - The user interface should include:
     - A form to allow users to input the Google Collections URL.
     - A button to submit the URL and generate the graph visualization.
     - A section to display the generated graph.
   - The HTML should be user-friendly, responsive, and visually appealing.

2. `graph.html`:
   - This HTML file will be responsible for displaying the generated graph visualization.
   - It will contain the necessary HTML structure and elements to render the graph.
   - The graph should be interactive, allowing users to zoom, pan, and explore the semantic relationships between the items.

### Routes

1. `/`:
   - This route will handle the root URL of the application, which should load the `index.html` file.

2. `/generate-graph`:
   - This route will handle the submission of the Google Collections URL.
   - It will extract the URL from the request, fetch the list of items from the URL, and generate the graph visualization.
   - The generated graph should be returned as a JSON response.

3. `/display-graph`:
   - This route will handle the request to display the generated graph.
   - It will load the `graph.html` file and provide the graph visualization as data for the template to render.