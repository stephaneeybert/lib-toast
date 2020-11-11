# LibToast

# Bump the library project version
cd projects/lib-toast/;
npm version patch;
cd ../../;

# Build the library
npm run package;

# Sync the workspace version to the library project one
ng-version-sync-parent;

# Publish the library
npm publish ./dist/lib-toast/stephaneeybert-lib-toast-

# In the client application
npm install @stephaneeybert/lib-toast
