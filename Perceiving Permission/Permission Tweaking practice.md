Its some kind of game round of 8 which i dont like because i have to restart multiple times . 

At the start of the game : 
  Current permissions - 
    User: Read and Write
    Group: Read only
    World : Read only 

 Permission needed:
     User: Read and Write
     Group : No permission
     World : Read only 

So at the first step we have to remove the read permission of the group 
`chmod g-r /challenge/pwn`

`chmod 666 /challenge/pwn`

