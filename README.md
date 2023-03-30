# zipme
Contains a class that can be used to compress one or multiple files into a zip file with the option to add password protection.

```python 
from zipper import Zipper

#If you want to zip a single file without password protection
Zipper(input_file_name=<input_file_name>)

#If you want to zip a single file with password protection
Zipper(input_file_name=<input_file_name>, is_password_protected = True, password = <password>)

#If you want to zip all the contents of your current directory without password protection (skips sub-directories and hidden files starting with '.')
Zipper(compress_multiple=True)

#If you want to zip all the contents of your current directory with password protection (skips sub-directories and hidden files starting with '.')
Zipper(is_password_protected = True, password = <password>, compress_multiple=True)

#If you want a custom zip file name
Zipper(input_file_name=<input_file_name>, zip_file_name=<filename.zip>)
```
