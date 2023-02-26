# Web infrastructure design

![web_structure](https://media.geeksforgeeks.org/wp-content/uploads/20220817182651/NetworkInfrastructure1.png)

Web Applications Infrastructure/Web Infrastructure also called internet infrastructure is the physical hardware, transmission media, and software used to interconnect computers and users on the Internet.

- Simple Web Infrastructure
- Distributed Web Infrastructure
- Monitored Web Infrastructure

## Learning Objectives

- In this project we learned how to draw a diagram to represent  the web stack built in `*sysadmin/devops*` track of ALX SE School project work.
- We discussed what each component of the diagram is doing
- Our team explored the concept of `system redundancy`
- We had fun discussing important web infrastructure design acronyms: `LAMP`, `SPOF`, `QPS`

#### Here is the design we came up with 

## Simple Web Infrastructure

![](https://miro.medium.com/max/720/1*xKd1CchSaSKV83Oizju8kg.webp)

- 1 server
- 1 web server `(Nginx)`
- 1 application server
- 1 application files (your code base)
- 1 database `(MySQL)`
- 1 domain name `foobar.com` configured with a `www` record that points to your server IP `8.8.8.8`

## Distrubuted Web Infrasture

![](https://upload.wikimedia.org/wikipedia/commons/5/55/Network_Architecture_Diagram_-_Distributed_Web_Infrastructure.pdf)

- 2 servers
- 1 web server `(Nginx)`
- 1 application server
- 1 load-balancer `(HAproxy)`
- 1 set of application files (your code base)
- 1 database `(MySQL)`

## Monitored web infrastructure

![](https://miro.medium.com/max/720/1*t7oSAWV7gtp-WSRNXfM9Hw.webp)

- 3 firewalls
- 1 SSL certificate to serve www.foobar.com over HTTPS
- 3 monitoring clients (data collector for Sumologic or other monitoring services)


## THIS PROJECT WAS HANDLED BY:

### 1. MONEHIN FEYISARA

>    EMAIL: monehinstephen@gmail.com

>    COUNTRY: Nigeria

>    PROFESSION: Software Engineer | AI Engineer | Front end dev | Graphic Designer

###  2. SUNDAY AUDU

>   EMAIL:

>   COUNTRY: Nigeria

>   PROFESSION: Software Engineer


###  3. TAGBOR SIMON

>   EMAIL: simontagbor360@gmail.com

>   COUNTRY: Ghana

>   PROFESSION: Software Engineer 
 
