# Base Screeps Repo

This is my bare bones repo for starting a new screeps bot. It contains a gruntfile to publish changes to screeps and a tsconfig to build ts files.

## Usage
1. Clone the repo
2. Modify your .screeps.json
3. Install grunt scripts
4. Push some code

### 1. Clone the Repo
The first step to use the screeps base template is cloning this repo. The command below will do this:

```
git clone https://github.com/WilliamDann/screeps_base.git
```

### 2. Modify your .screeps.json

The .screeps.json file is configuration for the screeps grunt worker. Below is an example of a .screeps.json file:

```json
{
    "username": "YourScreepsUsername",
    "token"   : "your-screeps-token",
    "branch"  : "your-desired-branch",
    "ptr"     : false
}
```

To generate a token, visit the "Manage Account" menu in the top right of the client. The "Auth Tokens" section allows you to create an auth token.

### 3. Install grunt scripts
The dependancies are listed in the package.json already - all you need to do is run the install command.
```
npm i
```

### 4. Push Some Code

There are three commands included in the package.json.
1. Clean
2. Build
3. Push

#### Clean
```
npm run clean
```
This removes the bin/ and dist/ directories. Removing these removes old files from the build.

#### Build
```
npm run build
```
This runs a clean, then runs the typescript compiler.

#### Push
```
npm run push
```

This runs a clean, a build, and uses the gruntfile to push code.

You should be all set to write code! 
