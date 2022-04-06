# marketplace-sample-payloads
ADP Marketplace sample request and response JSON payloads
{
  "name": "Selenium_Software",
  "version": "1.0.0",
  "description": "Selenium Packages for testing fusionapps",
  "main": "index.js",
  "scripts": {
    "test": "node node_modules/mocha/bin/mocha --require ts-node/register reportDir=C:/oracle/automation/Reports --browser=CR --no-timeouts --env=C:/oracle/automation/Reports/silver2007cauto.xml --reporter=mochawesome --reporter-options enableCode=false",
    "debug": "node node_modules/mocha/bin/mocha --inspect-brk --require ts-node/register --recursive --no-timeouts  reportDir=C:/oracle/automation/Reports --browser=CR --env=C:/oracle/automation/Reports/silver2007cauto.xml"
  },
  "keywords": [],
  "author": "Jagannadha Prasad",
  "license": "ISC",
  "devDependencies": {
    "@oracle/oraclejet-webdriver": "https://artifacthub-phx.oci.oraclecorp.com/ojet-dev-local/oracle-oraclejet-webdriver-10.1.3.tgz",
    "@oracle/oj-dynamic-webdriver": "https://artifacthub-phx.oci.oraclecorp.com/jet-dev-local/oracle-oj-dynamic-webdriver-10.1.1.tgz",
    "@fndapps/application-adapters": "http://artifactory-slc.oraclecorp.com/artifactory/api/npm/faxarch-npm-virtual/@fndapps/application-adapters/-/@fndapps/application-adapters-0.0.5.tgz",
    "@spectra/oj-spectra-webdriver": "https://artifacthub-phx.oci.oraclecorp.com/atgpf-npm-local/@spectra/oj-spectra-webdriver/-/@spectra/oj-spectra-webdriver-2110.0.0.tgz",
    "@types/chai": "^4.2.1",
    "@types/mocha": "^5.2.7",
    "@types/node": "^13.13.5",
    "@types/selenium-webdriver": "4.0.11",
    "@types/papaparse": "^5.1.1",
    "@typescript-eslint/eslint-plugin": "^3.0.2",
    "@typescript-eslint/parser": "^3.0.2",
    "async": "^3.1.0",
    "axe-reports": "^1.1.11",
    "axe-webdriverjs": "^2.3.0",
    "axios": "^0.19.2",
    "babel-cli": "^6.26.0",
    "babel-plugin-transform-strict-mode": "^6.24.1",
    "chai": "^4.2.0",
    "dateformat": "^3.0.3",
    "desktop-screenshot": "^0.1.1",
    "eslint": "^7.1.0",
    "fs": "0.0.1-security",
    "html-dnd": "^1.2.1",
    "https-proxy-agent": "^5.0.0",
    "husky": "^4.2.5",
    "ignore-case": "^0.1.0",
    "jsonpath": "^1.0.2",
    "lodash": "^4.17.15",
    "log4js": "^5.1.0",
    "mocha": "^6.2.0",
    "mocha-parallel-tests": "^2.3.0",
    "module-alias": "^2.2.0",
    "mochawesome": "^4.1.0",
    "papaparse": "^5.1.1",
    "path": "^0.12.7",
    "platform": "^1.3.5",
    "selenium-standalone": "^6.16.0",
    "selenium-webdriver": "3.6.0",
    "serial-mocha": "0.0.4",
    "setimmediate": "^1.0.5",
    "source-map-support": "^0.5.13",
    "ts-node": "^8.3.0",
    "type-detect": "^4.0.8",
    "typedoc": "^0.15.0",
    "typescript": "^3.6.2",
    "winston": "^3.2.1",
    "xml2js": "^0.4.22",
    "xmldom": "^0.1.27",
    "xpath": "0.0.27",
    "yaml": "^1.6.0",
    "yargs": "^14.0.0",
    "imap": "^0.8.19",
    "nodemailer": "^6.4.8",
    "request-promise": "^4.2.5",
    "pdf2json": "^1.2.0",
    "xlsx": "^0.16.2",
    "qs": "^6.9.4",
    "tough-cookie": "^4.0.0",
    "axios-cookiejar-support": "^1.0.0",
    "jszip": "^3.5.0",
    "diff-js-xml": "1.0.6",
    "oracledb": "^5.0.0"
  },
  "_moduleAliases": {
    "@family": "fusionapps"
  }
}
tsconfig

{
  "compilerOptions": {    
  "target": "es2015",
	"sourceMap": true,	
  "types" : [ "node","mocha","chai" ],
	"downlevelIteration": true,
	"experimentalDecorators": true,
    "typeRoots": [
      "./node_modules/@types"
    ],
    "baseUrl": ".",
    "paths": {
                "*": ["./node_modules/*"],  
		"@family/*": ["fusionapps/*"]
     },
	"lib": [
    "es2015",
    "es2015.promise",
    "DOM",
    "ScriptHost"],
    "noImplicitAny":false,
    "esModuleInterop": true,
    "module": "commonjs",
    "moduleResolution": "node",
	  "allowJs": false,
	  "resolveJsonModule": true
	
  },  
  "include": [ 
	"**/*.ts" 
  ],
  "exclude":[
	"**/node_modules/**"
  ]
}

