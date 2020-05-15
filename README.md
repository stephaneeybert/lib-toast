# LibToast

# Bump the version
cd projects/lib-toast/;
npm version patch;
cd ../../;

# Build the library
npm run package;

# Publish the library
npm publish ./dist/lib-toast/stephaneeybert-lib-toast-
ng-version-sync-parent

# In the client application
npm install @stephaneeybert/lib-toast
