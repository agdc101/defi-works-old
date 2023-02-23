# defi-works installation guide


## Infrastructure set-up

1) Install Homebrew (for Mac/Linux) == "Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple's operating system, macOS, as well as Linux." == https://brew.sh/

2) Install Composer == "Composer is an application-level dependency manager for the PHP programming language that provides a standard format for managing dependencies of PHP software and required libraries" == https://getcomposer.org/download/

3) Install Symfony == "Symfony is a free and open-source PHP web application framework and a set of reusable PHP component libraries." == https://symfony.com/download

4) Install Yarn == "Yarn is one of the main JavaScript package managers, developed in 2016 by Facebook for the Node.js JavaScript runtime environment." == https://classic.yarnpkg.com/en/docs/install#mac-stable == (This will also install Node.js if it is not already installed.)

6) Install webpack encore == "Webpack is a free and open-source module bundler for JavaScript." == composer require encore.

7) Install babel == "JSX should not be implemented directly by browsers, but instead requires a compiler to transform it into ECMAScript. This is where Babel comes in. Babel acts as this compiler allowing us to leverage all the benefits of JSX while building React components" == yarn add @babel/preset-react@^7.0.0 --dev

7) Install mySQL server & mySQL GUI (Workbench) == "The MySQL server provides a database management system with querying and connectivity capabilities" == create mySQL database.

## Project File Set-up

1) Create new Symfony app - in terminal of Project folder "symfony new --webapp <project-name>".
  
2) Create env.local file - change database URL.
  
3) In terminal, Run "yarn install" == to install project dependancies.
  
4) In terminal, Run "symfony server:start" == starts symfony server, go to web address to make sure all ok.
  
5) In terminal, Run "yarn encore dev --watch" == Yarn/encore webpack watching for code changes.
  
6) Enable React in webpack.config.js file == uncomment ".enableReactPreset()".
  
7) In terminal, Run "bin/console make:controller" == makes Symfony controller so routes can be handler. Follow prompts.
  
### run in terminal --> "symfony server:start" --> "yarn encore dev --watch".
