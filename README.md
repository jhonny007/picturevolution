# picturEvolution
Evolution of art works by adding, changing, coloring ...

You know the coloring books for adults where you can spend hours or even days creating beautiful unique copies?
While one purpose is to relax while coloring them it would be nice to share your version with the world.

see http://picturEvolution.org for an old static one-page proof of concept

This will be possible with picturEvolution:
  * DONE everyone can share her art works with the world
  * TODO you can rate the artworks with up to five stars
  * TODO you can sell your own art works for one Euro as PDF Download
  * TODO you can auction the original for a price you can define
  * TODO modified copies can be uploaded and connected to the original

The revenues will be divided: 
  * 1/3 of the revenues are donated to http://plant-for-the-planet.org to do something against the climate change 
  * 1/3 is used for further development and hosting costs
  * 1/3 goes back to the creator of the artwork

## Prerequisites

You will need [Leiningen][1] 1.7.0 or above installed.

[1]: https://github.com/technomancy/leiningen

## Running

To start a web server for the application, run:

    lein ring server

## Database
Use Postgresql (9.5.14)
    sudo -i -u postgres
    psql

    CREATE USER admin;
    alter user admin with password 'admin';

    CREATE DATABASE PICTUREVOLUTION OWNER admin;
    
    psql admin -h 127.0.0.1 -d picturevolution
    
    \q to quit
    \d show relations

## TODOs
  * IN-PROGRESS add statistics (users, images, downloads, size of images, last added user, last added picture, ...)
  * provide download for free artwork (static download file)
  * provide download for every artwork (create pdf and download file)
  * add gravatar to home galleries
  * use name from gravatar profile
  * rotate the image (portrait/landscape) 

## License

GNU General Public License v3.0


Copyright © 2018 Christian Gruber
