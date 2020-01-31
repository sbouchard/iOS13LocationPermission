# iOS13LocationPermission
iOS is changing the permission level granted by the user

1- User go to LocationViewController and asked for location permission.
2- requestAlwaysAuthorization called
3- User select Allow Once
4- Current Location permission is set to wheninuse. (Correct behavior)
5- User navigate back to root controller
6- User go again to LocationViewController
7- requestAlwaysAuthorization called
8- No permission is aks, cause already set for this session (Correct behavior)
9- Current Location permission is set to Always. (Wrong) . <----- WHY?? The user never agree to this permission.
