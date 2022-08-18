## Steps for each new xojotool build

1. Compress the files and folders created by the Xojo build process into a `.zip` file and rename to `xojotool-X.X.X-win64.zip` (where `X.X.X` is the version number). The version number must be bigger than the current one for Scoop to correctly update `xojotool`.
2. Draft a new release for `xojotool` and upload the Windows, Linux and macOS files to the `xojotool` repo. Copy the URL for the Windows download
3. Update the `version` key to the new version number
4. Set the URL in `xojotool.json` to the Windows zip URL
5. Determine the Windows zip file's SHA256 value with the Terminal command: `openssl sha256 [file]`
6. Replace the SHA56 value in the JSON file `hash` key with the new one
7. Commit and push the changes in the JSON file to GitHub.
