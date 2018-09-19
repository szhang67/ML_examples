
Steps to run the code

I. Building the code

Once you pull the code from, build it using the command below:
docker build -t "mlw" -f Dockerfile .

or you can pull the docker image directly
docker pull kgunnamieee/mlw

II. Executing the code

To execute the code enter the following command

			docker run -p 8888:8888 -p 6006:6006 -p 6064:6064 mlw 


Now, open the following link

			http://localhost:8888/

Inside the jupyter server, open each notebook and use the commands in jupyter to execute the code



III. Debug mode

To enter the debug mode uncomment the debug part in each file and follow the instructions given there. 

To open the debugger go to the following link,

			http://localhost:6006/

---
command line:
open a separate terminal from host and type "docker ps "
You will get the following output

CONTAINER ID        IMAGE                               COMMAND     CREATED             STATUS              PORTS NAME               
xxxxxxxxxxxxxx        mlw                                 "/mlw/start.sh"
('container_id')
Then do
docker exec -it "container_id"  bash
to attach new bash shell to the same container

