# Vue-3-with-Ionic


# Live Reload Commands

- **Start Live Reload Process:**
  ```bash
  ionic cap run ios -l --external
Run the App:

bash
Copy
Edit
npx cap run ios
npx cap run android
Open IDE for Android or iOS:

bash
Copy
Edit
npx cap open ios
npx cap open android
Sync the Latest Changes:

bash
Copy
Edit
npx cap sync ios
npx cap sync android
Run the App with Live Reloading Enabled:

bash
Copy
Edit
npx cap run ios --livereload
npx cap run android --livereload
Vue Router Methods
Navigation:

router.push() - Navigate to a new route (push to the history stack).
router.replace() - Navigate and replace the current route (no history entry).
router.back() - Go back to the previous route.
router.go() - Go forward or backward a specific number of steps in the history.
Route Access:

router.currentRoute - Get the current route info.
router.resolve() - Resolve a route to a URL.
router.hasRoute() - Check if a route exists.
Route Management:

router.addRoute() - Dynamically add routes.
router.removeRoute() - Dynamically remove routes.
Navigation Guards:

router.beforeEach() - Global navigation guard (before navigation).
router.afterEach() - Global navigation guard (after navigation).
