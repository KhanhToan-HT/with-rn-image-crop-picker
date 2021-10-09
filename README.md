# with-rn-image-crop-picker

Expo config plugin for [react-native-image-crop-picker](https://github.com/ivpusic/react-native-image-crop-picker).

### Warning
Only supports iOS right now.

Requires Expo Dev Client. 
Learn more about: 
- Expo Managed Workflow in 2021: [part 1](https://blog.expo.io/expo-managed-workflow-in-2021-5b887bbf7dbb), [part 2](https://blog.expo.io/expo-managed-workflow-in-2021-d1c9b68aa10)
- [Expo Dev Client Docs](https://docs.expo.dev/clients/getting-started/)
- [Expo config plugin](https://docs.expo.io/guides/config-plugins)

## Usage

1. Install with Expo

```sh
$ expo install with-rn-image-crop-picker
```

2. Check your app.json. It should look like this:

```json
 "plugins": [
      "with-rn-image-crop-picker"
    ],
```

3. Rebuild your app

```sh
$ expo prebuild
$ expo run:ios --device
```

## Configuartion

You can configure the iOS messages by adding the following props to your app.json file:

- PhotoLibraryUsageDescription
- CameraUsageDescription
- MicrophoneUsageDescription

Example:
```json
"plugins": [
  [
		"with-rn-image-crop-picker",
		{
			"PhotoLibraryUsageDescription": "Allow app XYZ to access your photos",
			"CameraUsageDescription": "Allow app XYZ to access your camera",
			"MicrophoneUsageDescription": "Allow app XYZ to access your microphone"
		}
	]
]
```

## Contributing

Contributions are very welcome!
