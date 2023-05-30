# Install UI5 CLI

Download [Nodejs](https://nodejs.org/) first.

Run below commands in CMD/Powershell or in any IDE with Terminal.

```bash
# Global installation to have the command available
npm install --global @ui5/cli

# Additional local install in your project
npm install --save-dev @ui5/cli

# Verify installation
ui5 --help
```

# Create a new folder/project and write below Command prompts to get started.

1. This will generate `package.json` file in your project folder.
```bash
npm init --yes
```

2. This will generate `ui5.yml` file in the project.
```bash
ui5 init
```

3. Create `manifest.json` file manually in the **webapp** folder.
```javascript
// Write below code in the manifest file. !Dont Copy this comment!
{
    "sap.app": {
    "id":"sap.ui.demo.walkthrough",
    "type":"application"
  }
}
```

4. Invoke the UI5 Framework using below command prompt.
```bash
ui5 use openui5@latest
```

5. This will add required libraries in the `ui5.yml`.
```bash
ui5 ui5 add sap.ui.core sap.m sap.ui.table themelib_sap_fiori_3
```

6. Finally, use below command to run the local webserver to test your app.
```bash
# It will provide a local host link in the terminal/cmd. Open the link your browser and click on index.html file to run your app.
ui5 serve
```
