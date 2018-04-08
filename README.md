# Liferay AntiSamy Customization Example

This fragment module customized the Antisamy sanitizer iframe configuration so that you can add iframe tags to your web content.

By default AntiSamy strips iframes from web content with this rule:

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

Download the binaries from the latest folder and deploy.

# Building manually

Clone the repository into your Liferay Workspace modules folders and build.

