## Prerequisites

- [Node](https://nodejs.org/en/) version should match defined in `.nvmrc`.
>   
> We strongly rercommend using `NVM` for installing Node.
>  
> * Install nvm. [Read more](https://medium.com/@Joachim8675309/installing-node-js-with-nvm-4dc469c977d9)
> * Run `nvm istall 12.x.x` (where '12.x.x' is Node version defined in `.nvmrc`)
> * Run `nvm use 12.x.x` (where '12.x.x' is Node version defined in `.nvmrc`)    


## Development

- Go to project root directory and run in terminal: `npm install` (this command installs all dependencies needed for project. No need to do this if no new packages were added and you allready installed them before)
- From root folder in terminal run `npm run start` (this command runs [webpack development server](https://webpack.js.org/configuration/dev-server/))
- Open http://localhost:9000/

## Deployment

- Go to project root directory and run in terminal: `npm run build` (this command compiles source code and saves all generated files in `.dist` folder)

## Linters

This project has JS and CSS linters added.
- To run [styles lint](https://github.com/stylelint/stylelint): `npm run lint:styles`
- To run [JS lint](https://eslint.org/): `npm run lint:js`


## Tools and dependencies

### WebPack
> We use [webpack](https://webpack.js.org/) for assets compiling and bundling.

### Babel
> We use [babel](https://babeljs.io/) to compile new ES syntax to older versions.

### Handlebars
> We use [handlebars](https://handlebarsjs.com/) for html templating.

### Routing 
> We are using webpack dev server for routing.
> * You can find dev server configuration in `webpack.config.js`.
>  * You can find router configuration in `config/routes.js`.

### Pre-hooks
> We are using [husky](https://github.com/typicode/husky) to add pre commit hook which runs linters every time you commit changes and does not allow to commit if there are any errors.

