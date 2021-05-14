# Update Android version Gradle action

This action update the `versionCode` and `versionName` properties of the build.gradle file for your Android projects.

## Inputs

### `build-gradle-path`

**Required** The relative path for the build.gradle file.

### `version-code` 
  
**Required** The value of the version code, this must be between 0 and 2100000000.

###  `version-name`
    
**Required** The value of the version name

###  `print-file`

Output the build.gradle file in console before and after update.

## Usage

```yaml
- name: Update gradle version for Android
  uses: damienaicheh/update-android-version-gradle-action@v1.0.0
  with:
    build-gradle-path: './path_to_your/build.gradle'
    version-code: 2
    version-name: '2.0'
    print-file: true
```