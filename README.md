# container for contentful backup

## export
[documentation](https://github.com/contentful/contentful-cli/tree/master/docs/space/export)

```
	docker-compose run docker-contentful sh -c 'cd source && contentful space export \
		--space-id "[spaceId]" \
		--management-token "[managementToken]"'
```

## import
[documentation](https://github.com/contentful/contentful-cli/tree/master/docs/space/import)

```
	docker-compose run docker-contentful sh -c 'cd source && contentful space import \
		--space-id "[spaceId]" \
		--management-token "[managementToken]" \
		--content-model-only  "true"
		--content-file "./[fileName]"'
```