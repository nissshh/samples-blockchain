# samples-blockchain
Below is the list pf samples that re added to the repositrou

1. Sending an intkey client (sender) to deployed intkey TP.
Steps
1. Start the validator
$ sudo -u sawtooth sawtooth-validator -vv
2. Deploy settings-tp
$ sudo settings-tp -C tcp://127.0.0.1:4004 -vv
3. Deploy rest-api to start teh rest endoint 
$ sudo sawtooth-rest-api -C tcp://127.0.0.1:4004 -vv
4. Deploy int-key-python
$ sudo intkey-tp-python -vv -C tcp://127.0.0.1:4004
5. Add a sample intley values as 
-Note: I added this step so asto find input and output transactions, at thjis stage I am alos finding a why we need it :)
6. Run the sample Java as a java program from any IDE with inc as a command to increment value.

'

Runing Sawtooth in Peer Mode = Docker

Below are the steps to run Docker in Peer mode, using docker compose

Pre Requisits
- Docker and Docker compose shoudl be installed.


1. Checkout the repository 
2. cd to docker docker/docker-compose
3. Run below command to start peering
$ sudo docker-compose -f sawtooth-local-validator-peer.yaml up
in order to bring down, d Ctrl + C and the run below command
$ sudo docker-compose -f sawtooth-local-validator-peer.yaml down
4. To enter the shell , open the new terminal window  and run below command and then yuo can start testing in peering mode.
$docker exec -it sawtooth-shell-default bash
  


Runnig Sawtooth as PEER and Privitized on Sawtooth
1. Checkout the repository 
2. cd to docker docker/docker-compose
3. Run below command to start peering
4. Enter the shell , open the new terminal window  and run below command and then yuo can start testing in peering mode.
$docker exec -it sawtooth-shell-default bash

We have configured hard keys for the sample to be used for as users and validators . these keys are kept location keys/validagtor and keys/user
