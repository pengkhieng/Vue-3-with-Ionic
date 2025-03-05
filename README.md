# Vue-3-with-Ionic


# Live Reload Commands

**Start Live Reload Process:**
```bash
// WEB
  ionic serve
// iOS
  ionic cap run ios -l --external
// Android
  ionic cap run android -l --external
```

**Run the App:**
```bash
npx cap run ios
npx cap run android
```

**Open IDE for Android or iOS:**
```bash
npx cap open ios
npx cap open android
```

**Sync the Latest Changes:**
```bash
npx cap sync ios
npx cap sync android
```

**Run the App with Live Reloading Enabled:**
```bash
npx cap run ios --livereload
npx cap run android --livereload
```

***Vue Router Methods***
**Navigation:**

```bash
router.push()
```
- Navigate to a new route (push to the history stack).
  
```bash
router.replace()
```
- Navigate and replace the current route (no history entry).

```bash
router.back()
```
 - Go back to the previous route.

```bash
router.go()
```
 - Go forward or backward a specific number of steps in the history.

**Route Access:**

```bash
router.currentRoute
```
 - Get the current route info.

```bash
router.resolve()
```
 - Resolve a route to a URL.

```bash
router.hasRoute()
```
 - Check if a route exists.
   
**Route Management:**

```bash
router.addRoute()
```
 - Dynamically add routes.

```bash
router.removeRoute()
```
 - Dynamically remove routes.

**Navigation Guards:**

```bash
router.beforeEach()
```
 - Global navigation guard (before navigation).

```bash
router.afterEach()
```
 - Global navigation guard (after navigation).
