# TestMSBuild
This repository is for testing MSBuild behavior.
See https://stackoverflow.com/questions/59876630/how-to-make-msbuild-to-not-stop-on-error-on-net-solution
and https://stackoverflow.com/questions/68380883/set-msbuild-outputpath-conditioned-on-project-name
for details.

Different projects only output in console.

Use `build.bat` or just the following command.
```bat
msbuild Complete.sln /p:Configuration=Debug /p:Platform=x86 /m /t:BuildAll /p:OutputPath=build
```
