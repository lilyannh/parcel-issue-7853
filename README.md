# Sample repo for issue 7798 https://github.com/parcel-bundler/parcel/issues/7798

### From root package.json:

- `npm run root-app1-start` will start up app1. If you make changes in `app1\src\App.jsx`, the console will clear, but changes will not appear in the page until you manually refresh.
- `npm run root-app2-start` will start up app2. If you make changes in `app2\src\App.jsx`, HMR works.

### From app1 package.json:

- `npm run app1-start` will start up app1. If you make changes in `app1\src\App.jsx`, the console will clear, but changes will not appear in the page until you manually refresh.

Note that there is no package.json in app2 subfolder. It seems like maybe the subfolder package.json is getting in the way? In this simple example, the package.json in the subfolder is not needed, but in practice, I would like to have them to define aliases and npm scripts specific to the subfolder.
