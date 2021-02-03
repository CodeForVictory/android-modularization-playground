
- Where do stuff like analytics go? Infrastructure related for sure
- Where do common ui views go? Or common ui stuff really?
-

To figure out:
- app-infrastructure









- Implementations of core platform stuff? (time, etc.)
- Tooling and libraries implementations?


THOUGHTS

I'm not sure if feature-common makes sense. Instead, we could have just features with ui-integration modules

OR


/ui-common (platform)
    /core (Activity, navigation, MVI, testing components...)
    /fonts
    /resources?

/feature-common
    /campaign
        /ui-integration
        /domain
        /data
    /user
        /ui-integration
        /domain
        /data

    other common model


MY PROJECT:
/feature-ui-integration
    /recipes


OTHER STRUCTURES: (check MVI project. It might not make sense)

/app
/app-feature-common
/app-feature-ui-integration
/app-ui
    if we wanted to have a demo mode, we can just compile the ui features we want, from there, through different build variants.
/app-ui-common
    design system?



