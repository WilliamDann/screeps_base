# Base Screeps Repo

This is my bare bones repo for starting a new screeps bot. It contains a gruntfile to publish changes to screeps and a tsconfig to build ts files.

## Commands
```
npm run clean
```
Empties the dist and bin directories. This is done before a build to remove old files.

```
npm run build
```
Runs the npm clean command and then runs the build command.

```
npm run push
```
Cleans, builds, and runs the gruntfile to push the contents of the build to screeps.

## .screeps.json
This file configures the grunt task to push code to screeps.
```json
{
    "username": "YourUsername",
    "token"   : "your-screeps-token",
    "branch"  : "your-desired-branch",
    "ptr"     : false
}
```

## tsconfig.json
This file configures the typescript compiler. To run the build simply use

```
npm run build
```
