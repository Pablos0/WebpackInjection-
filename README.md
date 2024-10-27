# build-deploy-webpack

This is the starting code to build and deploy using webpack. It is a continuation of Fruit Marketplace.

Below command will run the application 

``` python3 -m http.server ```

Directory SRC refer to source directories. DIST is for output directories.

# Adding below command will install a web pack 

``` npm install webpack webpack-cli html-webpack-plugin --save-dev ```

- <font color="blue">webpack</font> is a module bundler. Its main purpose is to bundle JS files for usage in a browser, yet it is also capable of transforming, bundling, or pachaging just about any resource or asset.
- <font color="blue">webpack-cli</font> provides a flexible set of commands for developers to increase speed when setting up a custom Webpack project.
- <font color="blue">html-webpack-plugin</font> simplifies the creation of HTML files to serve the Webpack bundles.  

<font color="blue">package.json</font> holds importan information about the project. It contains both human-readable metadata about the project, such as the project name and description, and the functional metadata, such as the package version number and a list of dependencies required by the application.
<font color="blue">package-lock.json</font> is automatically generated for any operations where npm modifies either the <font color="blue">node_modules</font> tree or <font color="blue">package.jsom</font>. It describes the exact tree that was generated, allowing subsequent installs to generate identical trees regardless of intermediate dependency updates.     

## Running Webpack 

<font color="blue">npx webpack</font> create <font color="blue">dist/main.js</font> file using as script <font color="blue">src/index.js</font> 

``` cd dist ```
``` python3 -m http.server ``` 

To import assets is required type below codes 

CSS import
``` <link rel="stylesheet" href=<%=require('./css/main.css')%> type="text/css" media="all" /> ```

Title
``` <title><%= htmlWebpackPlugin.options.title %></title> ```

Meta description
``` <meta name="description" content="<%= htmlWebpackPlugin.options.metaDesc %>" /> ```

Header 
``` <h1 class="text-center"><%= htmlWebpackPlugin.options.header %></h1> ```

Images 
```<img src=<%=require('./images/img_name.jpg')%> alt="...." /> ```

- In root directory run
``` npx webpack ```

- In dist directory
``` python3 -m http.server ```