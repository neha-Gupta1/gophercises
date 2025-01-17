# Gophercises

**1.Task CLI/Exercise 7**<br>
main ![alt coverage](https://github.com/nehaind/gophercises/blob/master/task/coverage.svg) <br>
db ![alt coverage](https://github.com/nehaind/gophercises/blob/master/task/db/coverage.svg)<br>
cmd ![alt coverage](https://github.com/nehaind/gophercises/blob/master/task/cmd/coverage.svg)<br><br>

**Usage:** Task is the command line TODO list. The application is build using GOlang and BoltDB. The task works as following:<br>
- The task command:<br>
$ ./task
Task is a CLI task manager

Usage:
  task [command]

Available Commands:
  add         Adds a task to your task list.
  do          Adds a task to your task list.
  help        Help about any command
  list        list down whole task list.

Flags:
  -h, --help   help for task

Use "task [command] --help" for more information about a command.
- For adding a new value:

$ ./task add "new task"
value added at index:  1

- For listing the task on the TODO list:<br>

$ ./task list
index:  1  value:  new task

- For marking the task as complete: <br>
$ ./task do 1<br>
marked the task as done and removed from the queue
$ ./task list
no element in the list

**2.Recover middleware/ Exercise 15** <br>

main ![alt coverage](https://github.com/nehaind/gophercises/blob/master/exercise15/coverage.svg) <br>
The Recover Middleware create some HTTP middleware that recovers from any panics in our application and renders a stack trace on the browser. The stack trace on the bowser displays the text in form of links. On clicking on each link the user is redirected to the page from where the panic has occured. The line is also hightlighted.

The exercise covers,
- creating HTTP handlers which provide response according to the path in URL.
- Recoving panic 
- Rendering source code on the borwser and highligthing the text using the chroma package.

**3.Secret**<br>
main ![alt coverage](https://github.com/nehaind/gophercises/blob/master/secret/coverage.svg) <br>
cmd ![alt coverage](https://github.com/nehaind/gophercises/blob/master/secret/cmd/coverage.svg)<br>
encrpyt ![alt coverage](https://github.com/nehaind/gophercises/blob/master/secret/encrypt/coverage.svg)<br>
vault ![alt coverage](https://github.com/nehaind/gophercises/blob/master/secret/vault/coverage.svg)
<br>**Usage:**
The exercise covers,
A command line tool which takes key and the input to be encryptes and stores it in the file.<br>
The tool also decrypts the input by providing the same key<br>
It contains two function get and set for performing the above options,

$ secret set twitter_api_key "some value here" -k "your-encoding-key"<br>
Value set!<br>
$ secret get twitter_api_key -k "your-encoding-key"<br>
"some value here"<br>

**3.Transform**<br>
main ![alt coverage](https://github.com/nehaind/gophercises/blob/master/transform/coverage.svg) <br>
cmd ![alt coverage](https://github.com/nehaind/gophercises/blob/master/transform/primitive/coverage.svg)<br>
**Usage:**<br>
Creating a web server where the user uploads an image, and then is guided through a selection process using various options on the primitive CLI.
