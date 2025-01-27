# Basic Level 3
"This time Network Security Sam remembered to upload the password file, but there were deeper problems than that."

<img width="612" alt="1" src="https://github.com/user-attachments/assets/2a71dc94-b54e-4238-b36d-f1f10e66cc28" />


Firstly lets view the *Page Source*

<img width="1380" alt="2" src="https://github.com/user-attachments/assets/b126e52a-b6ae-4e59-b94c-0ce205b3ff00" />

`<input type="hidden" name="file" value="password.php" />`: This is a hidden input field.  

`type="hidden"`: This attribute makes the input field invisible to the user. It does not appear in the user interface.

`name="file"`: Specifies the name of the field. The data can be accessed on the server side using this name.  

`value="password.php"`: Specifies the value of the field. This value is sent to the server. In this case, it sends the information that the file `password.php` needs to be processed. It indicates which file should be handled on the server side.

Now we will use **Path Traversal Method:**

If there is a path traversal vulnerability in the task's code, it may be possible to access the contents of the `password.php` file or other sensitive files on the server. For example, you could try sending a value like `../../../../password.php` to the `file` parameter in an attempt to navigate to parent directories.

<img width="904" alt="3" src="https://github.com/user-attachments/assets/0b5ff895-900e-4160-a5b3-2b3995f81370" />

And here we go:

<img width="197" alt="4" src="https://github.com/user-attachments/assets/af1d7f98-f008-4489-8702-05b61913967f" />

~~**I marked it because i want you guys to find it yourself**~~


<img width="558" alt="5" src="https://github.com/user-attachments/assets/c08aabf6-b8cc-45c8-aa02-15377e47dc40" />

