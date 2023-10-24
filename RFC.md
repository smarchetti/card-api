## RFC

### Entities

* **sport**
  * _fields_
    * id
    * slug
    * name
  * _relationships_
    * products (array of product)
* **product**
  * _fields_
    * id
    * slug
    * sport_id
    * name
  * _relationships_
    * sport
    * sets (array of set)
* **set**
  * _fields_
    * id
    * slug
    * product_id
    * name
  * _relationships_
    * product
    * parallels (array of parallels)
* **parallel**
  * _fields_
    * id
    * slug
    * set_id
    * name
  * _relationships_
    * set
    * cards (array of card)
* **card**
  * _fields_
    * id
    * slug
    * parallel_id
    * number
    * name
  * _relationships_
    * parallel
    * players (array of player)
    * teams (array of team)
    * attributes (array of attribute)
* **player**
  * _fields_
    * id
    * slug
    * name
  * _relationships_
    * cards (array of card)
* **team**
  * _fields_
    * id
    * slug
    * name
  * _relationships_
    * cards (array of card)
* **attribute**
  * _fields_
    * id
    * slug
    * name
  * _relationships_
    * cards (array of card)
