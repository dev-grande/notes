# PSQL database - Docker
## Table of Contents 

- [Installation](#installation)
- [Usage](#usage)

---

## Installation

> https://www.postgresql.org/download/

- Follow the PSQL download instructions for your machine.

> https://www.docker.com/get-started

- Create a Docker account.
- Download Docker for Desktop for your corresponding machine.
- Once the download is finished sign in with your credentials made in step 1.

### Clone

- Clone the following repo to your local machine using `https://https://github.com/invest-io/backend`

### Setup

> In the /backend/db directory run the following command to create and start the container with the Docker application.

```shell
$ docker-compose up -d
```

---

## Usage

> After set up, you can now log into the psql server which should be mapped to PORT 5432 on your machine with the following command.

```shell
$ export PGPASSWORD='test_password'; psql -h localhost -p 5432 -U test_user -d investio
```


> To stop and clear the Docker application and container use the following commands in the /backend/db directory. 

```shell
$ docker stop $(docker ps -a -q) && docker rm $(docker ps -a -q)
$ docker volume prune -f
```

---


## frontend

**Question 1**

* why use react over other frameworks? advantages/disadvantages?

<details><summary>**Answer**</summary><p>

React is well known for its ease of use, reusability, and modularity as your code base grows. 
  
**PROS**
- Create reusable UI components
- Easy to learn; It combines the use of HTML and Javascript
- Efficiency when updating the UI. Compared to updating the whole web page (all the components) it updates specific components that trigger when needed.
- High Performance - allows for fast and reposive UI

**CONS**
- Focuses on View more in Model-View-Controller (MVC) pattern. Model and Controller aspect must be integrated with additional tools.
- JSX learning curve
- Fast-paced development may make it hard to keep learning all the new tools with each update.

</p></details>

**Question 2**

* why use redux? when to use it / when not to use it?

<details><summary>**Answer**</summary><p>

Redux is a useful state management tool that makes it easier to mangage the state of your application with the ease of accessing and updating the state globally vs. locally for each component.  This removes the complications of passing the state up and down between compoments. 

*When to use it?*
- A good amount of data is being passed between components.
- If you have difficulty detecting/tracing changes to the state.

*When not to use it?*
- Barely any data is not being passed between components.
- If you already have a predefined way of sharing and arranging the state across compoments.

</p></details>
