Setup Gtk-2.0 into codeblocks
Topic -> compiling projects:
	  -> compiling single file
	  
	  
	 
************************************* Topic: compiling single file       ***********************************************************************************	 

Steps For compiling Single file
Step 1: download following 
Gtk lib from https://download.gnome.org/binaries/win32/gtk+/2.24/gtk+-bundle_2.24.10-20120208_win32.zip.mirrorlist
Codeblock from 




Step 2: extract  and install


step 3 Open codeblocks do following	
		***Here We are adding header files required for compiler***
			1. Goto Settings->Compiler->Global Compiler settings->Search Directory->Compiler-
			2. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\include\gtk-2.0 then ok
			3. click add Paste it<Extract location>\gtk+-bundle_2.24.10-20120208_win32\include\glib-2.0 then ok
			4. click add Paste it <Extract location>gtk+-bundle_2.24.10-20120208_win32\include\pango-1.0 then ok
			5. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\include\gdk-pixbuf-2.0 then ok
			6. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\include\cairo then ok
			7. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\include\atk-1.0 then ok
			8. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\glib-2.0\include then ok
			9. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\gtk-2.0\include then ok

		*** Here We are adding library for compile time ***
			1. Goto Settings->Compiler->Global Compiler settings->Linker Settings-->linker
			2. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\zdll.lib
			3. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\atk-1.0.lib
			4. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\cairo.lib
			5. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\expat.lib
			7. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\fontconfig.lib
			8. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\freetype.lib
			9. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\gailutil.lib
			10. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\gdk_pixbuf-2.0.lib
			11. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\gdk-win32-2.0.lib
			12. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\gio-2.0.lib
			13. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\glib-2.0.lib
			14. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\gmodule-2.0.lib
			15. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\gobject-2.0.lib
			16. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\gthread-2.0.lib
			17. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\gtk-win32-2.0.lib
			18. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\intl.lib
			19. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\libpng.lib
			20. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\pango-1.0.lib
			21. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\pangocairo-1.0.lib
			22. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\pangoft2-1.0.lib
			23. click add Paste it <Extract location>\gtk+-bundle_2.24.10-20120208_win32\lib\pangowin32-1.0.lib
			
step 4.setup runtime enviroment in windows 10/7
		Copying dll files in windows
		
		1.copy all file from location  <Extract location>\gtk+-bundle_2.24.10-20120208_win32\bin\
		2.Open location C:\Windows\SysWOW64\ Paste here
Step 5: Testing 
		run the following code in codeblocks
																		#include <gtk/gtk.h>

																		int main( int   argc,
																	  char *argv[] )
																	{
																GtkWidget *window;

																gtk_init (&argc, &argv);

																window = gtk_window_new (GTK_WINDOW_TOPLEVEL);
																gtk_widget_show  (window);

																gtk_main ();

																return(0);
																	}
															

Success.
************************************* Topic: compiling single file  Complete      ***********************************************************************************	 


************************************* Topic: compiling Projects       ***********************************************************************************	 
Follow the step 1,step 2,step 4 from above.
Now Create New project with Gtk Locate the Folder of  gtk+-bundle_2.24.10-20120208_win32

Done.
Success.



															






															
															






"zdll.lib" "atk-1.0.lib" "cairo.lib" "expat.lib" "fontconfig.lib" "freetype.lib" "gailutil.lib" "gdk_pixbuf-2.0.lib" "gdk-win32-2.0.lib" "gio-2.0.lib" "glib-2.0.lib" "gmodule-2.0.lib" "gobject-2.0.lib" "gthread-2.0.lib" "gtk-win32-2.0.lib" "intl.lib" "libpng.lib" "pango-1.0.lib" "pangocairo-1.0.lib" "pangoft2-1.0.lib" "pangowin32-1.0.lib" 


