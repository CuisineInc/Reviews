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
GET /api/:restaurantName/reviews/

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

Review: Review description and text contents

Overall, Food, Service, Ambience, Value: Rating 1-5

Noise: Noise level


POST /api/:restaurantName/reviews
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

For updating: app.put ~ "/api/reviews/:restaurantName" (PUT)
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
Review: Review description and text contents
Overall, Food, Service, Ambience, Value: Rating 1-5
Noise: Noise level

For deleting: app.delete ~ "/api/reviews/:restaurantName" (DELETE)
Input/parameters: {
	reviews_id,
}
Reponse: {
	success
}
Success: boolean of whether the delete was successful


