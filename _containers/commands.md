# Docker - COMMANDS

## Launching Container

| command                                                   | description                           | 
| ---                                                       | ---                                   |
| docker container ls                                       | list RUNNING docker containers        |  
| docker container ls -a                                    | list ALL containers                   |  
| docker run --interactive --name < nameOfContainer > ____  |                                       | 
| -d                                                        | run detached                          |

## Accessing Container

> docker exec

| command                                                   | description                           | 
| ---                                                       | ---                                   |
| docker exec < nameOfContainer > ____                      | run command against a container       | 
| docker exec -it < nameOfContainer > bash                  | drop into a shell                     | 

## Edit Files

| command                                                   | description                           | 
| ---                                                       | ---                                   |
| docker cp < source > < container > : < destination >      | copy file                             | 
| docker cp < container > : < source > < destination >      | copy file                             | 

## Container Management

| command                                                   | description                           | 
| ---                                                       | ---                                   |
| docker stop _____                                         |                                       | 
| docker rm < containerName >                               | removes single container              | 
| docker container prune                                    | removes all stopped containers        | 
| docker rename                                             | renames the container                 | 
| docker stats                                              | information about the container       | 