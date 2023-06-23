# Create Release Example

When you have completed an activity, and you think you should add it to the Changelog, then run the command `npx changeset` 
on your machine.
Follow the wizard, it will ask you what kind of type of change you have made, and what the change is.
Then it will create a file into the `.changeset` folder.

When you think you are ready to release a new version of your package, then run the command `npm run version`.
Command `npm run version` converts the changes in the `.changeset`folder into a `CHANGELOG.md`file.

## Known Issues
Changeset doesn't update the version within `package-lock.json`, so if you release a new version without updating it, on 
the next `npm install` command you will see changes. 
