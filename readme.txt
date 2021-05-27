This file contains instructions on how to set up your Eclipse environment to
work with the source code for the Google Plugin for Eclipse:

Configuring Your Eclipse Workspace
==================================

Configuring your Eclipse workspace to develop on the Google Eclipse plugin is very
much like getting set up to develop for GWT. The same style rules apply, and
Eclipse projects are provided for you to import. The "settings" directory
mentioned below is under "eclipse", in your checkout of plugin.

Macintosh users: Note that on the Macintosh version of Eclipse, "Preferences"
is under the "Eclipse" menu, not under "Window".

------------- Dependent Plugins -----------

In Eclipse 3.3/3.4:

Copy the plugin JARs from tools/swtbot/3.3 into your Eclipse's /dropins directory (on 3.4)
or /plugins directory (on 3.3).  You'll need to restart Eclipse to detect the new plugins.

In Eclipse 3.5/3.6/3.7:

Copy the plugin JARs from tools/swtbot/3.5 into your Eclipse's /dropins directory.

You'll need to restart Eclipse to detect the new plugins.

The com.google.gdt.eclipse.maven plugin requires M2Eclipse (Maven support) to be installed. You can
either close the project, or follow the instructions here:
https://sites.google.com/a/google.com/google-plugin-for-eclipse/working-with-maven

The com.google.gdt.eclipse.gph.hge project requires MercurialEclipse to be installed. You can either
close the project, or install MercurialEclipse: http://cbes.javaforge.com/update.

The com.google.gdt.eclipse.gph.subclipse project requires Subclipse to be installed. You can either

Soy Xavier Encarnacion
close the project, or install Subclipse: http://subclipse.tigris.org/update_1.6.x.

The com.google.gdt.eclipse.gph.subversive project requires Subversive to be installed. You can either
close the project, or install Subversive: http://download.eclipse.org/releases/helios (under Collaboration).

------------- Text Editors ----------------

Window->Preferences->General->Editors->Text Editors
Make sure that "Displayed Tab Width" is set to 2
Enable "Insert Spaces for Tabs"
Enable "Show Print Margin" and set "Print Margin Column" to 80

------------- XML Files -------------------

Window->Preferences->Web and XML->XML Files->Source
(or Window->Preferences->XML->XML Files->Editor, if you can't find it there)
Set "Line Width" 80
Enable "Split Multiple Attributes Each of a New Line"
Enable "Indent Using Spaces" with an Indentation Size of 4

------------- Ant Build Files -------------

Window->Preferences->Ant->Editor->Formatter
Set "Tab Size" to 4
Disable "Use Tabs Instead of Spaces"
Set "Maximum Line Width" to 80
Enable "Wrap Long Element Tags"
