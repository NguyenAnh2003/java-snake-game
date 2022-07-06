# java-snake-game
(socket, TCP, XML processing, database (sql server))
- user interface

![user_Interface](https://user-images.githubusercontent.com/94124019/177462371-a63651ee-7c3a-4917-add7-835757969b35.png)

# every button have sound effect

- snake interface

![snake_Interface](https://user-images.githubusercontent.com/94124019/177463004-f24ecee7-9a11-4de6-80a7-0609344e7ab3.png)


# Deep into program (explain code)
- Login form
Command of this func is "check"
 Details:
 Get all the text from textfield and send (send a list with the command ("check") and name and hash password) to server the server (get the command first ("check") this command represent for 1 function) will processing check the data from client and send response to client (yes, no) 
  yes -> start(button) enable
  no -> do nothing
- Show record (Special)
Command of this func is "show".
  Details: This function client will get the XML file from the server and load data in XML file to table. 
  So what server do here ? Not only send XML file. We also have initXML func for this feature -> So what func do ? -> It will select all the data from database in      desceding and load data on XML file.
- Update point 
Command of this func is "update"
  Details: This func will send point and name to server so it will encounter the updatePoint func (This func will compare the point from client(with username exist in database) and the point(of user) in database) 
  If the point <= point(in database) return; (do noting)
  Else (Update)
# Conclusion
Snake game (using src)
Main: Socket, TCP, File transfer
Sub: Sound effect
More: func with socket.
# Development
More feature :
 - Choosing snake color.
 - Animation with apple (scale .2s)
 - Choosing background color for game. 
 - (Maybe) adding background audio for login form.
