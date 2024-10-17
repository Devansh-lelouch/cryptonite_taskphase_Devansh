u=rw sets read and write permissions for the user, and wipes the execute permission
o=x sets only executable permissions for the world, wiping read and write
a=rwx sets read, write, and executable permissions for the user, group, and world! 


Additionally we can set user/group/world permission different by specifying them with something like :
`chmod u=rw,g=r,o=-` which sets different persmission for user,group and world

WHY IS THIS LEVEL SIMILAR TO THE PREVIOUS ONE ???? 
