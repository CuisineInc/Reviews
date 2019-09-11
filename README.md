# Cuisine Inc Reviews

> Reviews section for the Cuisine Inc restaurant reservation application

## Related Projects

  - https://github.com/CuisineInc/Reservations
  - https://github.com/CuisineInc/Photo-Gallery
  - https://github.com/CuisineInc/Menu

## Table of Contents

1. [Usage](#Usage)
1. [Requirements](#requirements)
1. [Development](#development)

## Usage

> Some usage instructions

## Requirements

An `nvmrc` file is included if using [nvm](https://github.com/creationix/nvm).

- Node 6.13.0
- etc

## Development

### Installing Dependencies

From within the root directory:

```sh
npm install -g webpack
npm install
```

## RESTful CRUD API
For creating: app.get ~ "/api/reviews/:restaurantName" (GET)

For posting: app.post ~ "/api/reviews" (POST)

For updating: app.put ~ "/api/reviews/:restaurantName" (PUT)

For deleting: app.delete ~ "/api/reviews/:restaurantName" (DELETE)

Reviews

Create/POST:
Input/parameters: {
	user_id,
	restaurant_id,
	review,
	overall,
	food,
	service,
	ambience,
	value,
	noise,
	would_recommend,
	date
}
Reponse: {
	reviews_id
}

Read/GET:
Input/parameters: {
	reviews_id
}
Response: {
	user_id,
	restaurant_id,
	review,
	overall,
	food,
	service,
	ambience,
	value,
	noise,
	would_recommend,
	date
}

Update/PUT:
Input/parameters: {
	reviews_id,
	user_id,
	restaurant_id,
	review,
	overall,
	food,
	service,
	ambience,
	value,
	noise,
	would_recommend,
	date
}
Reponse: {
	reviews_id
}

Delete/DELETE
Update/PUT:
Input/parameters: {
	reviews_id,
}
Reponse: {
	success
}

