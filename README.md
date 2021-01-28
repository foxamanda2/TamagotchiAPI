# TamagotchiAPI

# TamagotchiAPI

## Problem

- A User needs to create a virtual pet with a web API. It needs to create, read, update, and delete.

## Examples

- The Api should be able to add a pet, but only should return the name. The other properties should have a default.
- A pet should be able to be deleted from the database
- When scolding a pet it should subtract 5 from the happiness level and create a new scolding for the pet with the time
- When feeding a pet it should find the pet and subtract 5 from its hunger level and add 3 to its happiness. This should also create a new feeding for the pet.
- If you play with the pet it will add 5 to its happiness and add 3 to its hunger. This will create a new playtime for the pet.
- If get all pets is used it should return all the pets in the API.
- Get id should return all the pets with a specific Id.
- The happiness of the pet will be unlimited (for the explorer mode), but the happiness should not go below 0.
- The hunger is unlimited (for explorer mode), but should not go below 0.

## Data

- Pets Table

  - Id (int)
  - Name(string)
  - Birthday (DateTime) default
  - HungerLevel (int) default=0
  - HappinessLevel(int) default=0

- Playtimes Table

  - Id (int)
  - When (DateTime) default
  - PetId(int-foreign key to pet)

- Feedings

  - Id (int)
  - When (DateTime) default
  - PetId(int-foreign key to pet)

- Scoldings
  - Id (int)
  - When (DateTime) default
  - PetId(int-foreign key to pet)
