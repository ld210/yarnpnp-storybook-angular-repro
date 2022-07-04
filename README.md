# Pnptest
This project reproduce a bug with Storybook/Angular, in a Yarn Plug&Play context

Some things worth noting:
- there is a node_modules folder in the repo, that contains a fake cache folder(.pnp). This node_modules folder is only here to keep the Angular CLI happy, until this Pull-Request is published in a future Angular release : https://github.com/angular/angular-cli/pull/23487
- Everything Angular related works (ng serve, ng build, ng test, ng lint)
- to serve the app, run `yarn ng serve`

To reproduce the Storybook bug :
- simply run `yarn ng run pnptest:storybook`
