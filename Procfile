## Shipa generates release artifacts in "dist" directory. 
## Shipa uses a default Procfile if it doesn't find it the app being deployed.

## You can provide your own Procfile, like this one where it's executing using
## dll. Here PORT value is injected by Shipa
web: dotnet dist/myWebApp.dll --urls http://0.0.0.0:$PORT
