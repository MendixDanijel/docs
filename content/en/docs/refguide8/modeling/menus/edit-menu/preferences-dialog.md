---
title: "Preferences"
url: /refguide8/preferences-dialog/
weight: 50
---

## Introduction

The **Preferences** option opens a dialog box where you can set user-specific preferences which apply to the whole of Studio Pro.

## General Tab

### Interface

#### Keep Active Document Selected in Project Explorer

When enabled, **Project Explorer** automatically highlights the document that is currently active. When this property is disabled, the selection in **Project Explorer** remains unchanged when the active document changes.

### MxAssist Logic Bot

#### Enable MxAssist Logic Bot

If **Enable MxAssist Logic Bot** is checked, then [MxAssist Logic Bot](/refguide8/mx-assist-studio-pro/) is activated and can offer suggestions for activities in your microflows.

#### Show Suggestions for System Variables

When **Show suggestions for system variables** is checked, MxAssist Logic Bot will include system objects in its suggestions (for example, it can suggest that you change system objects like currentUser or currentSession).

### Error List

#### Auto-Check Delay

The **Auto-check delay** is the number of milliseconds that Studio Pro waits after a change, before starting the consistency checks. Increase this setting for large projects if Studio Pro responses slowly after changes.

#### Highlight Shown Errors and Warnings in the Editor

When **Highlight shown errors and warnings in the editor** is checked, the errors and warnings which are currently shown in the Error List (as determined by the **Errors** and **Warnings** toggle buttons and the suppression rules) will be highlighted on the affected elements in the editor.

### Deployment

#### JDK directory

This is the directory in which the Java Development Kit (JDK) is located on the computer on which you deploy the application. Usually, the correct directory is located automatically.

The JDK is necessary to run Mendix applications, because the Mendix Runtime is written in Java.

#### Enable Run Optimizations

Enable this setting to increase the speed at which a running application is updated after changes have been made in Studio Pro. When only pages, layouts, or snippets have been changed, an entire restart of the application is skipped to decrease deployment time. Also, no Java compilation is performed when no relevant files have changed.

## Model Tab

### When Prompted by a Widget to Automatically Fill Its Contents, Select 'Yes' by Default

This setting defines the default response to the question whether to automatically fill the contents of a data widget. This question is asked, for example, when dragging an Entity onto a Data View widget. When enabled, the pre-selected answer is **yes**; otherwise, it is **no**.

## Version Control Tab

### File Comparison

#### Executable

This is the path and name of the program that is used to view the details of file changes in the [Commit dialog box](/refguide8/commit-dialog/).

#### Argument Pattern

This is the pattern from which the arguments are derived that are passed to the file comparison program. The following two placeholders can be used in this pattern:

* `{0}` – this is replaced with the name of the original file before the arguments are passed to the file comparison program
* `{1}` – this is replaced with the name of the changed file before the arguments are passed to the file comparison program

### Subversion

#### Enable Private Version Control {#enable}

Select this option when you want to work on an app that is not stored in [Mendix Team Server](/developerportal/general/team-server/), but in another Subversion server to which you have access. This will allow you to specify the location of the app on the Subversion server when opening, downloading, or uploading the app.

## Advanced Tab

### Proxy Server

Sometimes the computer running Studio Pro cannot access the internet directly, but has to connect to a proxy server that requires authentication. If this is the case, then these settings can be used to specify the user name and password to connect to the proxy server.

## New Features Tab {#new-features}

The **New features** tab allows you to turn new features on and off. These are features which are being worked on but are either not yet developed sufficiently to remove the previous version, or which are currently optional.

{{% alert color="info" %}}
You need to restart Studio Pro for changes to these settings to take effect.
{{% /alert %}}

### New Version of the Changes Pane {#new-changes}

With this option, you can enable the new version of the [Changes](/refguide8/changes-pane/) pane. Should you find any issues in the new version, you can switch back to the old version by clearing this checkbox.

Default: *enabled*

### New Version of the Connector {#new-connector}

With this option, you can enable the new version of the [Connector](/refguide8/view-menu/#connector). Should you find any issues in the new version, you can switch back to the old version by clearing this checkbox.

Default: *disabled*

### New Version of the Project Explorer {#new-project-explorer}

With this option, you can enable the new version of the [Project Explorer](/refguide8/project-explorer/). Should you find any issues in the new version, you can switch back to the old version by clearing this checkbox.

Default: *enabled*

### New Version of the Toolbox {#new-toolbox}

With this option, you can enable the new version of the [Toolbox](/refguide8/view-menu/#toolbox). Should you find any issues in the new version, you can switch back to the old version by clearing this checkbox.

Default: *enabled*

## Read More

* [Upload to Version Control Server](/refguide8/upload-to-version-control-dialog/)
* [How to Work with an On-Premises Version Control Server](/howto8/collaboration-requirements-management/on-premises-svn-howto/)
