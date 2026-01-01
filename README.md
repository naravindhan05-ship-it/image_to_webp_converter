# Image to WebP Converter

A beautiful Flutter app that converts images to WebP format for better compression and quality. This app works on both Android and iOS platforms.

## Features

- 📸 **Camera Integration**: Take photos directly from the camera
- 🖼️ **Gallery Access**: Select images from your photo library
- 🔄 **WebP Conversion**: Convert images to WebP format with high quality
- 💾 **Local Storage**: Converted images are saved to your device
- 🎨 **Modern UI**: Clean, intuitive interface with Material Design 3
- 📱 **Cross-Platform**: Works on both Android and iOS

## Screenshots

The app features a clean, modern interface with:
- Image source selection (Camera/Gallery)
- Real-time conversion progress
- Before/after image preview
- Success/error notifications

## Technology Stack

- **Flutter**: Cross-platform mobile development framework
- **image_picker**: For camera and gallery access
- **image**: For image processing and WebP encoding
- **path_provider**: For file system access
- **permission_handler**: For managing device permissions

## Installation

### Prerequisites

- Flutter SDK (3.7.2 or higher)
- Android Studio / Xcode for platform-specific development
- A physical device or emulator for testing

### Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/naravindhan05-ship-it/image_to_webp_converter.git
   cd image_to_webp_converter
   ```

2. Install dependencies:
   ```bash
   flutter pub get
   ```

3. Run the app:
   ```bash
   flutter run
   ```

## Permissions

The app requires the following permissions:

### Android
- `CAMERA`: To take photos
- `READ_EXTERNAL_STORAGE`: To access gallery images
- `WRITE_EXTERNAL_STORAGE`: To save converted images
- `READ_MEDIA_IMAGES`: For Android 13+ media access

### iOS
- `NSCameraUsageDescription`: Camera access for taking photos
- `NSPhotoLibraryUsageDescription`: Photo library access for image selection

## How to Use

1. **Launch the app** and grant necessary permissions
2. **Tap "Select Image"** to choose your image source
3. **Choose Camera or Gallery** from the bottom sheet
4. **Select/Take your image**
5. **Tap "Convert to WebP"** to start the conversion
6. **View the converted image** and its save location

## WebP Benefits

- **Better Compression**: Up to 25-35% smaller file sizes compared to JPEG
- **Superior Quality**: Better quality at the same file size
- **Transparency Support**: Like PNG but with better compression
- **Animation Support**: Can replace GIFs with better compression
- **Wide Browser Support**: Supported by all modern browsers

## File Structure

```
lib/
├── main.dart              # Main app entry point and UI
android/
├── app/src/main/AndroidManifest.xml  # Android permissions
ios/
├── Runner/Info.plist      # iOS permissions
```

## Dependencies

```yaml
dependencies:
  flutter:
    sdk: flutter
  cupertino_icons: ^1.0.8
  image_picker: ^1.0.4      # Image selection
  image: ^4.1.3             # Image processing
  path_provider: ^2.1.1     # File operations
  permission_handler: ^11.0.1 # Permissions
```

## Platform Support

- ✅ Android (API 21+)
- ✅ iOS (iOS 12.0+)
- ❌ Web (Limited due to file system access)
- ❌ Desktop (Not implemented)

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Troubleshooting

### Common Issues

1. **Permission Denied**: Make sure you've granted camera and storage permissions
2. **Conversion Failed**: Ensure the selected image is in a supported format
3. **File Not Found**: Check if the app has write permissions to storage

### Support

If you encounter any issues, please check:
- Flutter version compatibility
- Device permissions
- Available storage space

## Future Enhancements

- [ ] Batch conversion support
- [ ] Quality adjustment settings
- [ ] Share converted images
- [ ] Image compression statistics
- [ ] Support for more output formats
- [ ] Cloud storage integration
