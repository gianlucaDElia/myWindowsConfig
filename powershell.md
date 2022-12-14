## Create powershell user profile
```
New-Item $PROFILE.CurrentUserCurrentHost -ItemType file -Force
```

## Change execution policy
```
Set-ExecutionPolicy -ExecutionPolicy Unrestricted
```
