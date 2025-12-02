# App Icon Documentation

## Pocket Dictionary App Icon

The app icon has been updated with a professional dictionary-themed design.

### Design Description

The icon features:
- **Background**: Clean blue color (#1565C0) representing knowledge and trust
- **Foreground**: An open book with:
  - White left page with text lines
  - Light gray right page with a prominent letter "A" 
  - Gray book spine/binding in the middle
  - Definition text lines below the letter
  
The design clearly conveys that this is a dictionary application.

### Icon Files

The icon system uses Android's Adaptive Icon format for modern devices (API 26+):

#### Vector Drawables
- `res/drawable/ic_launcher_background.xml` - Blue background layer
- `res/drawable/ic_launcher_foreground.xml` - Book and letter "A" design

#### Adaptive Icons
- `res/mipmap-anydpi-v26/ic_launcher.xml` - Main launcher icon (adaptive)
- `res/mipmap-anydpi-v26/ic_launcher_round.xml` - Round launcher icon (adaptive)

#### Raster Images (Legacy)
WebP format icons are generated for older devices in various densities:
- `res/mipmap-mdpi/` (48x48 dp)
- `res/mipmap-hdpi/` (72x72 dp)
- `res/mipmap-xhdpi/` (96x96 dp)
- `res/mipmap-xxhdpi/` (144x144 dp)
- `res/mipmap-xxxhdpi/` (192x192 dp)

### Color Scheme

- **Background**: #1565C0 (Blue 700 - Material Design)
- **Book Pages**: #FFFFFF (White) and #F5F5F5 (Very Light Gray)
- **Book Spine**: #E0E0E0 (Light Gray)
- **Letter "A"**: #1565C0 (Matching background for consistency)
- **Text Lines**: #BDBDBD (Gray)

### AndroidManifest Configuration

The manifest is properly configured to use the new icon:

```xml
<application
    android:icon="@mipmap/ic_launcher"
    android:roundIcon="@mipmap/ic_launcher_round"
    ...>
```

### Testing

To test the icon:
1. Build and install the app on a device/emulator
2. Check the home screen launcher
3. Test on different Android versions to see adaptive icon behavior
4. Verify it looks good on both light and dark backgrounds

### Adaptive Icon Benefits

- Automatically adapts to different device shapes (circle, squircle, rounded square)
- Supports parallax effects and animations on supported devices
- Monochrome variant for themed icons (Android 13+)
- Better visual consistency across the Android ecosystem

