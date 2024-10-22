# LibToast

# On a newly pulled codebase install the application
npm install

# Bump the library project version
cd ./projects/lib-toast/;
npm version patch;
cd ../../;

# Build the library
npm run package;

# Sync the workspace version to the library project one
ng-version-sync-parent;

# Publish the library
npm publish ./dist/lib-toast/stephaneeybert-lib-toast-

# Install the dependencies in the client application
npm install @stephaneeybert/lib-toast@latest

# Serve again the client application
Ctrl+C
ng serve
