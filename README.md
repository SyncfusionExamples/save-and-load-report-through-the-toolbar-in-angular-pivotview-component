# Export and import reports as JSON through custom toolbar options (Angular Pivot Table)

The Syncfusion Angular Pivot Table allows you to persist and restore report settings (also referred to as dataSourceSettings). In this sample, two custom toolbar actions are provided:
- **Save**: Exports the current Pivot Table configuration as a JSON file (for example, pivot.json).
- **Open**: Imports a previously saved JSON file and applies it to the Pivot Table.

These actions help users back up, share, or reload their exact Pivot Table layout, including rows, columns, values, filters, sorting, formatting, and more.

## ⚙️ How it works
This sample uses the **toolbarTemplate** property of the Pivot Table to render two custom controls in the toolbar:
- A Save button (anchor element) that serializes the current report using getPersistData, converts it to a downloadable file, and triggers a download in the browser.
- An An Open input (file element) that reads a selected JSON file using the FileReader API and then assigns the parsed content back to the component’s dataSourceSettings to instantly restore the report.

Key APIs and references used:
- [`dataSourceSettings`](https://ej2.syncfusion.com/angular/documentation/api/pivotview/#datasourcesettings)
- [`toolbarTemplate`](https://ej2.syncfusion.com/angular/documentation/api/pivotview/#toolbartemplate)
- [`getPersistData`](https://ej2.syncfusion.com/angular/documentation/api/pivotview/#getpersistdata)
- [`change event (MDN)`](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/change_event)

## 🛠 Prerequisites
- Node.js (LTS recommended)
- Angular CLI (to run locally with ng serve)
- Visual Studio Code (or any preferred editor)

## 📦 Installation and Running the Sample
1. Clone this repository:
   - https://github.com/SyncfusionExamples/save-and-load-report-through-the-toolbar-in-angular-pivotview-component
2. Open the project in Visual Studio Code.
3. Install dependencies:
   - In the integrated terminal, run:
     - npm install
4. Start the development server:
   - ng serve
5. Navigate to the URL shown in the terminal (typically http://localhost:4200) to view the sample.

## ✅ Compatibility
- This sample targets the Angular version specified in package.json. Update your local Node.js and Angular CLI to compatible versions if you encounter setup issues.

## 📚 Learn More

- [Getting Started with Syncfusion Angular Pivot Table](https://ej2.syncfusion.com/angular/documentation/pivotview/getting-started)
- [Live Feature Samples and Demos](https://ej2.syncfusion.com/angular/demos/#/tailwind3/pivot-table/overview)

## 💬 Support and Feedback

For any other queries, contact our [Syncfusion® support team](https://support.syncfusion.com/?utm_source=github&utm_medium=listing&utm_campaign=github-github-documenteditor-examples) or post your queries through the [community forums](https://www.syncfusion.com/forums?utm_source=github&utm_medium=listing&utm_campaign=github-github-documenteditor-examples). 

Request a new feature through [Syncfusion® feedback portal](https://www.syncfusion.com/feedback?utm_source=github&utm_medium=listing&utm_campaign=github-github-documenteditor-examples). 

## 📜 License

This is a commercial product and requires a paid license for possession or use. Syncfusion's licensed software, including this component, is subject to the terms and conditions of [Syncfusion's EULA](https://www.syncfusion.com/license/studio/22.2.5/syncfusion_essential_studio_eula.pdf?utm_source=github&utm_medium=listing&utm_campaign=github-github-documenteditor-examples). You can purchase a license [here](https://www.syncfusion.com/sales/products?utm_source=github&utm_medium=listing&utm_campaign=github-github-documenteditor-examples) or start a free 30\-day trial [here](https://www.syncfusion.com/account/manage-trials/start-trials?utm_source=github&utm_medium=listing&utm_campaign=github-github-documenteditor-examples)
