Sketch Data Parser plugin by Florian Peninon
------

### Installation
Download the sketch-data-parser.sketchplugin and copy all the files to the Sketch plugins directory at:
+ In Finder, use Go > Go To Folder and paste the following into the box.
(app store)
+ ~/Library/Containers/com.bohemiancoding.sketch/Data/Library/Application Support/sketch/Plugins (beta)
+ ~/Library/Application Support/sketch/Plugins

### How it works?
The plugin use a JSON to populate a list of predefined layers, here is an example :

First, you need to create a group (which will be the model group) with the current naming convention for your editable layers : 
````
$[name of your data]
````
Example : 

![Model group](https://dl.dropboxusercontent.com/u/4822469/groupe-example.png)
##### Warning : the current version of the plugin doesn't include sub-folder, so you have to keep your editable layers at the first level of your model group

In a second time you need to create a JSON with your data :
````
[
 { "name" : "Doris Chapman", "age" : 32, "diet" : "vegan" },
 { "name" : "Hudson Anderson", "age" : 23, "diet" : "low carb" },
]
````
And now you just have to run the plugin, paste the JSON in the prompt and Sketch will automatically duplicate the group for you and populate the new data inside.

### Evolution
Based on the needs I'm planning to add a way to use URL to use pictures.

If you have suggestions, or want to improve my code just do it!

