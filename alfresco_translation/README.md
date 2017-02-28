
## How to create JAR file

1) Prepare your files. Place all the files you want to include in the JAR file inside a single folder. They will need to be referenced through a single command line, so specifying separate paths is not feasible.
2) Open the command prompt and navigate to the folder where you stored your files.
3) Create the JAR file. The format of the command line for creating the JAR file looks like this: 
<pre>
	<b>jar cf 'jar-file'.jar input-file(s).</b>
</pre> 
* The "jar" portion refers to the jar.exe program, which compiles the JAR file. **jar** command can be used directly if Java JDK bin directory is added to the  **"path"** system variable. Otherwise you have to specify full path to the executable file.
*	The "c" option specifies that you want to create a JAR file
*	The "f" option means that you want to specify the filename.
*	The "jar-file" portion is where you should type the name that you want the file to have.
*	"Input-file(s)" is a space-separated list of all the files to be included in the JAR file.
*	If you add directories to the JAR file, the jar.exe utility will automatically add their contents.

Example for creating translation JAR file:
-  Open command prompt and navigate to the directory **"alfresco-serbian-language-pack\alfresco_translation\source\"** then type in command:
<pre>
	<b>jar cf C:\Serbian-translation.jar *</b>
</pre>
This will create *Serbian-translation.jar* file in the root of your local C drive (you can change the path to your desired location).
