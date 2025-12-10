 - [libft](https://github.com/jlutrera/libft): General-purpose C library.
 - [ft_printf](https://github.com/jlutrera/ft_printf): Reimplementation of printf().
 - [get_next_line](https://github.com/jlutrera/get_next_line): Function that returns a line from a file descriptor.
 - [Born2beroot](https://github.com/jlutrera/Born2beroot): Systems administration exercise.
 - [push_swap](https://github.com/jlutrera/push_swap): Stack sorting with minimal operations.
 - [Minitalk](https://github.com/jlutrera/minitalk): Data exchange via UNIX signals.
 - [FDF](https://github.com/jlutrera/FdF): 3D wireframe rendering.
 - [philosophers](https://github.com/jlutrera/philosophers): Threads and mutex synchronization.
   - El proyecto presenta cierto retraso en la ejecución que se resuelve simplificando los mensajes (dejar el texto sin más)
Pierde vistosidad y gana en eficiencia de ejecución.  En la última versión he añadido un flag (-v) que muestra el programa como lo tenía.  Sin éste flag se muestra el texto sin tanto formato, ganando en tiempo de ejecución y funcionando mejor el algoritmo.

Para ver CON formato:
		./philo -v arg1 arg2 arg3 arg4 [arg5] 
y sin formato:
		./philo arg1 arg2 arg3 arg4 [arg5] 
 - [minishell](https://github.com/jlutrera/minishell): Simple shell implementation.
 - [miniRT](https://github.com/jlutrera/miniRT): Basic ray tracing renderer.
 - [NetPractice](https://github.com/jlutrera/NetPractice): Networking exercises.
 - [CPP 00_04](https://github.com/jlutrera/CPP_00_04): C++ modules 00–04.
 - [CPP 05_09](https://github.com/jlutrera/CPP_05_09): C++ modules 05–09.
 - [Inception](https://github.com/jlutrera/Inception): System administration with Docker.
 - [webserv](https://github.com/jlutrera/webserv): HTTP server implementation.
 - [ft_transcendence](https://github.com/jlutrera/ft_transcendence): Full web application for Pong contest.
   - The last project of the 42 common core.

This project is **single page application** that allows users to create accounts, log in, and play a game of pong against other users.

The project is divided into three main parts:

-   **Web Sockets and algorithms**: The game is played in real time from different clients, using **web sockets** to communicate the game state between the clients and the server.

-   **Frontend**: A **vanilla JS** fronted that accts as a **single page application**, requesting the data to the backend and updating the DOM accordingly. And using **Bootstrap** for the styling of the page.

-   **Backend**: A Django server that provides an API for the frontend to interact with using **Django-Ninja** and using **Postgres** as a database. It also manages the game state and the web sockets connections.

This project runs in **Docker**. Using three containers:

-   **Django** (API and backend) 🐍

-   **Postgres** (database) 🗄️

-   **Nginx** (frontend) 🌐

# Team work 💪

This project was a team effort. You can checkout the team members here:

-   **José Luis Utrera**
    -   [Github](https://github.com/jlutrera)
    -   [LinkedIn](https://www.linkedin.com/in/jose-luis-utrera-5860a9297/)
    -   [42 intra](https://profile.intra.42.fr/users/jutrera-)
-   **Adrian Pacheco**
    -   [Github](https://github.com/Paches19)
    -   [LinkedIn](https://www.linkedin.com/in/adri%C3%A1n-pacheco-ter%C3%A1n-2154641b5/)
    -   [42 intra](https://profile.intra.42.fr/users/adpachec)
-   **Alejandro Aparicio**
    -   [Github](https://github.com/magnitopic)
    -   [LinkedIn](https://www.linkedin.com/in/magnitopic/)
    -   [42 intra](https://profile.intra.42.fr/users/alaparic)

# Run project

## With Docker

```bash
cp .example.env src/docker/.env

#Enter values for the variables in the .env file
vim src/docker/.env

make
```

## Without docker

Run the backend

```bash
cd /src/backend

docker run --name some-postgres -e POSTGRES_PASSWORD=postgres123 -e POSTGRES_USER=postgres -e POSTGRES_DB=transcendence_db -p 5432:5432 -d postgres

export POSTGRES_DB=transcendence_db POSTGRES_USER=postgres POSTGRES_PASSWORD=postgres123

python manage.py migrate

python manage.py runserver
```

# Database schema

In the project database we store the aplication information in 5 tables:

-   `user`: Stores user information for their login credentials as well as user statistics from matches

-   `match`: Record of all matches played, indicating what users participated, their respective score and if the match was from a tournament

-   `userTournament`: Table that stores what users are participating in a tournament

-   `tournament`: Table that stores the information of the tournaments, indicating the status of the tournament, the number of participants and the date of the tournament

-   `friend`: Table that stores the relationships between users, indicating if they are friends or if they have a pending friend request

![DB schema image](https://github.com/Paches19/transcendence/assets/21156058/9b4bf1d4-24a8-4cc7-82ee-a3a51a1e5cf5)
