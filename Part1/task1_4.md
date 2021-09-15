
1. `docker run -d -it --name looper ubuntu sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'`
2. `docker container ls` to check everything went well so far
3. `docker exec -it looper bash`to get inside the container 
4. `apt-get update; apt-get install curl;`

Then everything was messy for the next 20 minutes... Desperately trying everything I have "learnt". 

After that I managed to google that -ai is the magic flag to solve my problems and with that I get the terminal ask the website address again: 

5. `docker kill looper; docker start -ai looper;`

And afterwards I realized that the `-a` flag wasn't necessary, only `-i` would have been enough. 

