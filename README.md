# shell01
School 42 project
# Chapter VIII - Exercise 05: Can you create it?

### Exercise Overview

In this exercise, you are required to create a file with a very specific name, containing only the text `"42"` and nothing else.

### Requirements:
- The file must contain **only** the text `"42"`.
- ### Steps to complete the exercise:

1. Open your terminal.
2. Create the file with the required name. Since the filename contains special characters, you need to escape them:
  ```bash
  touch \\\?\$\*\'MaRViN\'\*\$\?\\
  ```
  This will create a file with the name `\?$*'MaRViN'*$?\`.

3. Open the file in a text editor or use the `echo` command to add the string `"42"`:
  ```bash
  echo -n "42" > \\\?\$\*\'MaRViN\'\*\$\?\\
  ```
  The `-n` flag prevents adding a new line after `"42"`.

4. Verify the file's content to ensure it contains only `"42"`:
  ```bash
  cat \\\?\$\*\'MaRViN\'\*\$\?\\
  ```

5. You can also confirm the file's existence with the `ls` command:
  ```bash
  ls -lRa *MaRV* | cat -e
  ```

### Example output:

```bash
$> ls -lRa *MaRV* | cat -e
-rw---xr-- 1 75355 32015 2 Oct 2 12:21 "\?$*'MaRViN'*$?\"
