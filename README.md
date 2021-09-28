## [Repository Name]

Read the properties of the json config file and insert it as environment variables in the workflow.


**Table of Contents**

<!-- toc -->

- [Description](#description)
- [Usage](#usage)
    + [Setting variables](#setting-variables)
    + [Without setting variables](#without-setting-variables)
- [License Summary](#license-summary)

<!-- tocstop -->


## Description
The action allow you to read a json file and insert the properties as a environment variables in the workflow that invoke the action.

## Usage
You can insert a custom file-path and the level that you want to read or leave the default properties.

	file-path:
		required: false
		default: ci-config.json
		
	level:
		required: false
		default: ./

### Setting Variables

	- uses: Iberia-Ent\software-engineering--read-file-action@v1
	  with: 
			file-path: './ci-config.json'
			level: '.dev'
		
### Without Setting Variables

	- uses: Iberia-Ent\software-engineering--read-file-action@v1
	  
## License Summary
This code is property of Iberia-Ent.