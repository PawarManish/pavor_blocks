# video: mauli_builds.mp4
# command to run project : npm start

# solve error ( port already in use {port_number})

1.  1.  find PID of running port => netstat -ano | findstr :3000 (in gitbash)
    2.  check PID i.e number in front of word LISTENING
    3.  close it ( write this ans in terminal powershell, not in gitbash)
        ans => taskkill /PID 15824 /F
    4.  example
        ~/Desktop/pinterest (master) $ netstat -ano | findstr :3000
        TCP 0.0.0.0:3000 0.0.0.0:0 LISTENING 15824
        TCP [::]:3000 [::]:0 LISTENING 15824
        TCP [::1]:62585 [::1]:3000 TIME_WAIT 0

# run project
ans=> npm start or nodemon

