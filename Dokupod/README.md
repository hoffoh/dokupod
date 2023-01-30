Configure local storage
--------------------------
#>DOKUPATH=/home/hoffoh/dokupodstore
#>mkdir $DOKUPATH
#>podman unshare chown -R 1000:1000 $DOKUPATH
#>sudo semanage fcontext -a -t container_file_t '/home/hoffoh/dokupodstore(/.*)?'
#>sudo restorecon -Rv $DOKUPATH
