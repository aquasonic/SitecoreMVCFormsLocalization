# Sitecore User Group Switzerland 2015 Demo (April)

This is the demo code for the Sitecore User Group Switzerland 2015. It covers the topic "Sitecore MVC Forms Localization" and was built against Sitecore 8 rev.150223.

## Installation
- Install Sitecore 8 somewhere on your local machine
- Checkout this repository on another location on your local machine
- Add needed assemblies into the `lib` folder (see README in folder for more information)
- Change `SerializationFolder` in `SUGCH2015.config` to your source code folder
- Change Web Deploy folder to your Sitecore installation website root folder and deploy the website
- Add the following assembly redirect to your `web.config` node `configuration/runtime/assemblyBinding`

		<dependentAssembly>
			<assemblyIdentity name="Ninject" publicKeyToken="c7192dc5380945e7" culture="neutral" />
			<bindingRedirect oldVersion="0.0.0.0-3.2.0.0" newVersion="3.2.0.0" />
		</dependentAssembly>
		
- Log into Sitecore as an admin
- Sync the Sitecore items by executing the sync operation on `<domain>/unicorn.aspx`