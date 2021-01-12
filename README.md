# container for contentful backup
## uses contentful-export

[documentation](https://github.com/contentful/contentful-export)

	docker-compose run docker-contentful sh -c 'cd source && contentful-export --space-id "[spaceId]" --management-token "[managementToken]"'