install:
	@helm install memo-client ./memo-app-client --values memo-app-client/values.yaml
	@helm install memo-db ./memo-app-db --values memo-app-db/values.yaml
	@helm install memo-server ./memo-app-server --values memo-app-server/values.yaml

update:
	@helm upgrade memo-client ./memo-app-client --values memo-app-client/values.yaml
	@helm upgrade memo-db ./memo-app-db --values memo-app-db/values.yaml
	@helm upgrade memo-server ./memo-app-server --values memo-app-server/values.yaml

purge:
	@helm ls --all --short | xargs -L1 helm delete