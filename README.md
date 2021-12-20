# Supernode List
Here we update supernode list in *supernode.json*.

For example:

    "Enlink": {
        "region": "Korea",
        "url": "https://lora.rosanetworks.com",
        "logo": "https://lora.rosanetworks.com/branding.png",
        "darkLogo": "https://lora.rosanetworks.com/branding_dark.png",
        "status":"online"
    },

# Latest version of DataDash app
Here we update latest version and latest supported version of DataDash app in *latest_app_version.json*.

    {
        "_comment": "Implemented in DataDash app in v2.0.3",
        "latest_app_version": {
            "version": "2.0.1",
         "message": "latest version test"
        },
        "latest_supported_app_version": {
            "version": "2.0.0",
            "message": "latest supported version test"
        }
    }

When DataDash app starts, it checks if currently running version of the app is below **latest_app_version.version**, in which case the app opens a page with **latest_app_version.message**.

It also check if currently running version of the app is below **latest_supported_app_version.version**, in which case the app shows a blocking page with **latest_supported_app_version.message**, and user must update the app.