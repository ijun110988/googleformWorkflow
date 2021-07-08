# Google Form Approval

### Description

This is an approval workflow built with Google Form, Gmail, and Google Apps Script.

### Make a copy of the script

[Make a copy](https://docs.google.com/forms/d/10GCs_lLFg_kUnfLEAzjI6_W8YLhzugjc-G_lBPAUcIg/copy)

### If you prefer to use clasp

[GAS-059 How to use clasp](https://github.com/ashtonfei/google-apps-script-projects/tree/GAS-259) - [Watch on YouTube](https://youtu.be/V-oE2OyvTKM)

### Script Type

Google Form

### Configuration

- Approval flows

```javascript
// Define the approval flows in this object
const FLOWS = {
	defaultFlow: [
		{
			email: "test@gmail.com",
			name: "Ashton Fei (default 1)",
			title: "Team Lead",
		},
		{
			email: "test@gmail.com",
			name: "Ashton Fei (default 2)",
			title: "Manager",
		},
	],
	HR: [
		{
			email: "test@gmail.com",
			name: "HR Lead",
			title: "HR Team Lead",
		},
		{
			email: "test@gmail.com",
			name: "HR Manager",
			title: "HR Manager",
		},
	],
	IT: [
		{
			email: "test@gmail.com",
			name: "IT Lead",
			title: "IT Team Lead",
		},
		{
			email: "test@gmail.com",
			name: "IT Manager",
			title: "IT Manager",
		},
		{
			email: "test@gmail.com",
			name: "IT President",
			title: "IT President",
		},
	],
};
```

- Web App Url

```javascript
this.url =
	"https://script.google.com/macros/s/AKfycbzKrd0zkrNgCm54Ycdv3e82BWxe4r34zSx4iZ0nTMU_TuhApgY/exec"; // IMPORTANT - copy the web app url after deploy
```

- Header name of flow key

```javascript
this.flowHeader = "Department"; // IMPORTANT - key field for your flows
```
