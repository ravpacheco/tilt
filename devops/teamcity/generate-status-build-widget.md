# How to generate a icon with status build on TeamCity 

Before we start is necessary remember that if your TeamCity server doesn't have a gest configured is impossible share for everyone a 
icon with build status of your project.

To enable this make shure that:

- Your build step has been enable status widget.
    
        To do this go to 'Edit Settings' and check the option on 'Build Options' sections
        Tip: The 'Build Options' sections is hide by default.   

- After enable status widget, you must generate a URL for status icon

        Use this pattern:
        'https://<server-url>/app/rest/builds/buildType:<build-id-of-your-build-step>/statusIcon.svg' to generate a svg icon 
        
        or
        
        'https://<server-url>/app/rest/builds/buildType:<build-id-of-your-build-step>/statusIcon' to generate a default icon 

        Tip: to found 'buildType' look for url of your build step!