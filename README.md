{
  "name": "vlc-like-electron",
  "version": "0.1.0",
  "description": "A small Electron-based VLC-like media player starter",
  "main": "src/main.js",
  "scripts": {
    "start": "electron .",
    "electron": "electron .",
    "build": "echo \"No build step - ready for packaging\"",
    "electron:build:win": "electron-builder --win",
    "electron:build:mac": "electron-builder --mac"
  },
  "author": "navidumediapayer",
  "license": "MIT",
  "devDependencies": {
    "electron": "^25.0.0",
    "electron-builder": "^24.6.0"
  },
  "build": {
    "appId": "com.example.vlclike",
    "files": [
      "**/*"
    ],
    "directories": {
      "buildResources": "build"
    },
    "win": {
      "target": [
        "nsis"
      ]
    },
    "mac": {
      "target": [
        "dmg"
      ]
    }
  }
}
