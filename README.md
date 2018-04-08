# Liferay AntiSamy Customization Example

This fragment module customized the Antisamy sanitizer iframe configuration so that you can add iframe tags to your web content.

By default AntiSamy strips iframes from contents (Web Content is currently whitelisted) with this rule:

```
		<tag name="iframe" action="remove"/>
		<tag name="frameset" action="remove"/>
		<tag name="frame" action="remove"/>
```

The altered configuration:

```	 
		<tag name="iframe" action="validate"/>
		<tag name="frameset" action="validate"/>
		<tag name="frame" action="validate"/>
```

# Requirements

Liferay DXP.

# Installation

Download the binary from the latest folder and deploy. 

You also have to define the path to the configuration file of this module in the AntiSamy settings: Control Panel -> System Settings -> Foundation -> Antisamy Sanitizer -> Configuration File URL. Just change the sanitizer-configuration.xml to custon-iframe-configuration.xml.

# Building manually

Clone the repository into your Liferay Workspace modules folders and build.

