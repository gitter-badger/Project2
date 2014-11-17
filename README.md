TODO:

- [ ] add associations
- [ ] add validations to README
- [ ] create seed
- [ ] create controllers
- [ ] create views
- [ ] write tests

Zen Crayons
===========
[![Gitter](https://badges.gitter.im/Join Chat.svg)](https://gitter.im/ysshah/Project2?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Add crayons to a box of crayons and apply them to a canvas. Share your boxes and your canvases with other people.

## Models

### User
_We will use Devise to manage users._
#### Associations

has many users (Each user has friends that he can share boxes and canvases with)

has many boxes

has many canvases

#### Controller

profile (contains boxes, canvases, etc.)

friend stuff

add a box

remove a box

### Box
_Boxes can be shared and contain crayons._
#### Associations

belongs to user

#### Controller

create a box

destroy a box

view a box

add a crayon

remove a crayon

### Crayon
_Each crayon is created by a user, and is in a box._
#### Associations

belongs to box

#### Controller

create a crayon

destroy a crayon

### Canvas
_A canvas can have crayons applied to it. Users can share their canvases._
#### Associations

belongs to user

has many boxes

has many crayons

#### Controller

create a canvas

destroy a canvas

add a box

remove a box

apply a crayon
