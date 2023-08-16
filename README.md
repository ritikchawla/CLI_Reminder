# GOLANG CLI Reminder

  

The **GOLANG CLI Reminder Tool** is a command-line utility written in Go that allows you to set reminders for yourself by specifying a time and a text message. When the specified time is reached, the tool will display a reminder with the provided message.

  

## Installation

  

Before using the GOLANG CLI Reminder Tool, you need to install the required dependencies. Run the following command to install the necessary packages:

  

```sh
go  get  github.com/gen2brain/beeep
go  get  github.com/olebedev/when
go  get  github.com/olebedev/when/rules/common
go  get  github.com/olebedev/when/rules/en
```

After  installing  the  dependencies,  you  can  build  the  tool  using  the  following  command:

  

```sh
go build -o reminder-tool main.go
  ```

## Usage

  

To use the GOLANG CLI Reminder Tool, follow the format below:

```sh
./reminder-tool <hh:mm> <text  message>
```  

- <`hh:mm`>:  The  time  at  which  you  want  to  receive  the  reminder  in  the  format  "hh:mm".

- <text  message>  The  message  you  want  to  display  as  the  reminder.


## Examples

 1. Set  a  reminder  for  3:30  PM  with  the  message  "Call Rohit":
	  ```
	./reminder-tool  15:30  "Call Rohit"
	  ```

2. Set  a  reminder  for  9:00  AM  with  the  message  "Work Meeting":
	  ```
	./reminder-tool  09:00  "Work Meeting"
	  ```
  

## Notes

- The  tool  will  only  display  reminders  for  future  times.

- The  reminder  will  be  displayed  using  the  beeep  package,  and  an  alert  sound  will  be  played.

- If  you're running the tool in the background, it will wait until the reminder time is reached before displaying the reminder and playing the sound.

  

## Thanks
I am passionate about exploring new technologies and creating exciting projects. If you have interesting project ideas and would like to collaborate, feel free to reach out to me via [email](mailto:chawlaritik@gmail.com).