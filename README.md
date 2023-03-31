## =============== sfdx CLI ==========================

# Authorize an Organization through Command Line
```
sfdx force:auth:web:login -r <Your Custom Organization URL>

sfdx force:auth:web:login --setalias vscodeOrg --setdefaultdevhubusername

Ex: sfdx force:auth:web:login -a https://simpsoftsolutions-f-dev-ed.my.salesforce.com/
```

# Logout from org
```
sfdx auth:logout --targetusername my-hub-org
sfdx auth:logout --all
```

# Push/Deploy the code into Salesforce
```
sfdx force:source:retrieve -m LightningComponentBundle

sfdx force:source:retrieve -m LightningComponentBundle -u aparupa123@simpsoft.com

sfdx force:source:retrieve -m ApexClass.MultiSelectLookupController  -u aparupa123@simpsoft.com
sfdx force:source:retrieve -m CustomObject,ApexClass
sfdx force:source:retrieve -m ApexClass:MyApexClass

sfdx force:source:retrieve -x manifest/package.xml
```

# Push/Deploy the code into Salesforce
```
sfdx force:source:deploy -m LightningComponentBundle

sfdx force:source:deploy -m LightningComponentBundle -u aparupa123@simpsoft.com

sfdx force:source:deploy -m ApexClass.MultiSelectLookupController -u aparupa123@simpsoft.com
```

# Install LWC DevServer for Live Preview
```
sfdx plugins:install @salesforce/lwc-dev-server
npm install -g node-gyp
npm install --global --production windows-build-tools
```

# LWC LIve Preview STart
```
sfdx force:lightning:lwc:start
```
